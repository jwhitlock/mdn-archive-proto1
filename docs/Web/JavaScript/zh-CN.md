---
version: prototype1
revision_id: 1343299
locale: zh-CN
slug: Web/JavaScript
tags: "学习" "Landing" "JavaScript"
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
<p><strong>JavaScript&nbsp;(&nbsp;</strong><strong>JS&nbsp;</strong>) 是{{Glossary("First-class Function", "“函数是一等公民”性质")}}的轻量级解释或JIT编译型的编程语言。虽然它是作为开发web页面的脚本语言而出名的，但是在很多<a class="external" href="https://en.wikipedia.org/wiki/JavaScript#Uses_outside_Web_pages">非浏览器环境</a>中也使用JavaScript，例如 <a class="external" href="https://nodejs.org/">node.js</a>&nbsp;和&nbsp;<a class="external" href="https://couchdb.apache.org">Apache CouchDB</a>。JS是一种{{Glossary("Prototype-based_programming", "基于原型")}}、多范式的动态脚本语言，并且支持面向对象、命令式和声明式（如函数式编程）风格。了解更多<a href="https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/About_JavaScript">&nbsp;关于JavaScript</a>。</p>
</div>

<p>本部分将专注于 JavaScript 语言本身，而非局限于网页或其他宿主环境。想要了解网页有关的 {{Glossary("API","APIs")}}&nbsp;，请参考 <a href="/zh-CN/docs/Web/API">Web APIs</a>&nbsp;以及 <a href="/zh-CN/docs/Glossary/DOM">DOM</a>。</p>

<p><a href="/zh-CN/docs/Web/JavaScript/Language_Resources">ECMAScript</a>&nbsp;是&nbsp;JavaScript 的标准。截至 2012 年，所有的<a href="https://kangax.github.io/compat-table/es5/">现代浏览器</a>都完整了支持&nbsp; ECMAScript 5.1，旧式的浏览器至少支持 ECMAScript 3 标准。在2015年6月17日，<a href="https://www.ecma-international.org">ECMA国际组织</a>发布了 ECMAScript 的第六版，该版本正式名称为ECMAScript 2015，但通常被称为 ECMAScript 6 或者ES6。自此，ECMAScript每年发布一次新标准。本文档目前覆盖了最新ECMAScript的草案，也就是<a href="https://tc39.github.io/ecma262/">ECMAScript2018</a>。</p>

<p>不要将 JavaScript 与&nbsp;<a href="https://en.wikipedia.org/wiki/Java_(programming_language)">Java 语言</a>&nbsp;混淆。虽然“Java”和“JavaScript”都是&nbsp;Oracle 公司在美国和其他国家注册（或未注册）的商标，但是这两门语言在语法、语义与用途方面有很大不同。</p>

<div class="column-container">
<div class="column-half">
<h2 id="教程">教程</h2>

<p>学习使用指南和教程去编写 JavaScript 程序。</p>

<h3 id="为初学者准备">为初学者准备</h3>

<p>如果你想学习 JavaScript，但苦于没有过 JavaScript 或者其他语言的编程经验，你可以投入到我们的<a href="/zh-CN/docs/Learn/JavaScript">JavaScript 主题学习区</a>。那里有完整的学习资源：</p>

<dl>
 <dt><a href="/zh-CN/docs/Learn/JavaScript/First_steps">JavaScript 起步</a></dt>
 <dd>回答一些基本问题，比如“JavaScript 是什么？”、“和什么相似？”、“可以做什么？”；同时还讨论如变量、字符串、数值和数组等 JavaScript 的关键特性。</dd>
 <dt><a href="/zh-CN/docs/Learn/JavaScript/Building_blocks">JavaScript 基本结构</a></dt>
 <dd>继介绍了 JavaScript 基本的关键特性后，将注意力转到常见的代码块类型，如条件语句，循环，函数和事件。</dd>
</dl>

<h3 id="JavaScript_指南">JavaScript 指南</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Guide">JavaScript 指南</a></dt>
 <dd>一份更详尽的 JavaScript 指南，适用于有过 JavaScript 或其他语言编程经验的读者。</dd>
</dl>

<h3 id="中级内容">中级内容</h3>

<dl>
 <dt><a href="/zh-CN/docs/Learn/JavaScript/Objects">JavaScript 对象介绍</a></dt>
 <dd>如果你想进一步使用该语言撰写更有效率的代码，理解 JavaScript 面向对象的精髓是很重要的，因此我们提供了该模块来帮助你理解它。</dd>
 <dt><a href="/zh-CN/docs/Learn/JavaScript/Client-side_web_APIs">客户端 Web API</a></dt>
 <dd>当你正在给网页或者网页APP编写客户端 JavaScript 时， 你离不开使用这些API&nbsp;— 这些用来操作浏览器各个不同方面和网页所在的操作系统，甚至是来自于其他网页和服务器的数据的接口。在这个模块，我们来探究这些API是什么，以及怎么在你的日常开发工作中使用一些最常用的API。</dd>
</dl>

<dl>
 <dt><a href="https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/A_re-introduction_to_JavaScript">重新介绍 JavaScript（JS 教程）</a></dt>
 <dd>为那些有 JavaScript 基础的朋友们深入介绍 JavaScript。</dd>
</dl>

<dl>
 <dt><a href="https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Data_structures">JavaScript 数据结构</a></dt>
 <dd>JavaScript 数据结构的概览</dd>
 <dt><a href="https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Equality_comparisons_and_when_to_use_them">如何使用比较操作符</a></dt>
 <dd>JavaScript 提供了三种比较操作符，包括严格比较操作符 <code>===</code> 和非严格的比较操作符 <code>==</code>，以及&nbsp;{{jsxref("Global_Objects/Object/is", "Object.is()")}} 方法。</dd>
</dl>

<h3 id="高级内容">高级内容</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Guide/Inheritance_and_the_prototype_chain">继承和原型的链式结构</a></dt>
 <dd>给受到普遍误解和低估的基于原型的继承做一个详细解释。</dd>
 <dt><a href="/zh-CN/docs/Web/JavaScript/Reference/Strict_mode">严格模式</a></dt>
 <dd>严格模式规定不能使用未定义的变量。严格模式是对ECMAScript 5 的严格限制，以求得更高效的性能和更便利的调试。</dd>
 <dt><a href="https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Typed_arrays">JavaScript 类型数组</a></dt>
 <dd>为使 JavaScript 处理原始二进制数据而提供的类型数组。</dd>
 <dt><a href="https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Memory_Management">内存管理</a></dt>
 <dd>JavaScript 中的内存生命周期和垃圾回收机制。</dd>
 <dt><a href="https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/EventLoop">并发模型以及事件循环</a></dt>
 <dd>JavaScript 现加入了基于“事件循环”的并发模型。</dd>
</dl>
</div>

<div class="column-half">
<h2 id="参考">参考</h2>

<p>浏览完整的&nbsp;<a href="/zh-CN/docs/Web/JavaScript/Reference">Javascript 参考</a>文档。</p>

<dl>
 <dt><a href="/zh-CN/docs/Web/JavaScript/Reference/Global_Objects">标准对象 </a></dt>
 <dd>标准的内置对象例如 {{jsxref("Array")}}, {{jsxref("Boolean")}}, {{jsxref("Date")}}, {{jsxref("Error")}}, {{jsxref("Function")}}, {{jsxref("JSON")}}, {{jsxref("Math")}}, {{jsxref("Number")}}, {{jsxref("Object")}}, {{jsxref("RegExp")}}, {{jsxref("String")}}, {{jsxref("Map")}}, {{jsxref("Set")}}, {{jsxref("WeakMap")}} , {{jsxref("WeakSet")}}&nbsp;以及其他对象</dd>
 <dt><a href="/zh-CN/docs/Web/JavaScript/Reference/Operators">表达式和运算符</a></dt>
 <dd>运算符的作用：{{jsxref("Operators/instanceof", "instanceof")}}, {{jsxref("Operators/typeof", "typeof")}}, {{jsxref("Operators/new", "new")}}, {{jsxref("Operators/this", "this")}}，<a href="/zh-CN/docs/Web/JavaScript/Reference/Operators/Operator_Precedence">运算符优先级</a>，以及其他运算符。</dd>
 <dt><a href="/zh-CN/docs/Web/JavaScript/Reference/Statements">语句和声明</a></dt>
 <dd>了解 {{jsxref("Statements/do...while", "do-while")}}, {{jsxref("Statements/for...in", "for-in")}}, {{jsxref("Statements/for...of", "for-of")}}, {{jsxref("Statements/try...catch", "try-catch")}}, {{jsxref("Statements/let", "let")}}, {{jsxref("Statements/var", "var")}}, {{jsxref("Statements/const", "const")}}, {{jsxref("Statements/if...else", "if-else")}}, {{jsxref("Statements/switch", "switch")}} 以及其他语句和关键字的作用。</dd>
 <dt><a href="https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Functions">函数</a></dt>
 <dd>学习如何使用 JavaScript 函数来开发你的应用。</dd>
</dl>

<h2 id="工具和资源">工具和资源</h2>

<p>有助于您编写和调试 JavaScript 代码的有用工具。</p>

<dl>
 <dt><a href="https://developer.mozilla.org/zh-CN/docs/Tools">Firefox 开发工具</a></dt>
 <dd>包括 <a href="/zh-CN/docs/Tools/Scratchpad">Scratchpad</a>, <a href="/zh-CN/docs/Tools/Web_Console">Web Console</a>, <a href="/zh-CN/docs/Tools/Profiler">JavaScript Profiler</a>, <a href="/zh-CN/docs/Tools/Debugger">Debugger</a> 等等</dd>
 <dt><a href="https://developer.mozilla.org/zh-CN/docs/JavaScript/shells">JavaScript Shells</a></dt>
 <dd>允许您快速测试 JavaScript 代码片段的运行环境。</dd>
 <dt><a href="https://togetherjs.com/">TogetherJS</a></dt>
 <dd>
 <p class="hero-header-text large">添加 TogetherJS 到您的网站，让用户实时互助，协作更简单。</p>
 </dd>
 <dt><a href="https://stackoverflow.com/questions/tagged/javascript">Stack Overflow</a></dt>
 <dd>StackOverflow 上的 JavaScript 问答。</dd>
 <dt><a href="/zh-CN/docs/Web/JavaScript/New_in_JavaScript">JavaScript版本和发行记录</a></dt>
 <dd>浏览 JavaScript的历史版本特性和实现情况.</dd>
 <dt><a href="https://jsfiddle.net/">JSFiddle</a></dt>
 <dd>编辑 JavaScript, CSS, HTML 并获得实时结果。使用外置资源，并和你的团队在线合作。</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/JavaScript_templates">JavaScript&nbsp;模版</a></dt>
 <dd>这个页面提供了一个 JavaScript 模版系统的列表</dd>
 <dt><a href="https://plnkr.co/">Plunker</a></dt>
 <dd>Plunker是一个在线社区，用于创建，协作和共享您的Web开发创意。编你您的JavaScript，CSS，HTML文件并获取实时结果和文件结构。</dd>
</dl>
</div>
</div>

<p>{{CommunityBox("JavaScript", "js-engine.internals", "mozilla.dev.tech.js-engine.internals", "js", "ES讨论|https://esdiscuss.org/|esdiscuss.org|ECMAScript标准探讨邮件列表||SpiderMonkey|https://wiki.mozilla.org/JavaScript|项目主页|助力JavaScript引擎||Twitter|https://twitter.com/SpiderMonkeyJS|@SpiderMonkeyJS|SpiderMonkey updates on Twitter")}}</p>

