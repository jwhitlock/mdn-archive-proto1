---
version: prototype1
revision_id: 933709
locale: en-US
slug: User:teoli/In_content
tags: 
title: In content
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>This list the widgets that need new styling.</p>

<h2 id="Action-driven_boxes">Action-driven boxes</h2>

<p>These boxes have helped a lot in lowering the bouncing rate and increasing the conversion rate (going to pages with actual content, not landing pages).</p>

<ul class="card-grid">
 <li><span>CSS Reference</span>

  <p>An <a href="/en-US/docs/Web/CSS/Reference" title="en-US/docs/CSS/CSS_Reference">exhaustive reference</a> for <u>seasoned Web developers</u> describing every property and concept of CSS.</p>
 </li>
 <li><span>CSS Tutorial</span>
  <p>A <a href="/en-US/docs/CSS/Getting_Started" title="en-US/docs/CSS/Getting_Started">step-by-step introduction</a> to help <u>complete beginners</u> get started. It presents all the needed fundamentals.</p>
 </li>
 <li><span>CSS3 Demos</span>
  <p>A <a href="/en-US/demos/tag/tech:css3" title="https://developer.mozilla.org/en-US/demos/tag/tech:css3">collection of demos</a> showing the <u>latest CSS technologies</u> in action: a boost for the creativity.</p>
 </li>
</ul>

<p class="Documentation" id="Documentation" name="Documentation">{{bug(924844)}} | <a href="https://developer.mozilla.org/en-US/docs/Web/CSS">In-context usage</a>.</p>

<p class="Documentation" name="Documentation">Another one, slightly different does appear on the FxOS zone landing page (can't cut &amp; paste here as the CSS is not accessible out of the landing pages:</p>

<p class="Documentation" name="Documentation"><a href="https://developer.mozilla.org/en-US/docs/Mozilla/Firefox_OS">Builds Apps for Firefox OS</a></p>

<p class="Documentation" name="Documentation">There's also a similar box at the top of the <a href="/en-US/Apps">App Center</a> that needs some work.</p>

<h2 class="Documentation" id="Documentation" name="Documentation">Two-column landing page text</h2>

<p>On small screen, this get transformed into one single column (via a media query).</p>

<div class="row topicpage-table">
<div class="section">
<h2 class="Documentation" id="Documentation" name="Documentation">Documentation and tutorials</h2>

<dl>
 <dt>CSS key concepts</dt>
 <dd>Describes the <a href="/en-US/docs/CSS/Syntax" title="/en-US/docs/CSS/Syntax">syntax and forms of the language</a> and ...</dd>
 <dt><a href="/en-US/docs/Web/Guide/CSS" title="/en-US/docs/Web/Guide/CSS">CSS developer guide</a></dt>
 <dd>Articles to help you learn CSS techniques to make your content shine.</dd>
</dl>

<h2 class="Tools" id="Tools" name="Tools">Tools for CSS development</h2>

<ul>
 <li><span class="external">The </span><a class="external" href="http://jigsaw.w3.org/css-validator/">W3C CSS Validation Service</a> checks if a given CSS is valid. It is an invaluable debugging tool.</li>
 <li>Firefox' <a class="link-https" href="https://addons.mozilla.org/en-US/firefox/addon/1843">Firebug extension</a><span class="external">, a popular</span> extension of that navigator that allows to edit live CSS on watched sites. Very practical to test some changes, though this extension does much more.</li>
</ul>
</div>

<div class="section">
<h2 class="Related_Topics" id="News" name="News">News</h2>

<ul>
 <li><a href="http://www.w3.org/TR/css-text-decor-3/" title="http://www.w3.org/TR/css-text-decor-3/">CSS Text-decoration Level 3</a> reached the <em>Candidate Recommandation</em> status, defining that the <code>text-decoration-*</code> and <code>text-emphasis-*</code> properties. The long known {{cssxref("text-shadow")}} is also defined in it. (<em>August 1st, 2013)</em></li>
 <li>Gecko's now support {{cssxref("background-origin")}}<code>: local</code>. It will be available from Firefox 25 (and already is in Nightly). <em>(July 25th, 2013)</em></li>
</ul>
</div>
</div>

<p>{{bug(924847)}} | <a href="https://developer.mozilla.org/en-US/docs/Web/CSS">In-context usage</a>.</p>

<h2 id="Specification_boxes">Specification boxes</h2>

<p>These boxes list the specifications where the described feature is defined, this is usually at the end of such a page (we have 1000s of such pages), right before a Browser compatibility section.</p>

<p>The current look and feel doesn't scale to small screen (read: phone screans), the current idea (but to be discussed, amended) is to switch a definition list style section on smaller screens. The idea has not been implemented.</p>

<p>The most complete (unusally long):</p>

<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">Specification</th>
   <th scope="col">Status</th>
   <th scope="col">Comment</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{SpecName('Undo Manager', '', 'Element')}}</td>
   <td>{{Spec2('Undo Manager')}}</td>
   <td>Added the <code>undoScope</code> and <code>undoManager</code> properties.</td>
  </tr>
  <tr>
   <td>{{SpecName('Pointer Events', '#extensions-to-the-element-interface', 'Element')}}</td>
   <td>{{Spec2('Pointer Events')}}</td>
   <td>Added the following event handlers: <code>ongotpointercapture</code> and <code>onlostpointercapture</code>.<br />
    Added the following methods: <code>setPointerCapture()</code> and <code>releasePointerCapture()</code>.</td>
  </tr>
  <tr>
   <td>{{SpecName('Selectors API Level 2', '#interface-definitions', 'Element')}}</td>
   <td>{{Spec2('Selectors API Level 2')}}</td>
   <td>Added the following methods:<code> matches()</code> (implemented as <code>mozMatchesSelector()</code>), <code>find()</code>, <code>findAll()</code>.</td>
  </tr>
  <tr>
   <td>{{SpecName('Selectors API Level 1', '#interface-definitions', 'Element')}}</td>
   <td>{{Spec2('Selectors API Level 1')}}</td>
   <td>Added the following methods: <code>querySelector()</code> and <code>querySelectorAll()</code>.</td>
  </tr>
  <tr>
   <td>{{SpecName('Pointer Lock', 'index.html#element-interface', 'Element')}}</td>
   <td>{{Spec2('Pointer Lock')}}</td>
   <td>Added the <code>requestPointerLock()</code> method.</td>
  </tr>
  <tr>
   <td>{{SpecName('Fullscreen', '#api', 'Element')}}</td>
   <td>{{Spec2('Fullscreen')}}</td>
   <td>Added the <code>requestFullscreen()</code> method.</td>
  </tr>
  <tr>
   <td>{{SpecName('DOM Parsing', '#extensions-to-the-element-interface', 'Element')}}</td>
   <td>{{Spec2('DOM Parsing')}}</td>
   <td>Added the following properties: <code>innerHTML</code>, and <code>outerHTML</code>.<br />
    Added the following method: <code>insertAdjacentHTML()</code>.</td>
  </tr>
  <tr>
   <td>{{SpecName('CSSOM View', '#extensions-to-the-element-interface', 'Element')}}</td>
   <td>{{Spec2('CSSOM View')}}</td>
   <td>Added the following properties: <code>scrollTop</code>, <code>scrollLeft</code>, <code>scrollWidth</code>, <code>scrollHeight</code>, <code>clientTop</code>, <code>clientLeft</code>, <code>clientWidth</code>, and <code>clientHeight</code>.<br />
    Added the following methods: <code>getClientRects()</code>, <code>getBoundingClientRect()</code>, and <code>scrollIntoView()</code>.</td>
  </tr>
  <tr>
   <td>{{SpecName('Element Traversal', '#ecmascript-bindings', 'Element')}}</td>
   <td>{{Spec2('Element Traversal')}}</td>
   <td>Added inheritance of the {{domxref("ElementTraversal")}} interface.</td>
  </tr>
  <tr>
   <td>{{SpecName('DOM WHATWG', '#interface-element', 'Element')}}</td>
   <td>{{Spec2('DOM WHATWG')}}</td>
   <td>Removed the following methods: <code>setIdAttribute()</code>, <code>setIdAttributeNS()</code>, and <code>setIdAttributeNode()</code>.<br />
    Removed the <code>schemaTypeInfo</code> property.</td>
  </tr>
  <tr>
   <td>{{SpecName('DOM3 Core', 'core.html#ID-745549614', 'Element')}}</td>
   <td>{{Spec2('DOM3 Core')}}</td>
   <td>Added the following methods: <code>setIdAttribute()</code>, <code>setIdAttributeNS()</code>, and <code>setIdAttributeNode()</code>. These methods were never implemented and have been removed in later specifications.<br />
    Added the <code>schemaTypeInfo</code> property. This property was never implemented and has been removed in later specifications.</td>
  </tr>
  <tr>
   <td>{{SpecName('DOM2 Core', 'core.html#ID-745549614', 'Element')}}</td>
   <td>{{Spec2('DOM2 Core')}}</td>
   <td>The <code>normalize()</code> method has been moved to {{domxref("Node")}}.</td>
  </tr>
  <tr>
   <td>{{SpecName('DOM1', 'level-one-core.html#ID-745549614', 'Element')}}</td>
   <td>{{Spec2('DOM1')}}</td>
   <td>Initial definition.</td>
  </tr>
 </tbody>
</table>

<p id="Browser_compatibility">A regular one:</p>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="col">Specification</th>
   <th scope="col">Status</th>
   <th scope="col">Comment</th>
  </tr>
  <tr>
   <td>{{SpecName('HTML WHATWG', "grouping-content.html#the-li-element", "HTMLLIElement")}}</td>
   <td>{{Spec2('HTML WHATWG')}}</td>
   <td>No change from {{SpecName("HTML5 W3C")}}.</td>
  </tr>
  <tr>
   <td>{{SpecName('HTML5 W3C', "grouping-content.html#the-li-element", "HTMLLIElement")}}</td>
   <td>{{Spec2('HTML5 W3C')}}</td>
   <td>The following property is now obsolete: <code>type</code>.</td>
  </tr>
  <tr>
   <td>{{SpecName('DOM2 HTML', 'html.html#ID-74680021', 'HTMLLIElement')}}</td>
   <td>{{Spec2('DOM2 HTML')}}</td>
   <td>No change from {{SpecName("DOM1")}}.</td>
  </tr>
  <tr>
   <td>{{SpecName('DOM1', 'level-one-html.html#ID-74680021', 'HTMLLIElement')}}</td>
   <td>{{Spec2('DOM1')}}</td>
   <td>Initial definition.</td>
  </tr>
 </tbody>
</table>

<p>A small one (quite common):</p>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="col">Specification</th>
   <th scope="col">Status</th>
   <th scope="col">Comment</th>
  </tr>
  <tr>
   <td>{{SpecName('Web Audio API', '#OscillatorNode-section', 'OscillatorNode')}}</td>
   <td>{{Spec2('Web Audio API')}}</td>
   <td>&nbsp;</td>
  </tr>
 </tbody>
</table>

<p>{{bug(924875)}} | <a href="https://developer.mozilla.org/en-US/docs/Web/API/Element">In-context usage</a>.</p>

<h2 id="Compatibility_tables">Compatibility tables</h2>

<p>The compatibility tables are at the bottom of most pages, they list which browser support what.</p>

<p>They must stay there, but we dream of a way to present compat info inside the page (as not all methods/properties have the same compatibility levels). To do it without being intrusive (it is a side information, though important in some use cases), is a challenge. [We don't want to take this challenge for the redesign launch, but any idea is welcome].</p>

<p>{{CompatibilityTable}}</p>

<div id="compat-desktop">
<table class="compat-table">
 <tbody>
  <tr>
   <th>Feature</th>
   <th>Chrome</th>
   <th>Firefox (Gecko)</th>
   <th>Internet Explorer</th>
   <th>Opera</th>
   <th>Safari</th>
  </tr>
  <tr>
   <td>Basic support</td>
   <td>8.0 as <code>webkitURL</code></td>
   <td>{{CompatGeckoDesktop("2.0")}} (non-standard name) [1]<br />
    {{CompatGeckoDesktop("19.0")}}</td>
   <td>10.0</td>
   <td>15.0 as <code>webkitURL</code></td>
   <td>6.0 as <code>webkitURL</code></td>
  </tr>
  <tr>
   <td><code>URLUtils</code> properties</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatUnknown}}</td>
  </tr>
  <tr>
   <td><code>username</code>, <code>password</code>, <code>href</code>, and <code>origin</code></td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatGeckoDesktop("26.0")}}</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatUnknown}}</td>
  </tr>
 </tbody>
</table>
</div>

<div id="compat-mobile">
<table class="compat-table">
 <tbody>
  <tr>
   <th>Feature</th>
   <th>Android</th>
   <th>Firefox Mobile (Gecko)</th>
   <th>IE Mobile</th>
   <th>Opera Mobile</th>
   <th>Safari Mobile</th>
  </tr>
  <tr>
   <td>Basic support</td>
   <td>{{CompatVersionUnknown}}as <code>webkitURL</code></td>
   <td>{{CompatGeckoMobile("14.0")}}(non-standard name) [1]<br />
    {{CompatGeckoMobile("19.0")}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>15.0 as <code>webkitURL</code></td>
   <td>6.0 as <code>webkitURL</code></td>
  </tr>
  <tr>
   <td><code>URLUtils</code> properties</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatNo}}</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatUnknown}}</td>
  </tr>
  <tr>
   <td><code>username</code>, <code>password</code>, <code>href</code>, and <code>origin</code></td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatGeckoDesktop("26.0")}}</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatUnknown}}</td>
  </tr>
 </tbody>
</table>
</div>

<p>[1] From Gecko 2 (Firefox 4) to Gecko 18 included, Gecko supported this interface with the non-standard <code>nsIDOMMozURLProperty</code> internal type. As the only to access such an object was through {{domxref("window.URL")}}, in practice, this didn't make any difference.</p>

<p><a href="https://developer.mozilla.org/en-US/docs/Web/API/URL">In context usage</a></p>

<p>&nbsp;</p>

<h2 id="Code_Sample">Code Sample</h2>

<pre class="brush: js">
@charset "utf-8";

/* This is a special template used as a custom CSS for MDN. *//*

    When editing this stylesheet, please be careful of different writing direction pages like: https://developer.mozilla.org/he/docs/HTML

    If you add a custom CSS class, please try one of the following.
        1, Report to the (evil) leader.
        2, Write a description about the class that you have added to -- https://developer.mozilla.org/en-US/docs/Project:Custom_CSS_Classes --

*/
</pre>

<h2 id="Notes">Notes</h2>

<div class="note">
<p><strong>Note:</strong> TextTextTextTextTextText TextTextTextTextTextTextText TextTextTextTextTextTextTextText TextTextTextTextTextTextText TextTextTextTextTextTextText TextTextTextTextText TextTextTextTextText TextTextTextText TextTextTextText TextTextTextTextText TextTextTextTextText TextTextTextTextText</p>
</div>

<p>No bug filed | <a href="https://developer.mozilla.org/en-US/Firefox_OS">In-context usage</a>.</p>

<div class="warning">
<p><strong>Warning:</strong> this is a warning message!</p>
</div>

<h2 id="Summary_boxes">Summary boxes</h2>

<p>Several kind of articles have prominent summary boxes. These have two goals:</p>

<ul>
 <li>Presenting some technical information always at the same position so that user can find it very very quickly.</li>
 <li>With the background color, give the sense of being in a specific area.</li>
</ul>

<p>We have such boxes for CSS properties reference pages, HTML elements, JavaScript method and property, WebAudio Node, events. We may have one or two new needs for those in the next two years.</p>

<h3 id="CSS">CSS</h3>

<p>{{cssbox("flex-flow")}}</p>

<h3 id="HTML">HTML</h3>

<ul class="htmlelt">
 <li><dfn><a href="/en-US/docs/HTML/Content_categories" title="HTML/Content_categories">Content categories</a></dfn> <a href="/en-US/docs/HTML/Content_categories#Flow_content" title="HTML/Content categories#Flow content">Flow content</a>, <a href="/en-US/docs/HTML/Content_categories#Phrasing_content" title="HTML/Content categories#Phrasing content">phrasing content</a>, palpable content.</li>
 <li><dfn>Permitted content</dfn><a href="/en-US/docs/HTML/Content_categories#Phrasing_content" title="HTML/Content categories#Phrasing content">Phrasing content</a>.</li>
 <li><dfn>Tag omission</dfn> {{no_tag_omission}}</li>
 <li><dfn>Permitted parent elements</dfn> Any element that accepts <a href="/en-US/docs/HTML/Content_categories#Phrasing_content" title="HTML/Content_categories#Phrasing_content">phrasing content</a>.</li>
 <li><dfn>DOM interface</dfn> {{domxref("HTMLDataElement")}}</li>
</ul>

<h3 id="Events">Events</h3>

<ul class="summary-box-events">
 <li><dfn>Specification</dfn> <a class="external" href="http://www.whatwg.org/specs/web-apps/current-work/multipage/dom.html#current-document-readiness">HTML5</a></li>
 <li><dfn>Interface</dfn><a href="/en-US/docs/HTML/Content_categories#Phrasing_content" title="HTML/Content categories#Phrasing content">Phrasing content</a>.</li>
 <li><dfn>Bubbles</dfn> No</li>
 <li><dfn>Cancelable</dfn> No</li>
 <li><dfn>Target</dfn> Document</li>
 <li><dfn>Default Action</dfn> None</li>
</ul>

<h3 id="JavaScript">JavaScript</h3>

<ul class="summary-box-js">
 <li><dfn><a href="/en-US/docs/HTML/Content_categories" title="HTML/Content_categories">Content categories</a></dfn> <a href="/en-US/docs/HTML/Content_categories#Flow_content" title="HTML/Content categories#Flow content">Flow content</a>, <a href="/en-US/docs/HTML/Content_categories#Phrasing_content" title="HTML/Content categories#Phrasing content">phrasing content</a>, palpable content.</li>
 <li><dfn>Permitted content</dfn><a href="/en-US/docs/HTML/Content_categories#Phrasing_content" title="HTML/Content categories#Phrasing content">Phrasing content</a>.</li>
 <li><dfn>Tag omission</dfn> {{no_tag_omission}}</li>
 <li><dfn>Permitted parent elements</dfn> Any element that accepts <a href="/en-US/docs/HTML/Content_categories#Phrasing_content" title="HTML/Content_categories#Phrasing_content">phrasing content</a>.</li>
 <li><dfn>DOM interface</dfn> {{domxref("HTMLDataElement")}}</li>
</ul>

<h2 id="Syntax_boxes">Syntax boxes</h2>

<p>The classical CSS syntax box:</p>

<pre class="twopartsyntaxbox">
<a href="/en-US/docs/CSS/Value_definition_syntax" title="CSS/Value_definition_syntax">Formal syntax</a>: {{csssyntax("flex")}}
</pre>

<pre>
flex: none                                            <em>/* value 'none' case */</em>
flex: &lt;'flex-grow'&gt;                                   <em>/* One value syntax, variation 1 */</em>
flex: &lt;'flex-basis'&gt;                                  <em>/* One value syntax, variation 2 */</em>
flex: &lt;'flex-grow'&gt; &lt;'flex-basis'&gt;                    <em>/* Two values syntax, variation 1 */</em>
flex: &lt;'flex-grow'&gt; &lt;'flex-shrink'&gt;                   <em>/* Two values syntax, variation 2 */</em>
flex: &lt;'flex-grow'&gt; &lt;'flex-shrink'&gt; &lt;'flex-basis'&gt;    <em>/* Three values syntax */</em>

flex: inherit</pre>

<p>The API syntax box:</p>

<pre class="syntaxbox">
<em>b</em> = <em>encoder</em>.encoding;</pre>

<h2 id="Banners">Banners</h2>

<p>In general we are fighting banners, there are a few exceptions, and still a lot of banners to remove (by incorporating the information in some other widgets...).</p>

<h3 id="Status_of_the_feature">Status of the feature</h3>

<p>These banners are really important: they indicate if a feature is experimental, obsolete, deprecated or non-standard. This is a very important piece of information: we want to make people to think about it before using it.</p>

<p>{{SeeCompatTable}}</p>

<p>(Harmony variant:</p>

<p>{{Harmony}}</p>

<p>{{obsolete_header}}</p>

<p>{{deprecated_header}}</p>

<p>{{non-standard_header}}</p>

<p>We also use special widgets to indicate it in some list, maybe we want to use similar colors and or the icon in big:</p>

<p>&nbsp;</p>

<h3 id="Others">Others</h3>

<p>{{draft}}</p>

<div class="overheadIndicator draft draftHeader"><strong>This page is not complete</strong>

<div>Firefox 25 hasn't reached its feature freeze yet. New features will be added to it in the near future.</div>
</div>

<h3 id="Phasing_out_(but_long-term)">Phasing out (but long-term)</h3>

<p>{{MobileOnlyHeader}}</p>

<p>{{gecko_minversion_header(17)}}</p>

<p>{{fx_minversion_header(3)}}</p>

<p>{{tb_minversion_header(3)}}</p>

<p>{{js_minversion_header("1.8.5")}}</p>

<p>{fx_minversion_note(3)}}</p>

<p>{{tb_minversion_header(3)}}</p>

<p>{{js_minversion_header("1.8.5")}}</p>

<p>{{warning("texttexttext")}}</p>

<p>{{outdated("outdatedoutdated")}}</p>

<p>{{lockedPage}}</p>

<p>{{unimplemented_header}}</p>

<p>I probably have missed a few of these banners. We need a rule to define border/content colors for them as we stumble on them. We don't plan to add many more, but new use case may arise in the future (I hate banners).</p>

<h2 id="Badges">Badges</h2>

<p>I also try to minimize the amount of badges (I call pages with a lot of these "Christmas trees". But here are the most common</p>

<p>{{non-standard_inline}} {{obsolete_inline}} {{experimental_inline}} {{deprecated_inline}} (the counter parts of the banners, these will stay in the future but their usage strictly limited to titles or &lt;dt&gt; of definition lists.</p>

<p>{{optional_inline}} {{readOnlyInline}}</p>

<ul>
 <li><code>SomeAPIWithNewName</code> {{renamed_inline}}</li>
 <li><code>AnUnimplementedAPI</code> {{unimplemented_inline}}</li>
 <li><code>AMethodNotAvailableInXPCOM</code> {{notxpcom_inline}}</li>
</ul>

<p>Phasing out:{{gecko_minversion_inline(5)}} {{fx_minversion_inline(5)}} {{tb_minversion_inline(5)}} {{js_minversion_inline(5)}} {{dom_level(5)}}</p>

<h2 id="Community_information_boxes">Community information boxes</h2>

<p>This box will be presented on all (or almost all) top-level landing pages for given technologies or topic areas, to provide links to the appropriate IRC channel, newsgroup, and other forums (like Stack Overflow).</p>

<div class="overheadIndicator communitybox">
<div class="column-container">
<div class="column-half">
<h2 id="Join_the_Community">Join the Community</h2>

<h3 id="Mailing_ListNewsgroup">Mailing List/Newsgroup</h3>

<ul class="communitymailinglist">
 <li><a href="">Some Item</a></li>
 <li><a href="">Some Item</a></li>
 <li><a href="">Some Item</a></li>
 <li><a href="">Some Item</a></li>
</ul>
</div>

<div class="column-half">
<ul class="communitycontact">
 <li><strong>Heading: </strong> Blah</li>
 <li><strong>Heading: </strong> Blah</li>
 <li><strong>Heading: </strong> Blah</li>
</ul>
</div>
</div>
</div>

<div class="note">
<p><strong>Notes:</strong> The "Mailing list/newsgroup" list will always be those four options. There will always be only one IRC option. The "Get help" section may not exist at all, or may have any number of options. See http://jsfiddle.net/3XxQL/ for the styled version of this prototype.</p>
</div>

<p>&nbsp;</p>

