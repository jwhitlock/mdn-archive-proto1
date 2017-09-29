---
version: prototype1
revision_id: 1312163
locale: vi
slug: Web/JavaScript
tags: "Landing" "JavaScript" "Học javascript"
title: JavaScript
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{JsSidebar()}}</div>

<div class="summary">
<p><strong>JavaScript</strong><sup>®</sup> (viết tắt là&nbsp;<strong>JS</strong>) là một ngôn ngữ lập trình hướng đối tượng thông dịch và&nbsp;gọn nhẹ với đặc tính&nbsp;<a href="https://en.wikipedia.org/wiki/First-class_functions" style="font-weight: bold; background-color: rgb(244, 247, 248);" title="https://en.wikipedia.org/wiki/First-class_functions">hàm&nbsp;đối tượng</a>&nbsp;(<a href="https://en.wikipedia.org/wiki/First-class_functions" title="https://en.wikipedia.org/wiki/First-class_functions">first-class functions</a>). JavaScript được biết tới như một ngôn ngữ kịch bản phía máy khách trong các trong Web - tức là thực thi trên trình duyệt, nhưng nó cũng được sử dụng rất nhiều ở các <a class="external" href="http://en.wikipedia.org/wiki/JavaScript#Uses_outside_web_pages">môi trường phi trình duyệt</a>&nbsp;như&nbsp;&nbsp;<a class="external" href="http://nodejs.org/">node.js</a> hay&nbsp;<a href="http://couchdb.apache.org">Apache CouchDB</a>. Ngôn ngữ này có đặc điểm là một&nbsp;ngôn ngữ kịch bản <a class="mw-redirect" href="https://en.wikipedia.org/wiki/Prototype-based" style="text-decoration: underline; font-weight: bold; background-color: rgb(244, 247, 248);" title="Prototype-based">dựa trên nguyên mẫu</a>&nbsp;(<a class="mw-redirect" href="https://en.wikipedia.org/wiki/Prototype-based" title="Prototype-based">prototype-based</a>), đa hình (multi-paradigm) nên khá linh động&nbsp;dynamic và hỗ trược được cả các phong cách lập trình hướng đối tượng, lập trình mệnh lệnh và lập trình hàm.&nbsp;Bạn có thể đọc thêm về JavaScript ở&nbsp;<a href="/en-US/docs/Web/JavaScript/About_JavaScript">đây</a>.</p>
</div>

<p><a href="/en-US/docs/JavaScript/Language_Resources">ECMAScript</a>&nbsp;là&nbsp;tiêu chuẩn chung cho&nbsp;JavaScript và tính&nbsp;tới thời điểm&nbsp;năm&nbsp;2012 thì tất cả các trình duyện hiện đại đều đã&nbsp;hỗ trợ đầy đủ các tiêu chuẩn&nbsp;ECMAScript 5.1, còn một số trình duyệt cũ thì cũng hỗ trợ ít nhất ở phiên bản&nbsp;ECMAScript 3. Vào ngày 17 tháng 06 năm 2015, phiên bản chính thức thứ 6 của ECMAScript đã được phát hành với tên gọi chính thức là ECMAScript 2015, nhưng nó cũng hay được gọi với tên là ECMAScript 6 hoặc ES6.</p>

<p>Phần này dành riêng cho việc hướng dẫn về ngôn ngữ JavaScript chứ không mô tả cụ thể cho từng môi trường như Web hay cho các môi trường máy chủ. Về các API dành riêng cho Web, bạn có thể xem ở&nbsp;phần&nbsp;<a href="/en-US/docs/Web/API">Web APIs</a> và&nbsp;<a href="/en-US/docs/Glossary/DOM">DOM</a>.</p>

<p>Lưu ý rằng JavaScript khác với&nbsp;<a href="http://en.wikipedia.org/wiki/Java_(programming_language)">ngôn ngữ lập trình Java</a>&nbsp;nên đừng nhầm lẫn với Java. Java là một nhãn hiệu được đăng kí bởi Oracle tại Mĩ và các quốc gia khác nữa.</p>

<div class="column-container">
<div class="column-half">
<h2 id="Creating" name="Creating">Hướng dẫn</h2>

<p>Học cách lập trình bằng&nbsp;JavaScript.</p>

<h3 id="Mở_đầu">Mở đầu</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide">Dẫn nhập về&nbsp;JavaScript</a></dt>
 <dd>Bạn chưa biết về JavaScript? Tốt, phần này sẽ dẫn bạn đi một vòng qua ngôn ngữ này.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/JavaScript_technologies_overview">Tổng quan về các công nghệ JavaScript</a></dt>
 <dd>Giới thiệu về hiện trạng của JavaScript ở các trình duyệt Web.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Introduction_to_Object-Oriented_JavaScript">Nhập môn hướng đối tượng với JavaScript</a></dt>
 <dd>Giới thiệu các khái niệm về lập trình hướng đối tượng trong&nbsp;JavaScript.</dd>
</dl>

<h3 id="Căn_bản">Căn bản</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript">Giới thiệu lại về&nbsp;JavaScript</a></dt>
 <dd>Một bản tổng quan dành cho người đã <em>biết</em>&nbsp;về&nbsp;JavaScript.</dd>
</dl>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures">Cấu trú dữ liệu trong&nbsp;</a><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures" style="font-weight: bold;">JavaScript</a></dt>
 <dd>Tổng quan về các cấu trúc dữ liệu trong&nbsp;JavaScript.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Equality_comparisons_and_when_to_use_them">Các phép so sánh bằng và cách sử dụng</a></dt>
 <dd>JavaScript cung cấp 3 kiểu so sánh giá trị khác nhau là: so sánh bằng chặt chẽ&nbsp;với&nbsp;<code>===</code>&nbsp;và so sánh bằng lỏng lẻo&nbsp;với&nbsp;<code>==.</code></dd>
</dl>

<h3 id="Nâng_cao">Nâng cao</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Inheritance_and_the_prototype_chain">Kế thừa và chuỗi nguyên mẫu</a></dt>
 <dd>Giải thích về sự hiểu lầm và đánh giá không chuẩn về&nbsp;kế thừa dựa trên nguyên mẫu (prototype-based inheritance)</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Strict_mode">Dạng chặt (strict mode)</a></dt>
 <dd>Một biến thể bị giới hạn&nbsp;của&nbsp;JavaScript.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Typed_arrays">Các kiểu dữ liệu&nbsp;mảng của JavaScript</a></dt>
 <dd>Các mảng của&nbsp;JavaScript cung cấp cơ chế truy cậ dữ liệu nhị phân gốc (raw binary data).</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Memory_Management">Quản lý bộ nhớ</a></dt>
 <dd>Về vòng đời bộ nhớ và bộ dọn rác trong&nbsp;JavaScript.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Tài_liệu">Tài liệu</h2>

<p>Xem bộ&nbsp;tài liệu&nbsp;<a href="/en-US/docs/Web/JavaScript/Reference">tham chiếu JS</a>&nbsp;đầy đủ.</p>

<dl>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects">Các đối tượng tiêu chuẩn</a></dt>
 <dd>Hướng dẫn về một số đối tượng chuẩn được xây dựng sẵn như&nbsp;<code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array" title="The JavaScript Array global object is a constructor for arrays, which are high-level, list-like objects."><code>Array</code></a></code>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean" title="The Boolean object is an object wrapper for a boolean value."><code>Boolean</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date" title="Creates a JavaScript Date instance that represents a single moment in time. Date objects are based on a time value that is the number of milliseconds since 1 January, 1970 UTC."><code>Date</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error" title="The Error constructor creates an error object. Instances of Error objects are thrown when runtime errors occur. The Error object can also be used as a base objects for user-defined exceptions. See below for standard built-in error types."><code>Error</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function" title="The Function constructor creates a new Function object. In JavaScript every function is actually a Function object."><code>Function</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON" title="The JSON object contains methods for parsing JavaScript Object Notation (JSON) and converting values to JSON. It can't be called or constructed, and aside from its two method properties it has no interesting functionality of its own."><code>JSON</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math" title="Math is a built-in object that has properties and methods for mathematical constants and functions. Not a function object."><code>Math</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number" title="The Number JavaScript object is a wrapper object allowing you to work with numerical values. A Number object is created using the Number() constructor."><code>Number</code></a>, <a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object"><code>Object</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp" title="The RegExp constructor creates a regular expression object for matching text with a pattern."><code>RegExp</code></a>, <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String" title="The String global object is a constructor for strings, or a sequence of characters."><code>String</code></a>,&nbsp;<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map" title="The Map object is a simple key/value map. Any value (both objects and primitive values) may be used as either a key or a value."><code>Map</code></a>, <code><a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set">Set</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/WeakMap" title="The WeakMap object is a collection of key/value pairs in which the keys are objects and the values can be arbitrary values."><code>WeakMap</code></a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/WeakSet" title="The WeakSet object lets you store weakly held objects in a collection.">WeakSet</a>..</code>.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Operators">Các biểu thức và toán tử</a></dt>
 <dd>Học thêm về các xử lý của các toán tử trong JavaScript như&nbsp;<code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/instanceof">instanceof</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/typeof">typeof</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/new">new</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this">this</a></code>...</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Statements">Các câu lệnh và khai báo</a></dt>
 <dd>Học về các câu lệnh và cách khai báo cũng như các từ khóa trong JavaScirpt như&nbsp;<code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/do...while">do-while</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...in">for-in</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...of">for-of</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/try...catch">try-catch</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let">let</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var">var</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const">const</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/if...else">if-else</a></code>, <code><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/switch">switch</a>..</code>.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Functions">Hàm</a></dt>
 <dd>Học cách làm việc với các hàm trong JS để phát triển các&nbsp;ứng dụng của bạn.</dd>
</dl>

<h2 id="Công_cụ_tài_nguyên">Công cụ &amp; tài nguyên</h2>

<p>Các công cụ hữu dụng để viết mã và &nbsp;gỡ lỗi&nbsp;với JavaScript.</p>

<dl>
 <dt><a href="/en-US/docs/Tools">Các công cụ phát triển của Firefox</a></dt>
 <dd><a href="/en-US/docs/Tools/Scratchpad">Scratchpad</a>, <a href="/en-US/docs/Tools/Web_Console">Web Console</a>, <a href="/en-US/docs/Tools/Profiler">JavaScript Profiler</a>, <a href="/en-US/docs/Tools/Debugger">Debugger</a>...</dd>
 <dt><a class="external" href="http://www.getfirebug.com/">Firebug</a></dt>
 <dd>Chỉnh sửa, gỡ lỗi, và theo dõi các mã&nbsp;CSS, HTML, và&nbsp;JavaScript trực tiếp với bất kì trang web nào.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Shells">JavaScript Shells</a></dt>
 <dd>A JavaScript shell cho phép bạn kiểm tra nhanh chóng&nbsp;các đoạn mã JavaScript.</dd>
 <dt><a href="https://togetherjs.com/">TogetherJS</a></dt>
 <dd>
 <p class="hero-header-text large">Hợp tác để giải quyết các vấn đề dễ hơn.</p>
 </dd>
 <dt><a href="http://stackoverflow.com/questions/tagged/javascript">Stack Overflow</a></dt>
 <dd>Các câu hỏi được đánh thẻ&nbsp;"JavaScript" trên hệ thống giải đáp Stack Overflow.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/New_in_JavaScript">Các phiên bản&nbsp;JavaScript và các chú thích phát hành</a></dt>
 <dd>Xem thêm về lịch sử của&nbsp;JavaScript cùng với các chú thích của nó.</dd>
</dl>
</div>
</div>

<p>{{CommunityBox("JavaScript", "js-engine.internals", "mozilla.dev.tech.js-engine.internals", "js", "ES discuss|http://esdiscuss.org/|esdiscuss.org|ECMAScript - thư thảo luận chính thức&nbsp;||SpiderMonkey|https://wiki.mozilla.org/JavaScript|Project page|Đóng góp cho&nbsp;JavaScript Engine||Twitter|https://twitter.com/FirefoxNightly|@FirefoxNightly|Cập nhập của&nbsp;Firefox Nightly trên&nbsp;Twitter")}}</p>

