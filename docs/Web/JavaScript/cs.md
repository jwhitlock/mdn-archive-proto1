---
version: prototype1
revision_id: 1002807
locale: cs
slug: Web/JavaScript
tags: "JavaScript"
title: JavaScript
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{JsSidebar}}</div>

<div class="callout-box"><strong><a href="/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript">Procvičení JavaScriptu</a></strong><br />
Přehled pro ty, kteří si <em>myslí</em>, že JavaScriptu rozumí</div>

<p><strong>JavaScript</strong><sup>®</sup> (obvykle zkracováno na&nbsp;<strong>JS</strong>) je nenáročný, interpretovaný, objektově orientovaný jazyk s <a href="https://en.wikipedia.org/wiki/First-class_functions" title="https://en.wikipedia.org/wiki/First-class_functions">first-class funkcemi</a>. Je znám zejména jako skriptovací jazyk pro webové stránky, nicméně je kromě prohlížečů používaný i v <a class="external" href="http://en.wikipedia.org/wiki/JavaScript#Uses_outside_web_pages">mnoha jiných prostředích</a>, např. v&nbsp;<a class="external" href="http://nodejs.org/">node.js</a> nebo&nbsp;<a href="http://couchdb.apache.org">Apache CouchDB</a>. Tento&nbsp;<a class="mw-redirect" href="https://en.wikipedia.org/wiki/Prototype-based" title="Prototype-based">prototypový</a>, <a href="/en-US/docs/multiparadigmlanguage.html" title="/en-US/docs/multiparadigmlanguage.html">multiparadigmatický</a>&nbsp;skriptovací jazyk je dále dynamický<font color="#666666">&nbsp;a podporuje</font><span style="line-height:1.572">&nbsp;jak objektově orientovaný, tak i imperativní a funkcionální programovací styl.</span></p>

<p>Standardem pro JavaScript je&nbsp;<a href="/en-US/docs/JavaScript/Language_Resources">ECMAScript</a>. Všechny moderní prohlížeče od roku 2012 plně podporují ECMAScript 5.1. Starší prohlížeče podporují alespoň ECMAScript 3. Šestá majoritní revize tohoto standardu je stále ve fázi příprav. Aktuální stav nových a vylepšených funkcí naleznete na&nbsp;<a class="external" href="http://wiki.ecmascript.org/doku.php?id=harmony:proposals">vyhrazené wiki</a>.</p>

<p>Tato část webu je věnována samotnému jazyku Javascript, tedy těm částem, které nejsou specifické pro webové stránky, ani jiná prostředí. Detaily API, která jsou určená pro webové stránky, naleznete na stránce&nbsp;<a href="/en-US/docs/DOM">Document Object Model</a> (DOM). O tom, jak si spolu DOM a JavaScript rozumí, si můžete přečíst v <a href="/en-US/docs/Gecko_DOM_Reference/Introduction#DOM_and_JavaScript">Referenčním manuálu DOM</a>.</p>

<p>JavaScript by neměl být zaměňován s&nbsp;<a href="http://en.wikipedia.org/wiki/Java_(programming_language)">programovacím jazykem Java</a>.</p>

<div class="column-container">
<div class="column-half">
<h2 id="Tutoriály">Tutoriály</h2>

<p>Naučte se jak programovat s JavaScriptem pomoci našich návodů a tutoriálů.</p>

<h3 id="Introductory">Úvod</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide">Příručka JavaScriptu</a></dt>
 <dd>Pokud s JavaScriptem začínáte, tato příručka vás jím provede.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/JavaScript_technologies_overview">JavaScript technologies overview</a></dt>
 <dd>Úvod do vlastností JavaScriptu&nbsp;ve webovém prohlížeči.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Introduction_to_Object-Oriented_JavaScript">Introduction to Object Oriented JavaScript</a></dt>
 <dd>Úvod do konceptů objektově orientovaného programování v JavaScriptu.</dd>
</dl>

<h3 id="Intermediate">Pro středně pokročilé</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript">A re-introduction to JavaScript</a></dt>
 <dd>Úvod pro ty, co si <em>myslí</em>, že už o JavaScriptu něco vědí.</dd>
</dl>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures">JavaScript data structures</a></dt>
 <dd>Přehled datových struktur poskytovaných v JavaScriptu.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness">Equality comparisons and sameness</a></dt>
 <dd>JavaScript nabízí tři odlišné operace porovnání:&nbsp;striktní rovnost pomocí&nbsp;<code>===</code>&nbsp;a ne tak striktní rovnost pomocí&nbsp;<code>==.</code></dd>
</dl>

<h3 id="Advanced">Pro pokročilé</h3>

<dl>
 <dt><a href="/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain">Dědění a řetězení prototypů</a></dt>
 <dd>Vysvětlení často nepochopeného a podceňovaného prototypového dědění.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Strict_mode">Strict mode</a></dt>
 <dd>Omezená verze JavaScriptu.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Typed_arrays">JavaScript typed arrays</a></dt>
 <dd>Typovaná pole JavaScriptu poskytují mechanismus pro přístup k nezpracovaným binárním datům.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Memory_Management">Memory Management</a></dt>
 <dd>Životní cyklus paměti a&nbsp;garbage collection v JavaScriptu.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Reference">Reference</h2>

<p>Browse the complete <a href="/en-US/docs/Web/JavaScript/Reference">JS reference</a> documentation.</p>

<dl>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects">Standard objects</a></dt>
 <dd>Get to know standard built-in objects <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array" title="The JavaScript Array global object is a constructor for arrays, which are high-level, list-like objects."><code>Array</code></a></code>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean" title="The Boolean object is an object wrapper for a boolean value."><code>Boolean</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date" title="Creates a JavaScript Date instance that represents a single moment in time. Date objects are based on a time value that is the number of milliseconds since 1 January, 1970 UTC."><code>Date</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error" title="The Error constructor creates an error object. Instances of Error objects are thrown when runtime errors occur. The Error object can also be used as a base objects for user-defined exceptions. See below for standard built-in error types."><code>Error</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function" title="The Function constructor creates a new Function object. In JavaScript every function is actually a Function object."><code>Function</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON" title="The JSON object contains methods for parsing JavaScript Object Notation (JSON) and converting values to JSON. It can't be called or constructed, and aside from its two method properties it has no interesting functionality of its own."><code>JSON</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math" title="Math is a built-in object that has properties and methods for mathematical constants and functions. Not a function object."><code>Math</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number" title="The Number JavaScript object is a wrapper object allowing you to work with numerical values. A Number object is created using the Number() constructor."><code>Number</code></a>, <a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object"><code>Object</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp" title="The RegExp constructor creates a regular expression object for matching text with a pattern."><code>RegExp</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String" title="The String global object is a constructor for strings, or a sequence of characters."><code>String</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map" title="The Map object is a simple key/value map. Any value (both objects and primitive values) may be used as either a key or a value."><code>Map</code></a>, <code><a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set">Set</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/WeakMap" title="The WeakMap object is a collection of key/value pairs in which the keys are objects and the values can be arbitrary values."><code>WeakMap</code></a></code>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/WeakSet" title="The WeakSet object lets you store weakly held objects in a collection."><code>WeakSet</code></a>, and others.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Operators">Expressions &amp; operators</a></dt>
 <dd>Learn more about the behavior of JavaScript's operators <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/instanceof">instanceof</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/typeof">typeof</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/new">new</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this">this</a></code>, and more.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Statements">Statements &amp; declarations</a></dt>
 <dd>Learn how <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/do...while">do-while</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...in">for-in</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...of">for-of</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/try...catch">try-catch</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let">let</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var">var</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const">const</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/if...else">if-else</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/switch">switch</a></code>, and more JavaScript statements and keywords work.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Functions">Functions</a></dt>
 <dd>Learn how to work with JS functions to develop your applications.</dd>
</dl>

<h2 id="Tools_resources">Tools &amp; resources</h2>

<p>Helpful tools while writing and debugging your JavaScript code.</p>

<dl>
 <dt><a href="/en-US/docs/Tools">Firefox Developer Tools</a></dt>
 <dd><a href="/en-US/docs/Tools/Scratchpad">Scratchpad</a>, <a href="/en-US/docs/Tools/Web_Console">Web Console</a>, <a href="/en-US/docs/Tools/Profiler">JavaScript Profiler</a>, <a href="/en-US/docs/Tools/Debugger">Debugger</a>, and more.</dd>
 <dt><a class="external" href="http://www.getfirebug.com/">Firebug</a></dt>
 <dd>Edit, debug, and monitor CSS, HTML, and JavaScript live in any web page.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Shells">JavaScript Shells</a></dt>
 <dd>A JavaScript shell allows you to quickly test snippets of JavaScript code.</dd>
 <dt><a href="https://togetherjs.com/">TogetherJS</a></dt>
 <dd>
 <p class="hero-header-text large">Collaboration made easy.</p>
 </dd>
 <dt><a href="http://stackoverflow.com/questions/tagged/javascript">Stack Overflow</a></dt>
 <dd>Stack Overflow questions tagged with "JavaScript".</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/New_in_JavaScript">JavaScript versions and release notes</a></dt>
 <dd>Browse JavaScript's feature history and implementation status.</dd>
</dl>
</div>
</div>

<p>{{CommunityBox("JavaScript", "js-engine.internals", "mozilla.dev.tech.js-engine.internals", "js", "ES discuss|https://esdiscuss.org/|esdiscuss.org|ECMAScript standard discussion mailing list||SpiderMonkey|https://wiki.mozilla.org/JavaScript|Project page|Contribute to the JavaScript Engine||Twitter|https://twitter.com/SpiderMonkeyJS|@SpiderMonkeyJS|SpiderMonkey updates on Twitter")}}</p>

<p><samp>*JavaScript je ochranná známka nebo registrovaná ochranná známka společnosti Oracle ve Spojených státech a dalších zemích.</samp></p>

