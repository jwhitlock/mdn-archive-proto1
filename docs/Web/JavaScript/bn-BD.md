---
version: prototype1
revision_id: 1309127
locale: bn-BD
slug: Web/JavaScript
tags: "জাভা স্ক্রিপ্ট" "জাভাস্ক্রিপ্ট"
title: জাভাস্ক্রিপ্ট
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<div>{{JsSidebar}}</div>

<p class="summary"><strong>JavaScript</strong>&nbsp;(সংক্ষেপে <strong>JS</strong>) একটি lightweight ইন্টারপ্রেটেড বা JIT কম্পাইল করা&nbsp;প্রোগ্রামিং ভাষা যাতে রয়েছে&nbsp;{{Glossary("First-class Function", "first-class functions")}}। এটি ওয়েব পেজের স্ক্রিপ্টিং ভাষা হিসেবে বেশি পরিচিত, এছাড়া&nbsp;<a class="external" href="https://en.wikipedia.org/wiki/JavaScript#Uses_outside_Web_pages">ব্রাউজার ছাড়াও অন্যান্য জায়গায়</a> ব্যবহার করা হয়, যেমন <a class="external" href="https://nodejs.org/">node.js</a> and <a href="https://couchdb.apache.org/">Apache CouchDB</a>. JavaScript&nbsp;হল {{Glossary("Prototype-based programming", "prototype-based")}}, multi-paradigm, dynamic scripting language, supporting object-oriented, imperative, and declarative (e.g. functional programming) styles. <a href="/en-US/docs/Web/JavaScript/About_JavaScript">JavaScript সম্পর্কে</a>&nbsp;আরো পড়ুন.</p>

<p>সাইটের এই সেকশনটি JavaScript ভাষার জন্য&nbsp;নিবেদিত, এবং ওয়েব পেইজ অথবা হোস্ট এনভাইরনমেন্টের সাথে সম্পৃক্ত নয়।&nbsp;{{Glossary("API","APIs")}} সম্পর্কে জানতে&nbsp;<a href="https://developer.mozilla.org/en-US/docs/Web/API">Web APIs</a>&nbsp;এবং&nbsp;<a href="https://developer.mozilla.org/en-US/docs/Glossary/DOM">DOM</a>&nbsp;দেখুন।</p>

<p>JavaScript&nbsp; স্ট্যান্ডার্ড এর নাম <a href="/bn-BD/docs/JavaScript/%E0%A6%AD%E0%A6%BE%E0%A6%B7%E0%A6%BE%E0%A6%B0_%E0%A6%B0%E0%A6%BF%E0%A6%B8%E0%A7%8B%E0%A6%B0%E0%A7%8D%E0%A6%B8" title="ECMAScript">ECMAScript</a>। ২০১২ সাল পর্যন্ত পাওয়া তথ্য অনুযায়ী সব <a href="https://kangax.github.io/compat-table/es5/">নতুন ব্রাউজার</a> ECMAScript 5.1 সমর্থন করে। পুরোনো ব্রাউজারগুলো অন্তত ECMAScript 3 সমর্থন করে। ২০১৫ সালের ১৭ জুন <a href="http://www.ecma-international.org">ECMA International</a> তার ষষ্ঠ প্রধান সংস্করণ প্রকাশ করে, আনুষ্ঠানিক ভাবে যা ECMAScript 2015 নামে অভিহিত, এবং সাধারন ভাবে এটি ECMAScript 6 বা ES6 নামে পরিচিত। তখন থেকেই বাৎসরিক প্রকাশ চক্র অনুযায়ী ECMAScript -এর মান প্রকাশিত হচ্ছে। এই ডকুমেন্টেশনটি সর্বশেষ খসড়া সংস্করণ, যা <a href="https://tc39.github.io/ecma262/">ECMAScript 2018</a> কে বোঝায়।</p>

<p>&nbsp;JavaScript এর সাথে&nbsp; <a href="https://en.wikipedia.org/wiki/Java_%28programming_language%29">Java programming language</a> কে গুলিয়ে ফেলবেন&nbsp;না। "Java" এবং "JavaScript" উভয় প্রোগ্রামিং ভাষাই Oracle কোম্পানির ট্রেডমার্ক বা ট্রেডমার্ক হিসেবে নিবন্ধিত যুক্তরাষ্ট্র এবং&nbsp;অন্যান্য দেশে। যাইহোক, এই দুই প্রোগ্রামিং ভাষার বাক্য গঠন প্রণালী (syntax), শব্দার্থবিদ্যা(semantics), এবং ব্যবহার একেবারেই আলাদা।</p>

<div class="column-container">
<div class="column-half">
<h2 id="টিউটোরিয়াল">টিউটোরিয়াল</h2>

<p>শিখুন কিভাবে জাভাস্ক্রিপ্ট দিয়ে &nbsp;প্রোগ্রাম করে।</p>

<h3 id="প্রারম্ভিক">প্রারম্ভিক</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide">জাভাস্ক্রিপ্ট</a><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide">&nbsp;গাইড</a></dt>
 <dd>যদি আপনি জাভাস্ক্রিপ্ট নতুন হয়ে থাকেন;, এই সহায়িকার মাধ্যমে আপনি এই&nbsp;ভাষার সম্পূর্ণ ধারনা পাবেন।</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/JavaScript_technologies_overview">এক নজরে জাভাস্ক্রিপ্টের প্রযুক্তি</a></dt>
 <dd>ওয়েব ব্রাউজারে জাভাস্ক্রিপ্ট পরিচিতি।</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Introduction_to_Object-Oriented_JavaScript">অবজেক্ট&nbsp;ওরিয়েন্টেড&nbsp;জাভাস্ক্রিপ্ট এর পরিচিতি&nbsp;</a></dt>
 <dd>&nbsp;অবজেক্ট ওরিয়েন্টেড প্রোগ্রামিং&nbsp;জাভাস্ক্রিপ্ট&nbsp;সম্পরকে আলোচনা।&nbsp;&nbsp;</dd>
</dl>

<h3 id="মধ্যবর্তী">মধ্যবর্তী</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript">জাভাস্ক্রি</a><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript">প্ট এর&nbsp;&nbsp;পুনঃউপস্থাপন</a></dt>
 <dd>যারা জাভাস্ক্রিপ্ট সম্পর্কে&nbsp;জানতে&nbsp;চায়ম, তাদের&nbsp;জন্য একটি সংক্ষিপ্ত বিবরণ।</dd>
</dl>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures">জাভাস্ক্রিপ্ট এর&nbsp;ডাটা স্ট্রাকচার&nbsp;</a></dt>
 <dd>জাভাস্ক্রিপ্ট এর&nbsp;ডাটা স্ট্রাকচার সম্পর্কে আলোচনা।</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness">সমতুল্যতা এবং অভিন্নতা&nbsp;</a></dt>
 <dt><code>জাভাস্ক্রিপ্ট তিনধরনের স্মতাকে সমর্থন&nbsp;করে: কঠোর সমতার ক্ষেত্রে&nbsp;=== এবং শিথিল&nbsp;সমতার ক্ষেত্রে&nbsp;== ।</code></dt>
</dl>

<h3 id="এডভান্স">এডভান্স</h3>

<dl>
 <dt><a href="/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain">ইনহেরিটেন্স এবং প্রোটোটাইপ চেইন</a></dt>
 <dd>ব্যাপক&nbsp;ভুল বুঝা&nbsp;এবং অবহেলা করা হচ্ছে&nbsp;প্রোটোটাইপ ইনহেরিটেন্স ব্যাখ্য ।</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Strict_mode">কঠোর মুড</a></dt>
 <dd>কঠোর মুডের সঙ্গা হচ্ছে&nbsp;&nbsp;যে আপনি এটি আরম্ভ করার পূর্বে কোনো ভেরিয়েবল ব্যবহার করতে পারবেন না।&nbsp;এটা ECMAScript 5 একটি&nbsp;সীমাবদ্ধতা,&nbsp;দ্রুত কর্মক্ষমতা এবং সহজ ডিবাগিংএর&nbsp;জন্য।&nbsp;</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Typed_arrays">জাভাস্ক্রিপ্টের&nbsp;অ্যারে টাইপ</a></dt>
 <dd>জাভাস্ক্রিপ্টের অ্যারে নতুন&nbsp;বাইনারি তথ্য অ্যাক্সেসের জন্য একটি প্রক্রিয়া প্রদান &nbsp;করে।</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Memory_Management">মেমরি ম্যানেজমেন্ট</a></dt>
 <dd>মেমরীর জীবনচক্র এবং জাভাস্ক্রিপ্টের মধ্যেকার আবর্জনা সংগ্রহ।</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Reference">Reference</h2>

<p>ব্রাউজ করুন.সম্পূর্ণ &nbsp;<a href="/en-US/docs/Web/JavaScript/Reference">জেএস-&nbsp;রেফারেন্স</a>&nbsp;ডকুমেন্টেশন ।</p>

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

<p>U.S. এবং অন্যান্য দেশে জাভাস্ক্রিপ্ট ওরাকল এর ট্রেডমার্ক অথবা নিবন্ধিত ট্রেডমার্ক।</p>

