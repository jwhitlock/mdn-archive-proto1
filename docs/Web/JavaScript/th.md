---
version: prototype1
revision_id: 1252165
locale: th
slug: Web/JavaScript
tags: "Landing" "TopicStub" "JavaScript" "NeedsTranslation"
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

<p class="summary"><strong>JavaScript</strong> (<strong>JS</strong>) เป็นภาษาโปรแกรมชนิดหนึ่ง, ภาษามีขนาดเล็ก, อาศัยตรวจแปลภาษา, มีคุณสมบัติ&nbsp;<a href="https://en.wikipedia.org/wiki/First-class_functions" title="https://en.wikipedia.org/wiki/First-class_functions">first-class functions.&nbsp;</a> คนส่วนใหญ่จะรู้จักว่าเป็นภาษาสคริปต์สำหรับหน้าเวบ แต่ปัจจุบันมีการนำไปใช้ใน&nbsp;<a href="https://en.wikipedia.org/wiki/JavaScript#Uses_outside_web_pages">สภาพแวดล้อมอื่นๆอีกจำนวนมากที่ไม่ใช่ browser</a> เช่น <a class="external" href="https://nodejs.org/">node.js</a>&nbsp;หรือ&nbsp;<a href="https://couchdb.apache.org/">Apache CouchDB</a>. JS เป็นภาษาแบบ&nbsp;<a class="mw-redirect" href="https://en.wikipedia.org/wiki/Prototype-based_programming" title="Prototype-based">prototype-based</a>, multi-paradigm, dynamic&nbsp;scripting&nbsp;สนับสนุนสไตล์การเชียนแบบ&nbsp;object-oriented, imperative และ declarative ( เช่น การโปรแกรมแบบ functional) <a href="/en-US/docs/Web/JavaScript/About_JavaScript">อ่านเพิ่มเติม</a></p>

<p>ส่วนนี้ของเวปไซท์มีไว้สำหรับภาษา JavaScript โดยเฉพาะ, เนื้อหายังไม่เจาะจงกับการเขียนหน้าเวป&nbsp;หรือ&nbsp;สภาพแวดล้อมอื่นๆ. สำหรับเนื้อหาเกี่ยวกับ <a href="http://en.wikipedia.org/wiki/Application_programming_interface">APIs</a>&nbsp;สำหรับการเขียนเวปโดยตรงนั้นสามารถดูได้ที่&nbsp;<a href="/en-US/docs/Web/API">Web APIs</a> และ <a href="/en-US/docs/Glossary/DOM">DOM</a></p>

<p>มาตรฐานของ&nbsp;JavaScript คือ&nbsp;<a href="/en-US/docs/JavaScript/Language_Resources">ECMAScript</a>. นับตั้งแต่ปี 2012 เป็นต้นมา&nbsp;browser ยุคใหม่ทั้งหมดรองรับการทำงานตามมาตรฐาน&nbsp;ECMAScript 5.1 อย่างสมบูรณ์&nbsp;ในขณะที่ browser ที่เก่ากว่านั้นจะรองรับอย่างน้อย ECMAScript 3. ในวันที่ 17 มิถุนายน 2015&nbsp;<a href="http://www.ecma-international.org/">ECMA International</a>&nbsp;ได้ตีพิมพ์มาตรฐาน ECMAScript รุ่นที่ 6 ซึ่งมีชื่อเรียกอย่างเป็นทางการว่า&nbsp;ECMAScript 2015 แต่เป็นที่รู้จักโดยทั่วไปว่า&nbsp;ECMAScript 6 หรือ ES6. นับตั้งแต่นั้นมาตรฐาน ECMAScript ก็จะถูกปรับปรุงทุกปี.&nbsp; สำหรับเอกสาร(ที่ท่านอ่าน) นี้อ้างถึงมาตรฐานฉบับร่างรุ่นล่าสุด, ซึ่งปัจจุบันคือ <a href="http://tc39.github.io/ecma262/">ECMAScript 2017</a>.</p>

<p>อย่าสับสน JavaScript กับ ภาษา <a href="https://en.wikipedia.org/wiki/Java_(programming_language)">Java</a>. ทั้ง&nbsp; "Java" and "JavaScript" เป็น ตราสินค้าจดทะเบียนของบริษัท Oracle ในสหรัฐอเมริกาและประเทศอื่นๆ. ทั้งสองภาษามีความต่างอย่างมากทั้งด้าน วากยสัมพันธ์ (syntax), ความหมาย (semantics) และการใช้งาน</p>

<div class="column-container">
<div class="column-half">
<h2 id="บทเรียน">บทเรียน</h2>

<p>เรียนรู้วิธีการเขียนโปรแกรมด้วย JavaScript</p>

<h3 id="เบี้องต้น">เบี้องต้น</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/th/docs/Web/JavaScript/Guide">คู่มือจาวาสคริปต์</a></dt>
 <dd>ถ้าคุณไม่รู้จัก Javascript มาก่อน คู่มือนี้จะแนะนำให้คุณรู้จักภาษานี้</dd>
 <dt><a href="https://developer.mozilla.org/th/docs/Web/JavaScript/JavaScript_technologies_overview">ภาพรวมของเทคโนโลยีจาวาสคริปต์</a></dt>
 <dd>บทนำเกี่ยวกับสภาพโดยทั่วไปของ Javascript บนเว็บเบราเซอร์</dd>
 <dt><a href="https://developer.mozilla.org/th/docs/Web/JavaScript/Introduction_to_Object-Oriented_JavaScript">บทนำเกี่ยวกับจาวาสคริปต์เชิงวัตถุ</a></dt>
 <dd>บทนำเกี่ยวกับแนวความคิดการเขียนโปรแกรมเชิงวัตถุใน&nbsp;JavaScript.</dd>
</dl>

<h3 id="ขั้นกลาง">ขั้นกลาง</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/th/docs/Web/JavaScript/A_re-introduction_to_JavaScript">บทนำอีกครั้งเกี่ยวกับจาวาสคริปต์</a></dt>
 <dd>คำอธิบายคร่าวๆ สำหรับผู้ที่คิดว่ารู้จักจาวาสคริปต์มาก่อนแล้ว</dd>
</dl>

<dl>
 <dt><a href="https://developer.mozilla.org/th/docs/Web/JavaScript/Data_structures">โครงสร้างข้อมูลของจาวาสคริปต์</a></dt>
 <dd>คำอธิบายคร่าวๆเกี่ยวกับโครงสร้างข้อมูลที่มีในจาวาสคริปต์</dd>
 <dt><a href="https://developer.mozilla.org/th/docs/Web/JavaScript/Equality_comparisons_and_sameness">การเปรียบเทียบความเท่ากันและความเหมือน</a></dt>
 <dd>จาวาสคริปต์มีคำสั่งที่ใช้เปรียบเทียบอยู่สามแบบที่แตกต่างกัน: strict equality using ===, loose equality using == และ&nbsp;&nbsp;<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/is" title="The Object.is() method determines whether two values are the same value."><code>Object.is()</code></a>&nbsp;method</dd>
</dl>

<h3 id="ระดับสูง">ระดับสูง</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/th/docs/Web/JavaScript/Inheritance_and_the_prototype_chain">การสืบทอดและความต่อเนื่องของต้นแบบ</a></dt>
 <dd>การอธิบายสิ่งที่มักเข้าใจผิดๆ และการใช้การสืบทอดแบบ prototype-based อย่างไม่ถูกต้อง</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Strict_mode">Strict mode</a></dt>
 <dd>โหมด Strict จะทำให้คุณไม่สามารถใช้ตัวแปรใดๆ ก่อนที่จะมีการกำหนดค่าตั้งต้นให้แก่ตัวแปรนั้นได้ โหมดนี้จะควบคุมความแตกต่างของ ECMAScript 5 เพื่อประสิทธิภาพที่เร็วกว่าและง่ายสำหรับการแก้ไขจุดบกพร่อง</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Typed_arrays">JavaScript typed arrays</a></dt>
 <dd>ชนิดข้อมูลแบบอาเรย์มีกระบวนการสำหรับการเข้าถึงข้อมูลแบบไบนารี่</dd>
 <dt><a href="https://developer.mozilla.org/th/docs/Web/JavaScript/Memory_Management">การจัดการหน่วยความจำ</a></dt>
 <dd>วงจรชีวิตหน่วยความจำและการกำจัดหน่วยความจำที่ไม่ใช้แล้วในจาวาสคริปต์</dd>
</dl>
</div>

<div class="column-half">
<h2 id="อ้างอิง">อ้างอิง</h2>

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

<h2 id="เครื่องมือและแหล่งที่มา">เครื่องมือและแหล่งที่มา</h2>

<p>เครื่องมือที่ช่วยในขณะการเขียน และดีบั๊กโค๊ด&nbsp;JavaScript.</p>

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

