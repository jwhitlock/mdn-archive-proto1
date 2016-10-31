---
version: prototype1
revision_id: 1136223
locale: en-US
slug: Archive/JXON
tags: "AJAX" "DOM" "JSON" "JXON" "XML" "XPath" "Object" "Document" "XMLHttpRequest" "Object-Oriented"
title: JXON
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p><strong>JXON</strong> (lossless <strong>J</strong>avaScript <strong>X</strong>ML <strong>O</strong>bject <strong>N</strong>otation) is a generic name by which is defined the representation of JavaScript Objects using <a href="/en/XML" title="en/XML">XML</a>. There are no real standards for this conversion, but <a href="#The_Parker_Convention" title="The Parker Convention">some conventions begin to appear on the web</a>. There are some cases in which the whole content of an XML document must be read from the JavaScript interpreter (like for web-apps languages or settings XML documents, for example). In these cases JXON could represent the most practical way.</p>

<p>In this article we will show how to convert a parsed XML {{ domxref("document") }} (i.e. an instance of <a href="http://www.w3.org/TR/DOM-Level-2-Core/core.html#i-Document"><code>Document</code></a>) to a JavaScript Object tree (i.e. a tree of nested instances of <a href="/en/JavaScript/Reference/Global_Objects/Object" title="en/JavaScript/Reference/Global_Objects/Object"><code>Object</code></a>) and viceversa, with some different algorithms. It could be useful to read the&nbsp;<a href="/en/XML_Introduction" title="en/XML_Introduction">XML introduction article</a> first.</p>

<p>If you want <strong>a complete bidirectional JXON library</strong> (modelled on the <a href="/en/JavaScript/Reference/Global_Objects/JSON" title="en/JavaScript/Reference/Global_Objects/JSON"><code>JSON</code></a> global object), skip to the <a href="#Appendix.3A_a_complete.2C_bidirectional.2C_JXON_library" title="A complete JXON library">dedicated paragraph</a> (but please read the <a href="#const_compatibility" title="#const_compatibility">note about the <code>const</code> statement compatibility</a>).</p>

<div class="note"><strong>Note:</strong> If you are interested to address only some parts of an XML document (and are not starting in JavaScript/JSON for templating purposes), use <a href="/en/XPath" title="en/XPath">XPath</a> instead of converting the whole document into JSON.</div>

<h2 id="Conversion_snippets">Conversion snippets</h2>

<p>Now imagine you&nbsp;have this sample XML document:</p>

<h5 id="example.xml">example.xml</h5>

<pre class="brush: xml">
&lt;?xml version="1.0"?&gt;
&lt;!DOCTYPE catalog SYSTEM "catalog.dtd"&gt;
&lt;catalog&gt;
&nbsp;&nbsp;&lt;product description="Cardigan Sweater"&gt;
&nbsp;&nbsp;&nbsp;&lt;catalog_item gender="Men's"&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;item_number&gt;QWZ5671&lt;/item_number&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;price&gt;39.95&lt;/price&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;size description="Medium"&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;color_swatch image="red_cardigan.jpg"&gt;Red&lt;/color_swatch&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;color_swatch image="burgundy_cardigan.jpg"&gt;Burgundy&lt;/color_swatch&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;/size&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;size description="Large"&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;color_swatch image="red_cardigan.jpg"&gt;Red&lt;/color_swatch&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;color_swatch image="burgundy_cardigan.jpg"&gt;Burgundy&lt;/color_swatch&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;/size&gt;
&nbsp;&nbsp;&nbsp;&lt;/catalog_item&gt;
&nbsp;&nbsp;&nbsp;&lt;catalog_item gender="Women's"&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;item_number&gt;RRX9856&lt;/item_number&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;discount_until&gt;Dec 25, 1995&lt;/discount_until&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;price&gt;42.50&lt;/price&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;size description="Medium"&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;color_swatch image="black_cardigan.jpg"&gt;Black&lt;/color_swatch&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;/size&gt;
&nbsp;&nbsp;&nbsp;&lt;/catalog_item&gt;
&nbsp;&nbsp;&lt;/product&gt;
&nbsp;&nbsp;&lt;script type="text/javascript"&gt;&lt;![CDATA[function matchwo(a,b) {
&nbsp;&nbsp;&nbsp;&nbsp;if (a &lt; b &amp;&amp; a &lt; 0) { return 1; }
&nbsp;&nbsp;&nbsp;&nbsp;else { return 0; }
}]]&gt;&lt;/script&gt;
&lt;/catalog&gt;
</pre>

<p>First, create a DOM tree like the previous example as described in the <a href="/en/How_to_create_a_DOM_tree" title="en/How_to_create_a_DOM_tree">How to Create a DOM tree</a> article. If you have already have a DOM tree from using {{ domxref("XMLHttpRequest") }}, skip to the next paragraph.</p>

<div class="note"><strong>Note:</strong> If you are using an instance of <a href="/en-US/docs/DOM/XMLHttpRequest" title="/en-US/docs/DOM/XMLHttpRequest"><code>XMLHttpRequest</code></a> in order to retrieve your XML file, please use the <code>yourRequest.responseXML</code> property to get a <em>parsed</em> XML document. Don't use <code>yourRequest.responseText</code>!</div>

<p>The algorithms proposed here (see: <a href="#Algorithm_.231.3A_a_verbose_way" title="Go to JXON algorithm #1">#1</a>, <a href="#Algorithm_.232.3A_a_less_verbose_way" title="Go to JXON algorithm #2">#2</a>, <a href="#Algorithm_.233.3A_a_synthetic_technique" title="Go to JXON algorithm #3">#3</a>, <a href="#Algorithm_.234.3A_a_very_minimalist_way" title="Go to JXON algorithm #4">#4</a>) will consider only the following types of nodes and their attributes:</p>

<ol>
 <li>{{ domxref("Document") }} (only as function argument),</li>
 <li>{{ domxref("DocumentFragment") }} (only as function argument),</li>
 <li>{{ domxref("Element") }},</li>
 <li>{{ domxref("Text") }} (never as function argument),</li>
 <li>{{ domxref("CDATASection") }} (never as function argument),</li>
 <li>{{ domxref("Attr") }} (never as function argument).</li>
</ol>

<p>This is a good and <strong>standardized</strong> compromise for a JavaScript usage, since all of the information of an XML Document is contained in these&nbsp;node types. All other information (like processing instructions, schemas, comments, etc.) will be lost. This type of algorithm&nbsp;is still considered&nbsp;<strong>lossless</strong>, since what is lost is <strong>meta-information</strong> and not <strong>information</strong>.</p>

<p>In order to avoid conflicts, the representation of nodes and attributes names is <strong>case insensitive</strong> (always rendered in <strong>lower case</strong>), so objects' local property names set&nbsp;using JavaScript must always have some kind of capitalization (that is, at least one capital letter somewhere in their names), as you can see below.</p>

<p>The following algorithms are somewhat based on the <a href="#The_Parker_Convention" title="The Parker Convention">Parker convention, version 0.4</a>, which prescribes the <strong>transformation of <a href="/en/DOM/Node.nodeName" title="en/DOM/Node.nodeName">tags names</a> into <a href="/en/JavaScript/Guide/Working_with_Objects#Objects_and_properties" title="en/Core_JavaScript_1.5_Guide/Working_with_Objects#Objects_and_properties">object properties names</a></strong> and the <strong>recognition of the <a href="/en/JavaScript/Reference/Operators/typeof" title="en/JavaScript/Reference/Operators/typeof"><code>typeof</code></a></strong> of all the collected <a href="/en/DOM/Node.nodeValue" title="en/DOM/Node.nodeValue"><code>text content</code></a> of each tag (plain text parsing); but <a href="#Code_considerations" title="Code considerations">with some differences</a> (so, one can say that we follow <em>a our convention</em>). Moreover, <strong>all algorithms are equally lossless for the contemplated nodes</strong>.</p>

<p>We consider <strong><a href="#Algorithm_.233.3A_a_synthetic_technique" title="Go to JXON algorithm #3">the third algorithm</a> as the most representative and practical JXON parsing algorithm</strong>.</p>

<p>Now let's serialize <code>doc</code> — the DOM tree — to a JavaScript Object Tree (you can read more about <a href="/en/JavaScript/Guide/Working_with_Objects" title="Working with Objects">working with Objects</a> and&nbsp;<a href="/en/JavaScript/Introduction_to_Object-Oriented_JavaScript" title="Introduction to Object-Oriented JavaScript – MDC">how Javascript is Object-Oriented</a>). We can use several algorithms to convert its content to a Javascript Object Tree.</p>

<h3 id="Algorithm_1_a_verbose_way">Algorithm #1: a verbose way</h3>

<p>This simple recursive constructor will convert an XML DOM tree to a JavaScript Object tree. The text content of each element is stored into the <code>keyValue</code> property, while <code>nodeAttributes</code>, if they exist, are listed under the child object <code>keyAttributes</code>. The constructor's argument can be the entire XML <code>Document</code>, a <code>DocumentFragment</code> or simply an <code>Element</code> node.</p>

<pre class="brush: js">
/*\
|*|
|*|&nbsp; JXON Snippet #1 - Mozilla Developer Network
|*|
|*|&nbsp; https://developer.mozilla.org/en-US/docs/JXON
|*|&nbsp; https://developer.mozilla.org/User:fusionchess
|*|
|*|&nbsp; This framework is released under the GNU Public License, version 3 or later.
|*|&nbsp; http://www.gnu.org/licenses/gpl-3.0-standalone.html
|*|
\*/

function parseText (sValue) {
&nbsp;&nbsp;if (/^\s*$/.test(sValue)) { return null; }
&nbsp;&nbsp;if (/^(?:true|false)$/i.test(sValue)) { return sValue.toLowerCase() === "true"; }
&nbsp;&nbsp;if (isFinite(sValue)) { return parseFloat(sValue); }
&nbsp;&nbsp;if (isFinite(Date.parse(sValue))) { return new Date(sValue); }
&nbsp;&nbsp;return sValue;
}

function JXONTree (oXMLParent) {
 &nbsp;var nAttrLen = 0, nLength = 0, sCollectedTxt = "";
 &nbsp;if (oXMLParent.hasChildNodes()) {
 &nbsp;  for (var oNode, sProp, vContent, nItem = 0; nItem &lt; oXMLParent.childNodes.length; nItem++) {
 &nbsp;&nbsp;&nbsp;&nbsp; oNode = oXMLParent.childNodes.item(nItem);
 &nbsp;&nbsp;&nbsp;&nbsp; if ((oNode.nodeType - 1 | 1) === 3) { sCollectedTxt += oNode.nodeType === 3 ? oNode.nodeValue.trim() : oNode.nodeValue; } // nodeType is "Text" (3) or "CDATASection" (4)
 &nbsp;&nbsp;&nbsp;&nbsp; else if (oNode.nodeType === 1 &amp;&amp; !oNode.prefix) { // nodeType is "Element" (1)
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; sProp = oNode.nodeName.toLowerCase();
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; vContent = new JXONTree(oNode);
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (this.hasOwnProperty(sProp)) {
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (this[sProp].constructor !== Array) { this[sProp] = [this[sProp]]; }
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; this[sProp].push(vContent);
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } else { this[sProp] = vContent; nLength++; }
 &nbsp;&nbsp;&nbsp;&nbsp; }
 &nbsp;&nbsp; }
 &nbsp;&nbsp; this.keyValue = parseText(sCollectedTxt);
 &nbsp;} else { this.keyValue = null; }
 &nbsp;if (oParentNode.hasAttributes &amp;&amp; oXMLParent.hasAttributes()) {
 &nbsp;&nbsp; var oAttrib;
 &nbsp;&nbsp; this.keyAttributes = {};
 &nbsp;&nbsp; for (nAttrLen; nAttrLen &lt; oXMLParent.attributes.length; nAttrLen++) {
 &nbsp;&nbsp;&nbsp;&nbsp; oAttrib = oXMLParent.attributes.item(nAttrLen);
 &nbsp;&nbsp;&nbsp;&nbsp; this.keyAttributes[oAttrib.name.toLowerCase()] = parseText(oAttrib.value.trim());
 &nbsp;&nbsp; }
 &nbsp;}
 &nbsp;/*
 &nbsp;* Optional properties...

 &nbsp;this.keyLength = nLength;
 &nbsp;this.attributesLength = nAttrLen;
&nbsp; // this.DOMNode = oXMLParent;

&nbsp; */

 &nbsp;/* Object.freeze(this); */
}

/*
* Optional methods... Uncomment the optional properties first!

JXONTree.prototype.valueOf = function () { return this.keyValue; };
JXONTree.prototype.toString = function () { return String(this.keyValue); };
JXONTree.prototype.getItem = function (nItem) {
 &nbsp;if (nLength === 0) { return null; }
 &nbsp;var nCount = 0;
 &nbsp;for (var sKey in this) { if (nCount === nItem) { return this[sKey]; } nCount++; }
 &nbsp;return null;
};
JXONTree.prototype.getAttribute = function (nAttrId) {
&nbsp; if (nAttrLen === 0 || nAttrId + 1 &gt; nAttrLen) { return null; }
&nbsp; var nAttr = 0;
&nbsp; for (var sAttrName in this.keyAttributes) { if (nAttr === nAttrId) { return this.keyAttributes[sAttrName]; } nAttr++; }
&nbsp; return null;
};
JXONTree.prototype.hasChildren = function () { return this.keyLength &gt; 0; };

*/

var myObject = new JXONTree(doc);
// we got our javascript object! try: alert(JSON.stringify(myObject));
</pre>

<div class="note"><strong>Note:</strong> If you want to freeze the whole object tree (because of the "static" nature of an XML document), uncomment the string: <code>/* Object.freeze(this); */</code>. The <code><a href="/en/JavaScript/Reference/Global_Objects/Object/freeze" title="en/JavaScript/Reference/Global_Objects/Object/freeze">Object.freeze()</a></code> method prevents new properties from being added to it, prevents existing properties from being removed and prevents existing properties, or their enumerability, configurability, or writability, from being changed. In essence the object tree is made effectively immutable.</div>

<p>With this algorithm <a href="#example.xml" title="Go to the sample XML document">our example</a> becomes:</p>

<pre class="brush: js">
{
&nbsp;"catalog": {
&nbsp;&nbsp;&nbsp;"product": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"catalog_item": [{
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"item_number": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "QWZ5671"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"price": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": 39.95
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"size": [{
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color_swatch": [{
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "Red",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyAttributes": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"image": "red_cardigan.jpg"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "Burgundy",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyAttributes": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"image": "burgundy_cardigan.jpg"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}],
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": null,
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyAttributes": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"description": "Medium"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color_swatch": [{
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "Red",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyAttributes": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"image": "red_cardigan.jpg"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "Burgundy",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyAttributes": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"image": "burgundy_cardigan.jpg"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}],
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"purchased": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": null
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": null,
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyAttributes": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"description": "Large"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}],
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": null,
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyAttributes": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"gender": "Men's"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"item_number": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "RRX9856"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"discount_until": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": new Date(1995, 11, 25)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"price": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": 42.5
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"size": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color_swatch": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "Black",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyAttributes": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"image": "black_cardigan.jpg"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": null,
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyAttributes": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"description": "Medium"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": null,
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyAttributes": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"gender": "Women's"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}],
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": null,
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyAttributes": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"description": "Cardigan Sweater"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;"script": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "function matchwo(a,b) {\n&nbsp;if (a &lt; b &amp;&amp; a &lt; 0) { return 1; }\n&nbsp;else { return 0; }\n}",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyAttributes": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"type": "text/javascript"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;"keyValue": null
&nbsp;},
&nbsp;"keyValue": null
}
</pre>

<p>This is a recommanded technique if you don't know the structure of the XML document.</p>

<h3 id="Algorithm_2_a_less_verbose_way">Algorithm #2: a less verbose way</h3>

<p>Here is another, simpler, conversion method, in which <code>nodeAttributes</code> are listed under the same object of child nodes but have the “@” prefix (as suggested by the <a href="http://badgerfish.ning.com/" title="BadgerFish convention">BadgerFish Convention</a>). As above, the text content is stored into the <code>keyValue</code> property. The constructor's argument can be the entire XML <code>Document</code>, a <code>DocumentFragment</code> or simply an <code>Element</code> node of it.</p>

<pre class="brush: js">
/*\
|*|
|*|&nbsp; JXON Snippet #2 - Mozilla Developer Network
|*|
|*|&nbsp; https://developer.mozilla.org/en-US/docs/JXON
|*|&nbsp; https://developer.mozilla.org/User:fusionchess
|*|
|*|&nbsp; This framework is released under the GNU Public License, version 3 or later.
|*|&nbsp; http://www.gnu.org/licenses/gpl-3.0-standalone.html
|*|
\*/

function parseText (sValue) {
&nbsp;&nbsp;if (/^\s*$/.test(sValue)) { return null; }
&nbsp;&nbsp;if (/^(?:true|false)$/i.test(sValue)) { return sValue.toLowerCase() === "true"; }
&nbsp;&nbsp;if (isFinite(sValue)) { return parseFloat(sValue); }
&nbsp;&nbsp;if (isFinite(Date.parse(sValue))) { return new Date(sValue); }
&nbsp;&nbsp;return sValue;
}

function JXONTree (oXMLParent) {
&nbsp;&nbsp;if (oXMLParent.hasChildNodes()) {
&nbsp;&nbsp;&nbsp;&nbsp;var sCollectedTxt = "";
&nbsp;&nbsp;&nbsp;&nbsp;for (var oNode, sProp, vContent, nItem = 0; nItem &lt; oXMLParent.childNodes.length; nItem++) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;oNode = oXMLParent.childNodes.item(nItem);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if ((oNode.nodeType - 1 | 1) === 3) { sCollectedTxt += oNode.nodeType === 3 ? oNode.nodeValue.trim() : oNode.nodeValue; }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;else if (oNode.nodeType === 1 &amp;&amp; !oNode.prefix) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sProp = oNode.nodeName.toLowerCase();
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;vContent = new JXONTree(oNode);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if (this.hasOwnProperty(sProp)) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if (this[sProp].constructor !== Array) { this[sProp] = [this[sProp]]; }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;this[sProp].push(vContent);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;} else { this[sProp] = vContent; }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;if (sCollectedTxt) { this.keyValue = parseText(sCollectedTxt); }
&nbsp;&nbsp;}
&nbsp;&nbsp;if (oParentNode.hasAttributes &amp;&amp; oXMLParent.hasAttributes()) {
&nbsp;&nbsp;&nbsp;&nbsp;var oAttrib;
&nbsp;&nbsp;&nbsp;&nbsp;for (var nAttrib = 0; nAttrib &lt; oXMLParent.attributes.length; nAttrib++) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;oAttrib = oXMLParent.attributes.item(nAttrib);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;this["@" + oAttrib.name.toLowerCase()] = parseText(oAttrib.value.trim());
&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;}
&nbsp;&nbsp;/* Object.freeze(this); */
}

var myObject = new JXONTree(doc);
// we got our javascript object! try: alert(JSON.stringify(myObject));
</pre>

<div class="note"><strong>Note:</strong> If you want to freeze the whole object tree (because of the "static" nature of an XML document), uncomment the string: <code>/* Object.freeze(this); */</code>. The <code><a href="/en/JavaScript/Reference/Global_Objects/Object/freeze" title="en/JavaScript/Reference/Global_Objects/Object/freeze">Object.freeze()</a></code> method prevents new properties from being added to it, prevents existing properties from being removed and prevents existing properties, or their enumerability, configurability, or writability, from being changed. In essence the object tree is made effectively immutable.</div>

<p>With this algorithm <a href="#example.xml" title="Go to the sample XML document">our example</a> becomes:</p>

<pre class="brush: js">
{
&nbsp;&nbsp;"catalog": {
&nbsp;&nbsp;&nbsp;&nbsp;"product": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"catalog_item": [{
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"item_number": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "QWZ5671"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"price": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": 39.95
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"size": [{
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color_swatch": [{
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "Red",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@image": "red_cardigan.jpg"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "Burgundy",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@image": "burgundy_cardigan.jpg"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}],
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@description": "Medium"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color_swatch": [{
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "Red",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@image": "red_cardigan.jpg"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "Burgundy",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@image": "burgundy_cardigan.jpg"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}],
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@description": "Large"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}],
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@gender": "Men's"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"item_number": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "RRX9856"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"discount_until": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": new Date(1995, 11, 25)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"price": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": 42.5
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"size": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color_swatch": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "Black",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@image": "black_cardigan.jpg"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@description": "Medium"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@gender": "Women's"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}],
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@description": "Cardigan Sweater"
&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;"script": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "function matchwo(a,b) {\n&nbsp;&nbsp;if (a &lt; b &amp;&amp; a &lt; 0) { return 1; }\n&nbsp;&nbsp;else { return 0; }\n}",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@type": "text/javascript"
&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;}
}
</pre>

<p>This is a possible technique to use if you partially know the structure of the XML document.</p>

<h3 id="Algorithm_3_a_synthetic_technique">Algorithm #3: a synthetic technique</h3>

<p>Here is another method of conversion. This algorithm is the closest to the <a href="#The_Parker_Convention" title="The Parker Convention">Parker convention</a>. It is very similar to the previous one, except that nodes which do not contain other recognizable nodes than <code>Text</code> or <code>CDATASection</code> are not treated as objects, but directly as booleans, strings, numbers or <code>Date</code> objects (see the <a href="#The_Parker_Convention" title="The Parker Convention">Parker convention</a>). Empty nodes (i.e. which do not contain other <code>Element</code> nodes, <code>Text</code> nodes, <code>CDATASection</code> nodes or <code>Attr</code> nodes) have the default value <code>true</code> (see the <a href="#Code_considerations" title="Code considerations">Code considerations</a>). Also, this time we use a&nbsp;function instead of a&nbsp;constructor. The function's argument can be the entire XML {{ domxref("Document") }}, a {{ domxref("DocumentFragment") }}, or simply an {{ domxref("Element") }} node within it.&nbsp;<code>nodeAttributes</code> have the “@” prefix, as suggested by the <a href="http://badgerfish.ning.com/" title="BadgerFish convention">BadgerFish Convention</a>. <strong>In many cases, this is the most practical conversion method</strong>.</p>

<pre class="brush: js">
/*\
|*|
|*|&nbsp; JXON Snippet #3 - Mozilla Developer Network
|*|
|*|&nbsp; https://developer.mozilla.org/en-US/docs/JXON
|*|&nbsp; https://developer.mozilla.org/User:fusionchess
|*|
|*|&nbsp; This framework is released under the GNU Public License, version 3 or later.
|*|&nbsp; http://www.gnu.org/licenses/gpl-3.0-standalone.html
|*|
\*/

function parseText (sValue) {
&nbsp;&nbsp;if (/^\s*$/.test(sValue)) { return null; }
&nbsp;&nbsp;if (/^(?:true|false)$/i.test(sValue)) { return sValue.toLowerCase() === "true"; }
&nbsp;&nbsp;if (isFinite(sValue)) { return parseFloat(sValue); }
&nbsp;&nbsp;if (isFinite(Date.parse(sValue))) { return new Date(sValue); }
&nbsp;&nbsp;return sValue;
}

function getJXONTree (oXMLParent) {
&nbsp;&nbsp;var vResult = /* put here the default value for empty nodes! */ true, nLength = 0, sCollectedTxt = "";
&nbsp;&nbsp;if (oXMLParent.hasAttributes &amp;&amp; oXMLParent.hasAttributes()) {
&nbsp;&nbsp;&nbsp;&nbsp;vResult = {};
&nbsp;&nbsp;&nbsp;&nbsp;for (nLength; nLength &lt; oXMLParent.attributes.length; nLength++) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;oAttrib = oXMLParent.attributes.item(nLength);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;vResult["@" + oAttrib.name.toLowerCase()] = parseText(oAttrib.value.trim());
&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;}
&nbsp;&nbsp;if (oXMLParent.hasChildNodes()) {
&nbsp;&nbsp;&nbsp;&nbsp;for (var oNode, sProp, vContent, nItem = 0; nItem &lt; oXMLParent.childNodes.length; nItem++) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;oNode = oXMLParent.childNodes.item(nItem);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if (oNode.nodeType === 4) { sCollectedTxt += oNode.nodeValue; } /* nodeType is "CDATASection" (4) */
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;else if (oNode.nodeType === 3) { sCollectedTxt += oNode.nodeValue.trim(); } /* nodeType is "Text" (3) */
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;else if (oNode.nodeType === 1 &amp;&amp; !oNode.prefix) { /* nodeType is "Element" (1) */
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if (nLength === 0) { vResult = {}; }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sProp = oNode.nodeName.toLowerCase();
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;vContent = getJXONTree(oNode);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if (vResult.hasOwnProperty(sProp)) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if (vResult[sProp].constructor !== Array) { vResult[sProp] = [vResult[sProp]]; }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;vResult[sProp].push(vContent);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;} else { vResult[sProp] = vContent; nLength++; }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;}
&nbsp;&nbsp;if (sCollectedTxt) { nLength &gt; 0 ? vResult.keyValue = parseText(sCollectedTxt) : vResult = parseText(sCollectedTxt); }
&nbsp;&nbsp;/* if (nLength &gt; 0) { Object.freeze(vResult); } */
&nbsp;&nbsp;return vResult;
}

var myObject = getJXONTree(doc);
// we got our javascript object! try: alert(JSON.stringify(myObject));
</pre>

<div class="note"><strong>Note:</strong> If you want to freeze the whole object tree (because of the "static" nature of an XML document), uncomment the string: <code>/* if (nLength &gt; 0) { Object.freeze(vResult); } */</code>. The <code><a href="/en/JavaScript/Reference/Global_Objects/Object/freeze" title="en/JavaScript/Reference/Global_Objects/Object/freeze">Object.freeze()</a></code> method prevents new properties from being added to it, prevents existing properties from being removed and prevents existing properties, or their enumerability, configurability, or writability, from being changed. In essence the object tree is made effectively immutable.</div>

<p>With this algorithm, <a href="#example.xml" title="Go to the sample XML document">our example</a> becomes:</p>

<pre class="brush: js">
{
&nbsp;&nbsp;"catalog": {
&nbsp;&nbsp;&nbsp;&nbsp;"product": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@description": "Cardigan Sweater",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"catalog_item": [{
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@gender": "Men's",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"item_number": "QWZ5671",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"price": 39.95,
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"size": [{
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@description": "Medium",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color_swatch": [{
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@image": "red_cardigan.jpg",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "Red"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@image": "burgundy_cardigan.jpg",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "Burgundy"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@description": "Large",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color_swatch": [{
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@image": "red_cardigan.jpg",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "Red"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@image": "burgundy_cardigan.jpg",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "Burgundy"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@gender": "Women's",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"item_number": "RRX9856",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"discount_until": new Date(1995, 11, 25),
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"price": 42.5,
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"size": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@description": "Medium",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"color_swatch": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@image": "black_cardigan.jpg",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "Black"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}]
&nbsp;&nbsp;&nbsp;&nbsp;},
&nbsp;&nbsp;&nbsp;&nbsp;"script": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"@type": "text/javascript",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"keyValue": "function matchwo(a,b) {\n&nbsp;&nbsp;if (a &lt; b &amp;&amp; a &lt; 0) { return 1; }\n&nbsp;&nbsp;else { return 0; }\n}"
&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;}
}
</pre>

<p>This is a recommended technique if you know the structure of the XML document.</p>

<h3 id="Algorithm_4_a_very_minimalist_way">Algorithm #4: a very minimalist way</h3>

<p>The following is another possible way to do the conversion. It is very close to the <a href="#The_Parker_Convention" title="The Parker Convention">Parker convention</a>, too. With this algorithm, all {{ domxref("Element") }} nodes that contain other child {{ domxref("Element") }}, {{ domxref("Text") }}, or {{ domxref("CDATASection") }} nodes in the same level are treated as instances of <code>Boolean</code>, <code>Number</code>, <code>String</code>, or <code>Date</code> Constructors. So any child <code>Element</code> node, if exists, will be nested in these types of objects.</p>

<p>For example:</p>

<pre class="brush: xml">
&lt;employee type="usher"&gt;John Smith&lt;/employee&gt;
&lt;manager&gt;Lisa Carlucci&lt;/manager&gt;
</pre>

<p>becomes</p>

<pre class="brush: js">
var myObject = {
  "employee": new String("John Smith"),
  "manager": "Lisa Carlucci"
};

myObject.employee["@type"] = "usher";

// test

alert(myObject.manager); // "Lisa Carlucci"
alert(myObject.employee["@type"]); // "usher"
alert(myObject.employee); // "John Smith"
</pre>

<div class="note"><strong>Note:</strong> This algorithm represents <em>a special case of conversion</em>. <strong>The generated JavaScript Object tree is not <a href="/en/JavaScript/Reference/Global_Objects/JSON/stringify" title="en/JavaScript/Reference/Global_Objects/JSON/stringify">stringifyable</a></strong> (see the <a href="#Code_considerations" title="Code considerations">Code considerations</a>). It is very practical for internal JavaScript access, but don't use it if you want to transfer the tree via JSON string!</div>

<p>As for the third algorithm, nodes which do not contain other recognizable nodes than <code>Text</code> or <code>CDATASection</code> are not treated as objects, but directly as booleans, strings, numbers (primitive values) or <code>Date</code> objects; and empty nodes (i.e. which do not contain other <code>Element</code> nodes, <code>Text</code> nodes, <code>CDATASection</code> nodes or <code>Attr</code> nodes) have the default value <code>true</code>. As for the third algorithm it is not used a constructor, but a function. The function's argument can be the entire XML <code>Document</code>, a <code>DocumentFragment</code> or simply an <code>Element</code> node of it.&nbsp;<code>nodeAttributes</code> have the “@” prefix, as suggested by the <a href="http://badgerfish.ning.com/" title="BadgerFish convention">BadgerFish Convention</a>.</p>

<pre class="brush: js">
/*\
|*|
|*|&nbsp; JXON Snippet #4 - Mozilla Developer Network
|*|
|*|&nbsp; https://developer.mozilla.org/en-US/docs/JXON
|*|&nbsp; https://developer.mozilla.org/User:fusionchess
|*|
|*|&nbsp; This framework is released under the GNU Public License, version 3 or later.
|*|&nbsp; http://www.gnu.org/licenses/gpl-3.0-standalone.html
|*|
\*/

function parseText (sValue) {
&nbsp;&nbsp;if (/^\s*$/.test(sValue)) { return null; }
&nbsp;&nbsp;if (/^(?:true|false)$/i.test(sValue)) { return sValue.toLowerCase() === "true"; }
&nbsp;&nbsp;if (isFinite(sValue)) { return parseFloat(sValue); }
&nbsp;&nbsp;if (isFinite(Date.parse(sValue))) { return new Date(sValue); }
&nbsp;&nbsp;return sValue;
}

function objectify (vValue) {
&nbsp;&nbsp;if (vValue === null) {
&nbsp;&nbsp;&nbsp;&nbsp;return new (function() {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;this.toString = function() { return "null"; }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;this.valueOf = function() { return null; }
&nbsp;&nbsp;&nbsp;&nbsp;})();
&nbsp;&nbsp;}
&nbsp;&nbsp;return vValue instanceof Object ? vValue : new vValue.constructor(vValue);
}

var aTmpEls = []; // loaded element nodes cache

function getJXONTree (oXMLParent) {
&nbsp;&nbsp;var&nbsp;&nbsp;sProp, vContent, vResult, nLength = 0, nLevelStart = aTmpEls.length,
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; nChildren = oXMLParent.hasChildNodes() ? oXMLParent.childNodes.length : 0, sCollectedTxt = "";

&nbsp;&nbsp;for (var oNode, nItem = 0; nItem &lt; nChildren; nItem++) {
&nbsp;&nbsp;&nbsp;&nbsp;oNode = oXMLParent.childNodes.item(nItem);
&nbsp;&nbsp;&nbsp;&nbsp;if (oNode.nodeType === 4) { sCollectedTxt += oNode.nodeValue; } /* nodeType is "CDATASection" (4) */
&nbsp;&nbsp;&nbsp;&nbsp;else if (oNode.nodeType === 3) { sCollectedTxt += oNode.nodeValue.trim(); } /* nodeType is "Text" (3) */
&nbsp;&nbsp;&nbsp;&nbsp;else if (oNode.nodeType === 1 &amp;&amp; !oNode.prefix) { aTmpEls.push(oNode); } /* nodeType is "Element" (1) */
&nbsp;&nbsp;}

&nbsp;&nbsp;var nLevelEnd = aTmpEls.length, vBuiltVal = parseText(sCollectedTxt);

&nbsp;&nbsp;if (oParentNode.hasAttributes &amp;&amp; oXMLParent.hasAttributes()) {
&nbsp;&nbsp;&nbsp;&nbsp;vResult = objectify(vBuiltVal);
&nbsp;&nbsp;&nbsp;&nbsp;for (nLength; nLength &lt; oXMLParent.attributes.length; nLength++) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;oAttrib = oXMLParent.attributes.item(nLength);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;vResult["@" + oAttrib.name.toLowerCase()] = parseText(oAttrib.value.trim());
&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;} else if (nLevelEnd &gt; nLevelStart) { vResult = objectify(vBuiltVal); }

&nbsp;&nbsp;for (var nElId = nLevelStart; nElId &lt; nLevelEnd; nElId++) {
&nbsp;&nbsp;&nbsp;&nbsp;sProp = aTmpEls[nElId].nodeName.toLowerCase();
&nbsp;&nbsp;&nbsp;&nbsp;vContent = getJXONTree(aTmpEls[nElId]);
&nbsp;&nbsp;&nbsp;&nbsp;if (vResult.hasOwnProperty(sProp)) {
&nbsp;&nbsp;&nbsp;&nbsp;if (vResult[sProp].constructor !== Array) { vResult[sProp] = [vResult[sProp]]; }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;vResult[sProp].push(vContent);
&nbsp;&nbsp;&nbsp;&nbsp;} else { vResult[sProp] = vContent; nLength++; }
&nbsp;&nbsp;}

&nbsp;&nbsp;aTmpEls.length = nLevelStart;

&nbsp;&nbsp;if (nLength === 0) { vResult = sCollectedTxt ? vBuiltVal : /* put here the default value for empty nodes: */ true; }
&nbsp;&nbsp;/* else { Object.freeze(vResult); } */

&nbsp;&nbsp;return vResult;
}

var myObject = getJXONTree(doc);
alert(myObject.catalog.product.catalog_item[1].size.color_swatch["@image"]); // "black_cardigan.jpg"
alert(myObject.catalog.product.catalog_item[1].size.color_swatch); // "Black" !
</pre>

<div class="note"><strong>Note:</strong> If you want to freeze the whole object tree (because of the "static" nature of an XML document), uncomment the string: <code>/* else { Object.freeze(vResult); } */</code>. The <code><a href="/en/JavaScript/Reference/Global_Objects/Object/freeze" title="en/JavaScript/Reference/Global_Objects/Object/freeze">Object.freeze()</a></code> method prevents new properties from being added to it, prevents existing properties from being removed and prevents existing properties, or their enumerability, configurability, or writability, from being changed. In essence the object tree is made effectively immutable.</div>

<p>This is a possible technique if you know the structure of the XML document.</p>

<h3 id="Reverse_algorithms">Reverse algorithms</h3>

<p>It is possible to reverse the algorithms proposed here in order to build a new XML document starting from a JavaScript Objects Tree. For simplicity, we will propose here a single example, which in a single method represents the inversion of all our algorithms.</p>

<pre class="brush: js">
/*\
|*|
|*|&nbsp; JXON Snippet #5 - Mozilla Developer Network
|*|
|*|&nbsp; https://developer.mozilla.org/en-US/docs/JXON
|*|&nbsp; https://developer.mozilla.org/User:fusionchess
|*|
|*|&nbsp; This framework is released under the GNU Public License, version 3 or later.
|*|&nbsp; http://www.gnu.org/licenses/gpl-3.0-standalone.html
|*|
\*/

function createXML (oObjTree) {
&nbsp;&nbsp;function loadObjTree (oParentEl, oParentObj) {
&nbsp;&nbsp;&nbsp;&nbsp;var vValue, oChild;
&nbsp;&nbsp;&nbsp; if (oParentObj.constructor === String || oParentObj.constructor === Number || oParentObj.constructor === Boolean) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; oParentEl.appendChild(oNewDoc.createTextNode(oParentObj.toString())); /* verbosity level is 0 or 1 */
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (oParentObj === oParentObj.valueOf()) { return; }
&nbsp;&nbsp;&nbsp; } else if (oParentObj.constructor === Date) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;oParentEl.appendChild(oNewDoc.createTextNode(oParentObj.toGMTString()));&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;for (var sName in oParentObj) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if (isFinite(sName)) { continue; } /* verbosity level is 0 */
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;vValue = oParentObj[sName];
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if (sName === "keyValue") {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if (vValue !== null &amp;&amp; vValue !== true) { oParentEl.appendChild(oNewDoc.createTextNode(vValue.constructor === Date ? vValue.toGMTString() : String(vValue))); }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;} else if (sName === "keyAttributes") { /* verbosity level is 3 */
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for (var sAttrib in vValue) { oParentEl.setAttribute(sAttrib, vValue[sAttrib]); }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;} else if (sName.charAt(0) === "@") {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;oParentEl.setAttribute(sName.slice(1), vValue);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;} else if (vValue.constructor === Array) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for (var nItem = 0; nItem &lt; vValue.length; nItem++) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;oChild = oNewDoc.createElement(sName);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;loadObjTree(oChild, vValue[nItem]);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;oParentEl.appendChild(oChild);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;} else {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;oChild = oNewDoc.createElement(sName);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if (vValue instanceof Object) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;loadObjTree(oChild, vValue);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;} else if (vValue !== null &amp;&amp; vValue !== true) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;oChild.appendChild(oNewDoc.createTextNode(vValue.toString()));
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;oParentEl.appendChild(oChild);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;&nbsp;&nbsp;}
&nbsp;&nbsp;}
&nbsp;&nbsp;const oNewDoc = document.implementation.createDocument("", "", null);
&nbsp;&nbsp;loadObjTree(oNewDoc, oObjTree);
&nbsp;&nbsp;return oNewDoc;
}

var newDoc = createXML(myObject);
// we got our Document instance! try: alert((new XMLSerializer()).serializeToString(newDoc));
</pre>

<div class="note"><strong>Note:</strong> With this code the <code>Date</code> instances, if they exist, are converted into <a href="/en/JavaScript/Reference/Global_Objects/String" title="String">Strings</a> through the <a href="/en/JavaScript/Reference/Global_Objects/Date/toGMTString" title="toGMTString"><code>toGMTString()</code></a> method. Nothing prohibits the use of any other conversion method. In addition, all properties of the tree with a <code>true</code> value will be converted into empty elements with no text nodes (see the <a href="#Code_considerations" title="Code considerations">Code considerations</a>).</div>

<p>This is a good solution if you want to automate the creation of an XML document. It is a bad choice, however, if you want to re-build an XML document previously converted into JSON. Although <strong>the bidirectional conversion is very faithful</strong> (except for {{ domxref("CDATASection") }} nodes, which will be converted into {{ domxref("Text") }} nodes), the process is unnecessarily costly. In fact, if your goal is to edit an XML document, it is strongly recommended to work on it rather than create new ones.</p>

<h2 id="The_Parker_Convention">The Parker Convention</h2>

<p>The functions listed above for the conversion of an XML document to <a href="/en/JSON" title="en/JSON">JSON</a> (often called "JXON algorithms") are more or less freely based on the Parker Convention (especially regarding the transformation of <a href="/en/DOM/Node.nodeName" title="en/DOM/Node.nodeName">tags names</a> into <a href="/en/JavaScript/Guide/Working_with_Objects#Objects_and_properties" title="en/Core_JavaScript_1.5_Guide/Working_with_Objects#Objects_and_properties">object properties names</a>, the recognition of the <a href="/en/JavaScript/Reference/Operators/typeof" title="en/JavaScript/Reference/Operators/typeof"><code>typeof</code></a> of all the collected <a href="/en/DOM/Node.nodeValue" title="en/DOM/Node.nodeValue"><code>text content</code></a> of each tag and the absorption of solitary <code>Text</code> and/or <code>CDATASection</code> nodes into primitive values). It is called “Parker Convention” in opposition to “BadgerFish Convention”, after the comic Parker &amp; Badger by Cuadrado. See also: <a href="http://badgerfish.ning.com/" title="BadgerFish convention">BadgerFish Convention</a>.</p>

<p>The following is a transcription of the Parker Convention paper (version 0.4), from the page “<a href="http://code.google.com/p/xml2json-xslt/wiki/TransformingRules" title="TransformingRules – xml2json-xslt">TransformingRules</a>” of the <a href="http://code.google.com/p/xml2json-xslt/" title="xml2json-xslt project">xml2json-xslt project</a> site.</p>

<p>This Convention was written in order to regulate the conversion to <a href="/en/JSON" title="en/JSON">JSON</a> from <a href="/en/XSLT" title="en/XSLT">XSLT</a>, so parts of it are futile for JavaScript.</p>

<div class="note"><strong>Note:</strong> On October 29th, 2013, the World Wide Web Consortium relased <a href="http://www.w3.org/TR/microdata/#json" title="Converting HTML to other formats: JSON – World Wide Web Consortium">in a note</a> on <em>official</em> algorithm for converting <em><a href="/en-US/docs/Web/HTML/Global_attributes#itemid">HTML5 microdata</a></em> to <em><a href="/en/JSON" title="en/JSON">JSON</a></em>. However, <em>HTML microdata</em> <strong>is not</strong> <em>HTML:</em> microdata is a formatted <strong>subset</strong> of HTML.</div>

<h3 id="Translation_JSON">Translation JSON</h3>

<ol>
 <li>
  <p>The root element will be absorbed, for there is only one:</p>

  <pre class="brush: xml">
&lt;root&gt;test&lt;/root&gt;</pre>

  <p>becomes</p>

  <pre class="brush: js">
"test"
</pre>
 </li>
 <li>
  <p>Element names become object properties:</p>

  <pre class="brush: xml">
&lt;root&gt;&lt;name&gt;Xml&lt;/name&gt;&lt;encoding&gt;ASCII&lt;/encoding&gt;&lt;/root&gt;</pre>

  <p>becomes</p>

  <pre class="brush: js">
{
  "name": "Xml",
  "encoding": "ASCII"
}
</pre>
 </li>
 <li>
  <p>Numbers are recognized (integers and decimals):</p>

  <pre class="brush: xml">
&lt;root&gt;&lt;age&gt;12&lt;/age&gt;&lt;height&gt;1.73&lt;/height&gt;&lt;/root&gt;</pre>

  <p>becomes</p>

  <pre class="brush: js">
{
  "age": 12,
  "height": 1.73
}
</pre>
 </li>
 <li>
  <p>Booleans are recognized case insensitive:</p>

  <pre class="brush: xml">
&lt;root&gt;&lt;checked&gt;True&lt;/checked&gt;&lt;answer&gt;FALSE&lt;/answer&gt;&lt;/root&gt;</pre>

  <p>becomes</p>

  <pre class="brush: js">
{
  "checked": true,
  "answer": false
}
</pre>
 </li>
 <li>
  <p>Strings are escaped:</p>

  <pre class="brush: xml">
&lt;root&gt;Quote: &amp;quot; New-line:
&lt;/root&gt;
</pre>

  <p>becomes</p>

  <pre class="brush: js">
"Quote: \" New-line:\n"</pre>
 </li>
 <li>
  <p>Empty elements will become null:</p>

  <pre class="brush: xml">
&lt;root&gt;&lt;nil/&gt;&lt;empty&gt;&lt;/empty&gt;&lt;/root&gt;</pre>

  <p>becomes</p>

  <pre class="brush: js">
{
  "nil": null,
  "empty": null
}
</pre>
 </li>
 <li>
  <p>If all sibling elements have the same name, they become an array</p>

  <pre class="brush: xml">
&lt;root&gt;&lt;item&gt;1&lt;/item&gt;&lt;item&gt;2&lt;/item&gt;&lt;item&gt;three&lt;/item&gt;&lt;/root&gt;
</pre>

  <p>becomes</p>

  <pre class="brush: js">
[1, 2, "three"]
</pre>
 </li>
 <li>
  <p>Mixed mode text-nodes, comments and attributes get absorbed:</p>

  <pre class="brush: xml">
&lt;root version="1.0"&gt;testing&lt;!--comment--&gt;&lt;element test="true"&gt;1&lt;/element&gt;&lt;/root&gt;
</pre>

  <p>becomes</p>

  <pre class="brush: js">
{ "element": true }
</pre>
 </li>
 <li>
  <p>Namespaces get absorbed, and prefixes will just be part of the property name:</p>

  <pre class="brush: xml">
&lt;root xmlns:ding="http://zanstra.com/ding"&gt;&lt;ding:dong&gt;binnen&lt;/ding:dong&gt;&lt;/root&gt;
</pre>

  <p>becomes</p>

  <pre class="brush: js">
{ "ding:dong" : "binnen" }
</pre>
 </li>
</ol>

<div class="note"><strong>Note:</strong> Our algorithms comply with points 2, 3, 4 and 7. The third and the fourth algorithm comply also with point 6 (but <code>true</code> instead of <code>null</code> – see the <a href="#Code_considerations" title="Code considerations">Code considerations</a>). Point 5 is automatically managed by the JavaScript method <code><a href="/en/JavaScript/Reference/Global_Objects/JSON/stringify" title="en/JavaScript/Reference/Global_Objects/JSON/stringify">JSON.stringify()</a></code>. Regarding point 9, we chose to ignore all nodes which have a prefix; you can include them by removing the string <code>&amp;&amp; !oNode.prefix</code> from our algorithms (see the <a href="#Code_considerations" title="Code considerations">Code considerations</a>).</div>

<h3 id="Extra_JavaScript_translations">Extra JavaScript translations</h3>

<p>This is the same as the JSON translation, but with these extras:</p>

<ol>
 <li>
  <p>Property names are only escaped when necessary</p>

  <pre class="brush: xml">
&lt;root&gt;&lt;while&gt;true&lt;/while&gt;&lt;wend&gt;false&lt;/wend&gt;&lt;only-if/&gt;&lt;/root&gt;
</pre>

  <p>becomes</p>

  <pre class="brush: js">
{
  "while": true,
  wend: false,
  "only-if": null
}
</pre>
 </li>
 <li>
  <p>Within a string, closing elements "&lt;/" are escaped as "&lt;\/"</p>

  <pre class="brush: xml">
&lt;root&gt;&lt;![CDATA[&lt;script&gt;alert("YES");&lt;/script&gt;]]&gt;&lt;/root&gt;</pre>

  <p>becomes</p>

  <pre class="brush: js">
{ script: "&lt;script&gt;alert(\"YES\")&lt;\/script&gt;" }
</pre>
 </li>
 <li>
  <p>Dates are created as new <a href="/en/JavaScript/Reference/Global_Objects/Date" title="Date"><code>Date</code></a> objects</p>

  <pre class="brush: xml">
&lt;root&gt;2006-12-25&lt;/root&gt;</pre>

  <p>becomes</p>

  <pre class="brush: js">
new Date(2006, 12 - 1, 25)
</pre>
 </li>
 <li>
  <p>Attributes and comments are shown as comments (for testing purposes):</p>

  <pre class="brush: xml">
&lt;!--testing--&gt;&lt;root&gt;&lt;test version="1.0"&gt;123&lt;/test&gt;&lt;/root&gt;
</pre>

  <p>becomes</p>

  <pre class="brush: js">
/* testing */ { test /* @version = "1.0" */ : 123}
</pre>
 </li>
 <li>
  <p>A bit of indentation is done, to keep things legible</p>
 </li>
</ol>

<div class="note"><strong>Note:</strong> Our algorithms comply with the point 3 (but without month decrease). The points 1 and 2 are automatically managed by the JavaScript method <code><a href="/en/JavaScript/Reference/Global_Objects/JSON/stringify" title="en/JavaScript/Reference/Global_Objects/JSON/stringify">JSON.stringify()</a></code>.</div>

<h2 id="In_summary">In summary</h2>

<p>Let's take <strong><a href="#Algorithm_.233.3A_a_synthetic_technique" title="Go to JXON algorithm #3">the third algorithm</a> as the most representative JXON parsing algorithm</strong>. A single structured XML <code>Element</code> might have <em>eight different configurations</em>:</p>

<ol>
 <li>an empty element,</li>
 <li>an element with pure text content,</li>
 <li>an empty element with attributes,</li>
 <li>an element with text content and attributes,</li>
 <li>an element containing elements with different names,</li>
 <li>an element containing elements with identical names,</li>
 <li>an element containing elements and contiguous text,</li>
 <li>an element containing elements and non contiguous text.</li>
</ol>

<p>The following table shows the corresponding conversion patterns between XML and JSON according to the <a href="#Algorithm_.233.3A_a_synthetic_technique" title="Go to JXON algorithm #3">third algorithm</a>.</p>

<table>
 <thead>
  <tr>
   <th style="background: #faf9e2; color: #5d5636; text-align: center;"><strong>Case</strong></th>
   <th style="background: #faf9e2; color: #5d5636; text-align: center;"><strong>XML</strong></th>
   <th style="background: #faf9e2; color: #5d5636; text-align: center;"><strong>JSON</strong></th>
   <th style="background: #faf9e2; color: #5d5636; text-align: center;"><strong>Javascript access</strong></th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td style="background: #f6f6f6; color: #000000;">1</td>
   <td style="background: #f6f6f6; color: #000000;"><code>&lt;animal /&gt;</code></td>
   <td style="background: #f6f6f6; color: #000000;"><code>"animal": true</code></td>
   <td style="background: #f6f6f6; color: #000000;"><code>myObject.animal</code></td>
  </tr>
  <tr>
   <td style="background: #e7e5dc; color: #silver;">2</td>
   <td style="background: #e7e5dc; color: #silver;"><code>&lt;animal&gt;Deka&lt;/animal&gt;</code></td>
   <td style="background: #e7e5dc; color: #silver;"><code>"animal": "Deka"</code></td>
   <td style="background: #e7e5dc; color: #silver;"><code>myObject.animal</code></td>
  </tr>
  <tr>
   <td style="background: #f6f6f6; color: #000000;">3</td>
   <td style="background: #f6f6f6; color: #000000;"><code>&lt;animal name="Deka" /&gt;</code></td>
   <td style="background: #f6f6f6; color: #000000;"><code>"animal": {"@name": "Deka"}</code></td>
   <td style="background: #f6f6f6; color: #000000;"><code>myObject.animal["@name"]</code></td>
  </tr>
  <tr>
   <td style="background: #e7e5dc; color: #silver;">4</td>
   <td style="background: #e7e5dc; color: #silver;"><code>&lt;animal name="Deka"&gt;is my cat&lt;/animal&gt;</code></td>
   <td style="background: #e7e5dc; color: #silver;"><code>"animal": { "@name": "Deka", "keyValue": "is my cat" }</code></td>
   <td style="background: #e7e5dc; color: #silver;"><code>myObject.animal["@name"]</code>, <code>myObject.animal.keyValue</code></td>
  </tr>
  <tr>
   <td style="background: #f6f6f6; color: #000000;">5</td>
   <td style="background: #f6f6f6; color: #000000;"><code>&lt;animal&gt; &lt;dog&gt;Charlie&lt;/dog&gt; &lt;cat&gt;Deka&lt;/cat&gt; &lt;/animal&gt;</code></td>
   <td style="background: #f6f6f6; color: #000000;"><code>"animal": { "dog": "Charlie", "cat": "Deka" }</code></td>
   <td style="background: #f6f6f6; color: #000000;"><code>myObject.animal.dog</code>, <code>myObject.animal.cat</code></td>
  </tr>
  <tr>
   <td style="background: #e7e5dc; color: #silver;">6</td>
   <td style="background: #e7e5dc; color: #silver;"><code>&lt;animal&gt; &lt;dog&gt;Charlie&lt;/dog&gt; &lt;dog&gt;Mad Max&lt;/dog&gt; &lt;/animal&gt;</code></td>
   <td style="background: #e7e5dc; color: #silver;"><code>"animal": { "dog": ["Charlie", "Mad Max"] }</code></td>
   <td style="background: #e7e5dc; color: #silver;"><code>myObject.animal.dog[0]</code>, <code>myObject.animal.dog[1]</code></td>
  </tr>
  <tr>
   <td style="background: #f6f6f6; color: #000000;">7</td>
   <td style="background: #f6f6f6; color: #000000;"><code>&lt;animal&gt; in my house &lt;dog&gt;Charlie&lt;/dog&gt; &lt;/animal&gt;</code></td>
   <td style="background: #f6f6f6; color: #000000;"><code>"animal": { "keyValue": "in my house", "dog": "Charlie" }</code></td>
   <td style="background: #f6f6f6; color: #000000;"><code>myObject.animal.keyValue</code>, <code>myObject.animal.dog</code></td>
  </tr>
  <tr>
   <td style="background: #e7e5dc; color: #silver;">8</td>
   <td style="background: #e7e5dc; color: #silver;"><code>&lt;animal&gt; in my ho &lt;dog&gt;Charlie&lt;/dog&gt; use &lt;/animal&gt;</code></td>
   <td style="background: #e7e5dc; color: #silver;"><code>"animal": { "keyValue": "in my house", "dog": "Charlie" }</code></td>
   <td style="background: #e7e5dc; color: #silver;"><code>myObject.animal.keyValue</code>, <code>myObject.animal.dog</code></td>
  </tr>
 </tbody>
</table>

<h2 id="Code_considerations">Code considerations</h2>

<p>In these examples we chose to use a property named <code>keyValue</code> for the text content. The lack of standards for XML to JSON conversion leads developers to choose a variety of property names for the text content of XML {{ domxref("Element") }} nodes that also contain other child nodes. Sometimes a property called <code>$</code> is used. Other times a property called <code>#text</code> is used (however, a name like this isn't a good choice, since the text content of a node can be parsed into a non-string value by our algorithms during the conversion). In the algorithms proposed here, you can easily change this name, depending on your needs.</p>

<p>The choice of using a <code>true</code> value instead of a <code>null</code> value to represent empty nodes is due to the fact that <strong>when in an XML document there is an empty node the reason is often to express a<em> <code>Boolean</code></em></strong>, as in this case:</p>

<pre class="brush: xml">
&lt;car&gt;
  &lt;type&gt;Ferrari&lt;/type&gt;
  &lt;bought /&gt;
&lt;/car&gt;
</pre>

<p>If the value were <code>null</code> it would be more cumbersome to launch a code like this:</p>

<pre class="brush: js">
if (myObject.car.bought) {
  // do something
}
</pre>

<div class="note"><strong>Note:</strong> According to our <a href="#Algorithm_.233.3A_a_synthetic_technique" title="Go to JXON algorithm #3">third algorithm</a> and our <a href="#Algorithm_.234.3A_a_very_minimalist_way" title="Go to JXON algorithm #4">fourth algorithm</a>, just <code>CDATASection</code> nodes which contain nothing but white spaces (precisely: <code>/^\s+$/</code>) will be parsed as <code>null</code>.</div>

<p>The <a href="#Algorithm_.234.3A_a_very_minimalist_way" title="Go to JXON algorithm #4">fourth algorithm</a> represents a <strong>special case of conversion</strong>. As you can see, <strong>the generated JavaScript Object tree is not <a href="/en/JavaScript/Reference/Global_Objects/JSON/stringify" title="en/JavaScript/Reference/Global_Objects/JSON/stringify">stringifyable</a></strong>. It is very practical for internal JavaScript access, but don't use it if you want to transfer the tree via JSON string (as for <code><a href="/en/DOM/Worker" title="en/DOM/Worker">Worker</a></code> messages, for example).</p>

<p>We chose to <strong>ignore nodes which have a prefix</strong> (for example: <code>&lt;ding:dong&gt;binnen&lt;/ding:dong&gt;</code>), due to their special case (they are often used in order to represents an <a href="http://www.w3.org/TR/xmlschema-ref/" title="W3C XML Schema Definition Language (XSD): Component Designators">XML Schema</a>, which is <em>meta-information</em> concerning how to organize the <em>information</em> of the document, reserved for the XML parser). You can include them removing the string <code>&amp;&amp; !oNode.prefix</code> from our algorithms (by doing so the whole tag will become the property name: <code>{ "ding:dong": "binnen" }</code>).</p>

<p>An important consideration is that, when using the&nbsp;<a href="#Algorithm_.233.3A_a_synthetic_technique" title="Go to JXON algorithm #3">third</a> or the <a href="#Algorithm_.234.3A_a_very_minimalist_way" title="Go to JXON algorithm #4">fourth</a> algorithm, an XML {{ domxref("Document") }} can be used to create any type of JavaScript object. For example, If you want to create an object like the following:</p>

<pre class="brush: js">
{
&nbsp;&nbsp;"myboolean": true,
&nbsp;&nbsp;"myarray": ["Cinema", "Hot dogs", false],
&nbsp;&nbsp;"myobject": {
&nbsp;&nbsp;&nbsp;&nbsp;"nickname": "Jack",
&nbsp;&nbsp;&nbsp;&nbsp;"registration_date": new Date(1995, 11, 25),
&nbsp;&nbsp;&nbsp;&nbsp;"privileged_user": true
&nbsp;&nbsp;},
&nbsp;&nbsp;"mynumber": 99,
&nbsp;&nbsp;"mytext": "Hello World!"
}
</pre>

<p>you must just create an XML document with the following structure:</p>

<pre class="brush: xml">
&lt;myboolean&gt;true&lt;/myboolean&gt;
&lt;myarray&gt;Cinema&lt;/myarray&gt;
&lt;myarray&gt;Hot dogs&lt;/myarray&gt;
&lt;myarray&gt;false&lt;/myarray&gt;
&lt;myobject&gt;
&nbsp;&nbsp;&lt;nickname&gt;Jack&lt;/nickname&gt;
&nbsp;&nbsp;&lt;registration_date&gt;Dec 25, 1995&lt;/registration_date&gt;
&nbsp;&nbsp;&lt;privileged_user /&gt;
&lt;/myobject&gt;
&lt;mynumber&gt;99&lt;/mynumber&gt;
&lt;mytext&gt;Hello World!&lt;/mytext&gt;
</pre>

<p>This example also shows how the ideal JXON document is an XML document designed specifically to be converted in JSON format, though <em>our algorithms work fine with any kind of XML document</em>.</p>

<div class="note" id="ordering-lossless-note"><strong>Note:</strong> Despite the term JXON suggesting "lossless" conversions, these techniques are not actually lossless if one needs to preserve <strong>ordering of elements</strong>, as is common with many XML dialects (including of course <a href="/en-US/docs/XHTML" title="/en-US/docs/XHTML">XHTML</a>). The ECMAScript standard (JavaScript) indicates that object iteration order is <em>implementation dependent</em>.</div>

<h2 id="Appendix_a_complete_bidirectional_JXON_library">Appendix: a complete, bidirectional, JXON library</h2>

<p>Now we can create a more complete, bidirectional, JXON library based on <strong>all</strong> our algorithms (see: <a href="#Algorithm_.231.3A_a_verbose_way" title="Go to JXON algorithm #1">#1</a>, <a href="#Algorithm_.232.3A_a_less_verbose_way" title="Go to JXON algorithm #2">#2</a>, <a href="#Algorithm_.233.3A_a_synthetic_technique" title="Go to JXON algorithm #3">#3</a>, <a href="#Algorithm_.234.3A_a_very_minimalist_way" title="Go to JXON algorithm #4">#4</a>, <a href="#Reverse_algorithms" title="Reverse algorithms">reverse</a>). Its usage is modeled on the <a href="/en/JavaScript/Reference/Global_Objects/JSON" title="en/JavaScript/Reference/Global_Objects/JSON"><code>JSON</code></a> native object. <strong>Before implementing it in a working environment, please read the <a href="#const_compatibility" title="#const_compatibility">note about the <code>const</code> statement compatibility</a></strong>. The following code is also <a class="external external-icon" href="https://github.com/madmurphy/jxon.js">available on GitHub</a>.</p>

<pre class="brush: js">
"use strict";

/*\
|*|
|*|&nbsp; JXON framework - Copyleft 2011 by Mozilla Developer Network
|*|
|*|&nbsp; Revision #3 - October 31th, 2016
|*|
|*|&nbsp; https://developer.mozilla.org/en-US/docs/JXON
|*|&nbsp; https://developer.mozilla.org/User:fusionchess
|*|&nbsp; https://github.com/madmurphy/jxon.js
|*|
|*|&nbsp; This framework is released under the GNU Public License, version 3 or later.
|*|&nbsp; http://www.gnu.org/licenses/gpl-3.0-standalone.html
|*|
\*/

const JXON = new (function () {

&nbsp; function parseText (sValue) {
&nbsp;&nbsp;&nbsp; if (rIsNull.test(sValue)) { return null; }
&nbsp;&nbsp;&nbsp; if (rIsBool.test(sValue)) { return sValue.toLowerCase() === "true"; }
&nbsp;&nbsp;&nbsp; if (isFinite(sValue)) { return parseFloat(sValue); }
&nbsp;&nbsp;&nbsp; if (isFinite(Date.parse(sValue))) { return new Date(sValue); }
&nbsp;&nbsp;&nbsp; return sValue;
&nbsp; }

&nbsp; function EmptyTree () {}

&nbsp; EmptyTree.prototype.toString = function () { return "null"; };

&nbsp; EmptyTree.prototype.valueOf = function () { return null; };

&nbsp; function objectify (vVal) {
&nbsp;&nbsp;&nbsp; return vVal === null ? new EmptyTree() : vVal instanceof Object ? vVal : new vVal.constructor(vVal);
&nbsp; }

&nbsp; function createObjTree (oParentNode, nVerb, bFreeze, bNesteAttr) {

&nbsp;&nbsp;&nbsp; const
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; nLevelStart = aCache.length, bChildren = oParentNode.hasChildNodes(),
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; bAttributes = oParentNode.hasAttributes &amp;&amp; oParentNode.hasAttributes(), bHighVerb = Boolean(nVerb &amp; 2);

&nbsp;&nbsp;&nbsp; var
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; sProp, vContent, nLength = 0, sCollectedTxt = "",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; vResult = bHighVerb ? {} : /* put here the default value for empty nodes: */ true;

&nbsp;&nbsp;&nbsp; if (bChildren) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for (var oNode, nItem = 0; nItem &lt; oParentNode.childNodes.length; nItem++) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; oNode = oParentNode.childNodes.item(nItem);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (oNode.nodeType === 4) { sCollectedTxt += oNode.nodeValue; } /* nodeType is "CDATASection" (4) */
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; else if (oNode.nodeType === 3) { sCollectedTxt += oNode.nodeValue.trim(); } /* nodeType is "Text" (3) */
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; else if (oNode.nodeType === 1 &amp;&amp; !oNode.prefix) { aCache.push(oNode); } /* nodeType is "Element" (1) */
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }
&nbsp;&nbsp;&nbsp; }

&nbsp;&nbsp;&nbsp; const nLevelEnd = aCache.length, vBuiltVal = parseText(sCollectedTxt);

&nbsp;&nbsp;&nbsp; if (!bHighVerb &amp;&amp; (bChildren || bAttributes)) { vResult = nVerb === 0 ? objectify(vBuiltVal) : {}; }

&nbsp;&nbsp;&nbsp; for (var nElId = nLevelStart; nElId &lt; nLevelEnd; nElId++) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; sProp = aCache[nElId].nodeName.toLowerCase();
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; vContent = createObjTree(aCache[nElId], nVerb, bFreeze, bNesteAttr);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (vResult.hasOwnProperty(sProp)) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (vResult[sProp].constructor !== Array) { vResult[sProp] = [vResult[sProp]]; }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; vResult[sProp].push(vContent);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } else {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; vResult[sProp] = vContent;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; nLength++;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }
&nbsp;&nbsp;&nbsp; }

&nbsp;&nbsp;&nbsp; if (bAttributes) {

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; const
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; nAttrLen = oParentNode.attributes.length,
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; sAPrefix = bNesteAttr ? "" : sAttrsPref, oAttrParent = bNesteAttr ? {} : vResult;

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for (var oAttrib, nAttrib = 0; nAttrib &lt; nAttrLen; nLength++, nAttrib++) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; oAttrib = oParentNode.attributes.item(nAttrib);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; oAttrParent[sAPrefix + oAttrib.name.toLowerCase()] = parseText(oAttrib.value.trim());
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (bNesteAttr) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (bFreeze) { Object.freeze(oAttrParent); }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; vResult[sAttrProp] = oAttrParent;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; nLength -= nAttrLen - 1;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }

&nbsp;&nbsp;&nbsp; }

&nbsp;&nbsp;&nbsp; if (nVerb === 3 || (nVerb === 2 || nVerb === 1 &amp;&amp; nLength &gt; 0) &amp;&amp; sCollectedTxt) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; vResult[sValProp] = vBuiltVal;
&nbsp;&nbsp;&nbsp; } else if (!bHighVerb &amp;&amp; nLength === 0 &amp;&amp; sCollectedTxt) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; vResult = vBuiltVal;
&nbsp;&nbsp;&nbsp; }

&nbsp;&nbsp;&nbsp; if (bFreeze &amp;&amp; (bHighVerb || nLength &gt; 0)) { Object.freeze(vResult); }

&nbsp;&nbsp;&nbsp; aCache.length = nLevelStart;

&nbsp;&nbsp;&nbsp; return vResult;

&nbsp; }

&nbsp; function loadObjTree (oXMLDoc, oParentEl, oParentObj) {

&nbsp;&nbsp;&nbsp; var vValue, oChild;

&nbsp;&nbsp;&nbsp; if (oParentObj.constructor === String || oParentObj.constructor === Number || oParentObj.constructor === Boolean) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; oParentEl.appendChild(oXMLDoc.createTextNode(oParentObj.toString())); /* verbosity level is 0 or 1 */
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (oParentObj === oParentObj.valueOf()) { return; }
&nbsp;&nbsp;&nbsp; } else if (oParentObj.constructor === Date) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; oParentEl.appendChild(oXMLDoc.createTextNode(oParentObj.toGMTString()));
&nbsp;&nbsp;&nbsp; }

&nbsp;&nbsp;&nbsp; for (var sName in oParentObj) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; vValue = oParentObj[sName];
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (isFinite(sName) || vValue instanceof Function) { continue; } /* verbosity level is 0 */
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (sName === sValProp) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (vValue !== null &amp;&amp; vValue !== true) { oParentEl.appendChild(oXMLDoc.createTextNode(vValue.constructor === Date ? vValue.toGMTString() : String(vValue))); }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } else if (sName === sAttrProp) { /* verbosity level is 3 */
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for (var sAttrib in vValue) { oParentEl.setAttribute(sAttrib, vValue[sAttrib]); }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } else if (sName.charAt(0) === sAttrsPref) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; oParentEl.setAttribute(sName.slice(1), vValue);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } else if (vValue.constructor === Array) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for (var nItem = 0; nItem &lt; vValue.length; nItem++) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; oChild = oXMLDoc.createElement(sName);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; loadObjTree(oXMLDoc, oChild, vValue[nItem]);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; oParentEl.appendChild(oChild);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } else {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; oChild = oXMLDoc.createElement(sName);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (vValue instanceof Object) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; loadObjTree(oXMLDoc, oChild, vValue);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } else if (vValue !== null &amp;&amp; vValue !== true) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; oChild.appendChild(oXMLDoc.createTextNode(vValue.toString()));
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; oParentEl.appendChild(oChild);
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }
&nbsp;&nbsp;&nbsp; }

&nbsp; }

&nbsp; /* Uncomment the following code if you want to enable the .appendJXON() method for *all* the "element" objects! */

&nbsp; /*

&nbsp; Element.prototype.appendJXON = function (oObjTree) {
&nbsp;&nbsp;&nbsp; loadObjTree(document, this, oObjTree);
&nbsp;&nbsp;&nbsp; return this;
&nbsp; };

&nbsp; */

&nbsp; this.build = function (oXMLParent, nVerbosity /* optional */, bFreeze /* optional */, bNesteAttributes /* optional */) {
&nbsp;&nbsp;&nbsp; const nVerbMask = arguments.length &gt; 1 &amp;&amp; typeof nVerbosity === "number" ? nVerbosity &amp; 3 : /* put here the default verbosity level: */ 1;
&nbsp;&nbsp;&nbsp; return createObjTree(oXMLParent, nVerbMask, bFreeze || false, arguments.length &gt; 3 ? bNesteAttributes : nVerbMask === 3);
&nbsp; };

&nbsp; this.unbuild = function (oObjTree, sNamespaceURI /* optional */, sQualifiedName /* optional */, oDocumentType /* optional */) {
&nbsp;&nbsp;&nbsp; const oNewDoc = document.implementation.createDocument(sNamespaceURI || null, sQualifiedName || "", oDocumentType || null);
&nbsp;&nbsp;&nbsp; loadObjTree(oNewDoc, oNewDoc, oObjTree);
&nbsp;&nbsp;&nbsp; return oNewDoc;
&nbsp; };

&nbsp; const
&nbsp;&nbsp;&nbsp; sValProp = "keyValue", sAttrProp = "keyAttributes", sAttrsPref = "@", /* you can customize these values */
&nbsp;&nbsp;&nbsp; aCache = [], rIsNull = /^\s*$/, rIsBool = /^(?:true|false)$/i;

})();
</pre>

<div class="note" id="const_compatibility"><strong>Note:</strong> The current implementation of <a href="/en/JavaScript/Reference/Statements/const" title="en/JavaScript/Reference/Statements/const"><code>const</code></a> (constant statement) <strong>is not part of ECMAScript 5</strong>. It is supported in Firefox &amp; Chrome (V8) and partially supported in Opera 9+ and Safari. <strong>It is not supported in Internet Explorer 6-9, or in the preview of Internet Explorer 10</strong>. <a href="/en/JavaScript/Reference/Statements/const" title="en/JavaScript/Reference/Statements/const"><code>const</code></a> is going to be defined by ECMAScript 6, but with different semantics. Similar to variables declared with the <a href="/en/JavaScript/Reference/Statements/let" title="en/JavaScript/Reference/Statements/let"><code>let</code></a> statement, constants declared with <a href="/en/JavaScript/Reference/Statements/const" title="en/JavaScript/Reference/Statements/const"><code>const</code></a> will be block-scoped. <strong>We used it only for didactic purpose. If you want a full browser compatibility of this library, please replace all the <a href="/en/JavaScript/Reference/Statements/const" title="en/JavaScript/Reference/Statements/const"><code>const</code></a> statements with the <a href="/en/JavaScript/Reference/Statements/var" title="en/JavaScript/Reference/Statements/var"><code>var</code></a> statements.</strong></div>

<h3 id="Usage">Usage</h3>

<p>The obtained non-native <code>JXON</code> global object will have two methods:</p>

<table class="fullwidth-table">
 <tbody>
  <tr>
   <th>Method</th>
   <th>Description</th>
  </tr>
  <tr>
   <td><a href="#JXON.build_syntax" title="JXON.build"><code>JXON.build(<em>document</em>[, <em>verbosity</em>[, <em>freeze</em>[, <em>nesteAttributes</em>]]])</code></a></td>
   <td>Returns a JavaScript <a href="/en/JavaScript/Reference/Global_Objects/Object" title="en/JavaScript/Reference/Global_Objects/Object"><code>Object</code></a> based on the given XML Document.</td>
  </tr>
  <tr>
   <td><a href="#JXON.unbuild_syntax" title="JXON.unbuild"><code>JXON.unbuild(<em>objTree</em>[, <em>namespaceURI</em>[, <em>qualifiedNameStr</em>[, <em>documentType</em>]]])</code></a></td>
   <td>Returns an XML {{ domxref("Document") }} based on the given JavaScript <a href="/en/JavaScript/Reference/Global_Objects/Object" title="en/JavaScript/Reference/Global_Objects/Object"><code>Object</code></a>.</td>
  </tr>
 </tbody>
</table>

<p>These methods are inverses of each other. So, you can work with the <code>JXON</code> object by inserting the previous code at the beginning of your scripts. If you are not interested in a bidirectional conversion, don't use it, use only one of our algotithm instead.</p>

<p>Sample usage:</p>

<pre class="brush: js">
var myObject = JXON.build(doc);
// we got our javascript object! try: alert(JSON.stringify(myObject));

var newDoc = JXON.unbuild(myObject);
// we got our Document instance! try: alert((new XMLSerializer()).serializeToString(newDoc));</pre>

<p>…the same thing using AJAX:</p>

<pre class="brush: js">
function reqListener () {

&nbsp;&nbsp; &nbsp;var myObject = JXON.build(this.responseXML);
&nbsp;&nbsp; &nbsp;// we got our javascript object!
&nbsp;&nbsp; &nbsp;alert(JSON.stringify(myObject));

&nbsp;&nbsp; &nbsp;var newDoc = JXON.unbuild(myObject);
&nbsp;&nbsp; &nbsp;// we got our Document instance!
&nbsp;&nbsp; &nbsp;alert((new XMLSerializer()).serializeToString(newDoc));

};
&nbsp;
var oReq = new XMLHttpRequest();
oReq.onload = reqListener;
oReq.open("get", "example.xml", true);
oReq.send();</pre>

<h4 id="JXON.build_syntax">JXON.build syntax</h4>

<p><code>JXON.build(<a href="#JXON_build-document" title="JXON.build – @document"><em>document</em></a>[, <a href="#JXON_build-verbosity" title="JXON.build – @verbosity"><em>verbosity</em></a>[, <a href="#JXON_build-freeze" title="JXON.build – @freeze"><em>freeze</em></a>[, <a href="#JXON_build-nesteAttributes" title="JXON.build – @nesteAttributes"><em>nesteAttributes</em></a>]]])</code></p>

<h4 id="JXON.build_description">JXON.build description</h4>

<p>Returns a JavaScript <a href="/en/JavaScript/Reference/Global_Objects/Object" title="en/JavaScript/Reference/Global_Objects/Object"><code>Object</code></a> based on the given XML Document.</p>

<h4 id="JXON.build_parameters">JXON.build parameters</h4>

<dl>
 <dt><code id="JXON_build-document">document</code></dt>
 <dd>The XML document to be converted into JSON format.</dd>
 <dt><code id="JXON_build-verbosity">verbosity</code> <span class="inlineIndicator optional optionalInline">Optional</span></dt>
 <dd>The verbosity level of conversion (optional), from <code>0</code> to <code>3</code>. It is almost equivalent to our algorithms from <a href="#Algorithm_.234.3A_a_very_minimalist_way" title="Go to JXON algorithm #4">#4</a> to <a href="#Algorithm_.231.3A_a_verbose_way" title="Go to JXON algorithm #1">#1</a> (default value is <code>1</code>, which is equivalent to the <a href="#Algorithm_.233.3A_a_synthetic_technique" title="Go to JXON algorithm #3">algorithm #3</a>).</dd>
 <dt><code id="JXON_build-freeze">freeze</code> <span class="inlineIndicator optional optionalInline">Optional</span></dt>
 <dd>A boolean (optional) expressing whether the created object must be <a href="/en/JavaScript/Reference/Global_Objects/Object/freeze" title="en/JavaScript/Reference/Global_Objects/Object/freeze">freezed</a> or not (default value is <code>false</code>).</dd>
 <dt><code id="JXON_build-nesteAttributes">nesteAttributes</code> <span class="inlineIndicator optional optionalInline">Optional</span></dt>
 <dd>A boolean (optional) expressing whether the the <code>nodeAttributes</code> must be nested into a child-object named <code>keyAttributes</code> or not (default value is <code>false</code> for verbosity levels from <code>0</code> to <code>2</code>; <code>true</code> for verbosity level <code>3</code>).</dd>
</dl>

<h4 id="JXON.unbuild_syntax">JXON.unbuild syntax</h4>

<p><code>JXON.unbuild(<a href="#JXON_unbuild-objTree" title="JXON.unbuild – @objTree"><em>objTree</em></a>[, <a href="#JXON_unbuild-namespaceURI" title="JXON.unbuild – @namespaceURI"><em>namespaceURI</em></a>[, <a href="#JXON_unbuild-qualifiedNameStr" title="JXON.unbuild – @qualifiedNameStr"><em>qualifiedNameStr</em></a>[, <a href="#JXON_unbuild-documentType" title="JXON.unbuild – @objTree"><em>documentType</em></a>]]])</code></p>

<h4 id="JXON.unbuild_description">JXON.unbuild description</h4>

<p>Returns an XML Document based on the given JavaScript <a href="/en/JavaScript/Reference/Global_Objects/Object" title="en/JavaScript/Reference/Global_Objects/Object"><code>Object</code></a>.</p>

<h4 id="JXON.unbuild_parameters">JXON.unbuild parameters</h4>

<dl>
 <dt><code id="JXON_unbuild-objTree">objTree</code></dt>
 <dd>The JavaScript Object from which you want to create your XML Document.</dd>
 <dt><code id="JXON_unbuild-namespaceURI">namespaceURI</code> <span class="inlineIndicator optional optionalInline">Optional</span></dt>
 <dd>Is a <a href="https://developer.mozilla.org/en-US/docs/Web/API/DOMString" title="A UTF-16 String. As JavaScript already uses such strings, DOMString is mapped directly to a String."><code>DOMString</code></a> containing the namespace URI&nbsp;of the document to be created, or <code>null</code> if the document doesn't belong to one.</dd>
 <dt><code id="JXON_unbuild-qualifiedNameStr">qualifiedNameStr</code> <span class="inlineIndicator optional optionalInline">Optional</span></dt>
 <dd>Is a <a href="https://developer.mozilla.org/en-US/docs/Web/API/DOMString" title="A UTF-16 String. As JavaScript already uses such strings, DOMString is mapped directly to a String."><code>DOMString</code></a> containing the qualified name, that is an optional prefix and colon plus the local root element name, of the document to be created.</dd>
 <dt><code id="JXON_unbuild-documentType">documentType</code> <span class="inlineIndicator optional optionalInline">Optional</span></dt>
 <dd>Is the <a class="internal" href="https://developer.mozilla.org/En/DOM/DocumentType" title="En/DOM/DocumentType"><code>DocumentType</code></a> of the document to be created. It defaults to <code>null</code>.</dd>
</dl>

<h3 id="Extend_the_native_Element.prototype_object">Extend the native <code><a href="/en-US/docs/Web/API/element" title="/en-US/docs/Web/API/element">Element</a>.prototype</code> object</h3>

<p>If you want to enable the <code>.appendJXON()</code> method for all the native <a href="/en-US/docs/Web/API/element"><code>element</code></a> objects, you can uncomment the following code from the JXON library:</p>

<pre class="brush: js">
&nbsp; /* Uncomment the following code if you want to enable the .appendJXON() method for *all* the "element" objects! */

&nbsp; /*

&nbsp; Element.prototype.appendJXON = function (oObjTree) {
&nbsp;&nbsp;&nbsp; loadObjTree(document, this, oObjTree);
&nbsp;&nbsp;&nbsp; return this;
&nbsp; };

&nbsp; */</pre>

<h4 id="Example">Example</h4>

<p>Imagine you want to populate the following <a href="/en-US/docs/Web/API/HTMLElement"><code>HTMLElement</code></a> through JSON:</p>

<pre class="brush: html">
&lt;div id="form_container"&gt;&lt;/div&gt;</pre>

<p>Then, the following code:</p>

<pre class="brush: js">
document.getElementById("form_container").appendJXON({
&nbsp; "form": {
&nbsp;&nbsp;&nbsp; "script": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@type": "text/javascript",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "keyValue": "\n&nbsp; function numbersOnly (oToCheckField, oKeyEvent) {\n&nbsp; return oKeyEvent.charCode === 0 || /\\d/.test(String.fromCharCode(oKeyEvent.charCode));\n&nbsp; }\n"
&nbsp;&nbsp;&nbsp; },
&nbsp;&nbsp;&nbsp; "input": [{
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@type": "hidden",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@name": "instId",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@value": 1234
&nbsp;&nbsp;&nbsp; }, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@type": "hidden",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@name": "currency",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@value": "GBP"
&nbsp;&nbsp;&nbsp; }, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@type": "hidden",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@name": "amount",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@value": 0
&nbsp;&nbsp;&nbsp; }, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@type": "hidden",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@name": "name",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@value": "CAPTURED"
&nbsp;&nbsp;&nbsp; }],
&nbsp;&nbsp;&nbsp; "table": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "tr": [{
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "th": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@style": "text-align: right;",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "keyValue": "Product:"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; },
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "td": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "span": [{
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "input": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@type": "radio",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@name": "nome",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@id": "rel_tshirt",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@value": "tshirt"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; },
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "label": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@for": "rel_tshirt",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "keyValue": "T-Shirt"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; },
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@class": "product"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "input": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@type": "radio",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@name": "nome",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@id": "rel_trousers",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@value": "trousers"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; },
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "label": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@for": "rel_trousers",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "keyValue": "Trousers"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; },
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@class": "product"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "input": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@type": "radio",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@name": "nome",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@id": "rel_pullover",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@value": "pullover"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; },
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "label": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@for": "rel_pullover",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "keyValue": "Pullover"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; },
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@class": "product"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }, {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "th": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@style": "text-align: right;",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "keyValue": "Quantity:"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; },
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "td": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "input": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@type": "text",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@name": "myInput",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@onkeypress": "return numbersOnly(this, event);",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@onpaste": "return false;"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }]
&nbsp;&nbsp;&nbsp; },
&nbsp;&nbsp;&nbsp; "p": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "input": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@type": "submit",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@value": "Purchase!"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }
&nbsp;&nbsp;&nbsp; },
&nbsp;&nbsp;&nbsp; "@action": "https://secure-test.worldpay.com/wcc/purchase",
&nbsp;&nbsp;&nbsp; "@name": "BuyForm",
&nbsp;&nbsp;&nbsp; "@method": "POST"
&nbsp; }
});</pre>

<p>will populate the previous element in the following way:</p>

<pre class="brush: html">
&lt;div id="form_container"&gt;
&nbsp; &lt;form action="https://secure-test.worldpay.com/wcc/purchase" name="BuyForm" method="POST"&gt;
&nbsp;&nbsp;&nbsp; &lt;script type="text/javascript"&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; function numbersOnly(oToCheckField, oKeyEvent) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return oKeyEvent.charCode === 0 || /\d/.test(String.fromCharCode(oKeyEvent.charCode));
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }
&nbsp;&nbsp;&nbsp; &lt;/script&gt;
&nbsp;&nbsp;&nbsp; &lt;input type="hidden" name="instId" value="1234" /&gt;
&nbsp;&nbsp;&nbsp; &lt;input type="hidden" name="currency" value="GBP" /&gt;
&nbsp;&nbsp;&nbsp; &lt;input type="hidden" name="amount" value="0" /&gt;
&nbsp;&nbsp;&nbsp; &lt;input type="hidden" name="name" value="CAPTURED" /&gt;
&nbsp;&nbsp;&nbsp; &lt;table&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &lt;tr&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &lt;th style="text-align: right;"&gt;Product:&lt;/th&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &lt;td&gt;&lt;span class="product"&gt;&lt;input type="radio" name="nome" id="rel_tshirt" value="tshirt"/&gt;&lt;label for="rel_tshirt"&gt;T-Shirt&lt;/label&gt;&lt;/span&gt;&lt;span class="product"&gt;&lt;input type="radio" name="nome" id="rel_trousers" value="trousers"/&gt;&lt;label for="rel_trousers"&gt;Trousers&lt;/label&gt;&lt;/span&gt;&lt;span class="product"&gt;&lt;input type="radio" name="nome" id="rel_pullover" value="pullover"/&gt;&lt;label for="rel_pullover"&gt;Pullover&lt;/label&gt;&lt;/span&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &lt;/td&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &lt;/tr&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &lt;tr&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &lt;th style="text-align: right;"&gt;Quantity:&lt;/th&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &lt;td&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &lt;input type="text" name="myInput" onkeypress="return numbersOnly(this, event);" onpaste="return false;" /&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &lt;/td&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &lt;/tr&gt;
&nbsp;&nbsp;&nbsp; &lt;/table&gt;
&nbsp;&nbsp;&nbsp; &lt;p&gt;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &lt;input type="submit" value="Purchase!" /&gt;
&nbsp;&nbsp;&nbsp; &lt;/p&gt;
&nbsp; &lt;/form&gt;
&lt;/div&gt;</pre>

<h3 id="Other_examples">Other examples</h3>

<h4 id="Example_1_How_to_use_JXON_to_create_an_HTML_document_instead_of_an_XML_document">Example #1: How to use JXON to create an HTML document instead of an XML document:</h4>

<pre class="brush: js">
/* The structure of my document */
var oMyHTMLStruct = {
&nbsp; "html": {
&nbsp;&nbsp;&nbsp; "head": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "meta": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@http-equiv": "Content-Type",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@content": "text/html; charset=UTF-8"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; },
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "title": "My HTML Document",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "script": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "@type": "text/javascript",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "keyValue": "alert(\"Welcome!\");"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; },
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "style": "p:first-letter {\n&nbsp; font: italic bold 30px Georgia, serif;\n}"
&nbsp;&nbsp;&nbsp; },
&nbsp;&nbsp;&nbsp; "body": {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "h1": "My HTML Document",
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; "p": "Hello world!!"
&nbsp;&nbsp;&nbsp; }
&nbsp; }
};

/* Create the document */
var oMyHTMLDoc = JXON.unbuild(oMyHTMLStruct, "http://www.w3.org/1999/xhtml");</pre>

<p>…And here is the output of <code>alert((new XMLSerializer()).serializeToString(oMyHTMLDoc))</code>:</p>

<pre class="brush: html">
&lt;html&gt;

&lt;head&gt;
&nbsp; &lt;meta http-equiv="Content-Type" content="text/html; charset=UTF-8" /&gt;
&nbsp; &lt;title&gt;My HTML Document&lt;/title&gt;
&nbsp; &lt;script type="text/javascript"&gt;
&nbsp;&nbsp;&nbsp; alert("Welcome!");
&nbsp; &lt;/script&gt;
&nbsp; &lt;style&gt;
&nbsp;&nbsp;&nbsp; p:first-letter {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; font: italic bold 30px Georgia, serif;
&nbsp;&nbsp;&nbsp; }
&nbsp; &lt;/style&gt;
&lt;/head&gt;

&lt;body&gt;
&nbsp; &lt;h1&gt;My HTML Document&lt;/h1&gt;
&nbsp; &lt;p&gt;Hello world!!&lt;/p&gt;
&lt;/body&gt;

&lt;/html&gt;</pre>

<div class="note"><strong>Note:</strong> As we already said in <a href="#ordering-lossless-note">the note within <em>Code considerations</em></a>, despite the bidirectional conversion between XML and JSON <strong>is</strong> lossless regarding the whole content and the structure of an XML document, it <strong>is not</strong> lossless regarding the ordering of elements, which for some XML dialects (like XHTML) is part of the information. For instance, a bidirectional conversion of the following HTML paragraph:

<pre class="brush: html">
&lt;p&gt;She &lt;strong&gt;loves&lt;/strong&gt; you. And definitely &lt;strong&gt;hates&lt;/strong&gt; me.&lt;/p&gt;</pre>
would determine a result like the following:

<pre class="brush: html">
&lt;p&gt;&lt;strong&gt;loves&lt;/strong&gt;&lt;strong&gt;hates&lt;/strong&gt;Sheyou. And definitelyme.&lt;/p&gt;</pre>
As you can see in this special case, the whole information is preserved, the ordering of the elements is not.<br />
It turns out then that for some XML dialects JXON can be not the best choise, while it can be a really powerful tool in dealing with <em>standard XML</em>. One conversion method which is lossless for element order, as it relies on arrays (but, with a less human-readable, JavaScript-friendly syntax), is <a href="http://www.jsonml.org/" title="http://www.jsonml.org/">JsonML</a>.</div>

<h3 id="About_this_library">About this library</h3>

<p>The <code>JXON.build()</code> method summarizes all our four ways of conversion (see: <a href="#Algorithm_.231.3A_a_verbose_way" title="Go to JXON algorithm #1">#1</a>, <a href="#Algorithm_.232.3A_a_less_verbose_way" title="Go to JXON algorithm #2">#2</a>, <a href="#Algorithm_.233.3A_a_synthetic_technique" title="Go to JXON algorithm #3">#3</a>, <a href="#Algorithm_.234.3A_a_very_minimalist_way" title="Go to JXON algorithm #4">#4</a>). The result is therefore the same of our four algorithms, depending on the level of verbosity utilised. As above, optional properties and methods (commented in the example) of the <a href="#Algorithm_.231.3A_a_verbose_way" title="Go to JXON algorithm #1">first algorithm</a> (verbosity level: 3) are not included.</p>

<p>The <code>JXON.unbuild()</code> method utilises our <a href="#Reverse_algorithms" title="Reverse algorithms">reverse algorithm</a>.</p>

<p>Therefore, <strong>all <a href="#Code_considerations" title="Code considerations">code considerations</a> remain the same</strong>.</p>

<h2 id="Resources">Resources</h2>

<ul>
 <li><a href="http://code.google.com/p/xml2json-xslt/wiki/TransformingRules" title="TransformingRules – xml2json-xslt">The Parker Convention</a></li>
 <li><a href="http://badgerfish.ning.com/" title="BadgerFish convention">The BadgerFish Convention</a></li>
 <li><a href="http://www.balisage.net/Proceedings/vol7/html/Lee01/BalisageVol7-Lee01.html" title="JXON: an Architecture for Schema and Annotation Driven JSON/XML Bidirectional Transformations – Balisage: The Markup Conference 2011">JXON: an Architecture for Schema and Annotation Driven JSON/XML Bidirectional Transformations</a></li>
 <li><a href="http://www.w3.org/TR/microdata/#json">Converting HTML to other formats: JSON (The World Wide Web Consortium)</a></li>
 <li><a href="http://dinogambone.com/2012/jxon-a-simple-way-to-keep-xml-out-of-your-life/" title="JXON – A simple way to keep XML out of your life – Dino Gambone's blog">JXON – A simple way to keep XML out of your life – Dino Gambone's blog</a></li>
 <li><a href="http://webreflection.blogspot.it/2008/07/jxon-lossless-javascript-to-xml-object.html" title="Web Reflection: JXON – Lossless JavaScript to XML Object Notation convertion">Web Reflection: JXON – Lossless JavaScript to XML Object Notation convertion</a></li>
 <li><a href="http://davidwalsh.name/convert-xml-json" title="Convert XML to JSON with JavaScript – David Walsh Blog">Convert XML to JSON with JavaScript – David Walsh Blog</a></li>
 <li><a href="http://goessner.net/download/prj/jsonxml/" title="http://goessner.net/download/prj/jsonxml/">http://goessner.net/download/prj/jsonxml/</a> – just another json2xml and xml2json conversion tool</li>
 <li><a href="http://tawani.blogspot.it/2006/12/serialize-javascript-objects-to-xml-for.html" title="Serialize JavaScript objects to XML (for use with Ajax) – Tawani's Blog Rants">Serialize JavaScript objects to XML (for use with Ajax) – Tawani's Blog Rants</a></li>
 <li><a href="http://www.kawa.net/works/js/xml/objtree-e.html" title="XML.ObjTree – XML source code from/to JavaScript object like E4X – Kawa.net">XML.ObjTree – XML source code from/to JavaScript object like E4X – Kawa.net</a></li>
 <li><a href="http://www.jsonml.org/" title="http://www.jsonml.org/">JsonML</a> – a conversion method which is lossless for element order, as it relies on arrays.</li>
</ul>

<h2 id="See_also">See also</h2>

<ul>
 <li><a href="/en/XML" title="en/XML">XML</a></li>
 <li><a href="/en/JSON" title="en/JSON">JSON</a></li>
 <li><a href="/en/XPath" title="en/XPath">XPath</a></li>
 <li><a href="/en/E4X" title="en/E4X">E4X (ECMAScript for XML)</a></li>
 <li><a href="/en/Parsing_and_serializing_XML" title="en/Parsing_and_serializing_XML">Parsing and serializing XML</a></li>
 <li><a href="/en/DOM/XMLHttpRequest" title="en/XMLHttpRequest">XMLHttpRequest</a></li>
 <li><a href="/en/How_to_create_a_DOM_tree" title="en/How_to_create_a_DOM_tree">How to Create a DOM tree</a></li>
 <li><a href="/en/JavaScript/Introduction_to_Object-Oriented_JavaScript" title="Introduction to Object-Oriented JavaScript">Introduction to Object-Oriented JavaScript</a></li>
 <li><a href="/en/JavaScript/Guide/Working_with_Objects" title="Working with Objects">Working with Objects</a></li>
 <li><a href="/en/XML_Introduction" title="en/XML_Introduction">XML Introduction</a></li>
</ul>

