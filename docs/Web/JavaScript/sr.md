---
version: prototype1
revision_id: 1252567
locale: sr
slug: Web/JavaScript
tags: 
title: Јаваскрипт
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{JsSidebar}}</div>

<p class="summary"><strong>Јаваскрипт (ЈС) је лак, интерпретиран или&nbsp;<em> JIT</em> - компајлиран програмски језик са </strong>{{Glossary("First-class Function", "функцијама првог реда")}}. Иако је добро познат као скрипт језик веб страница,&nbsp; <a class="external" href="https://en.wikipedia.org/wiki/JavaScript#Uses_outside_Web_pages">користи се и у другим програмским окружењима</a>, као што су&nbsp; <a class="external" href="https://nodejs.org/">node.js</a> и&nbsp;<a href="https://couchdb.apache.org/">Apache CouchDB</a>.&nbsp;Јаваскрипт је &nbsp;{{Glossary("Prototype-based programming", "базиран на прототиповима")}}, мулти-парадигматични језик с динамичном типизацијом&nbsp;који подржава објектно-оријентисани, процедурални&nbsp;и декларативни&nbsp;(нпр. фунционални) стил програмирања. Прочитај више <a href="/en-US/docs/Web/JavaScript/About_JavaScript">о Јаваскрипту</a>.</p>

<p>&nbsp;</p>

<p>Овај део је посвећена самом Јаваскрипту, као програмском језику, а не деловима који су специфични за веб странице или друга окружења.<br />
 За информације о {{Glossary("API","APIs")}} које се тичу веб страница, посетите <a href="/en-US/docs/Web/API">Web APIs</a> и <a href="/en-US/docs/Glossary/DOM">DOM</a>.</p>

<p>Јаваскрипт стандард је <a href="/en-US/docs/Web/JavaScript/Language_Resources">ECMAScript</a>. Почев од 2012, сви <a href="https://kangax.github.io/compat-table/es5/">модерни веб претраживачи</a> у потпуности подржавају ECMAScript 5.1. Старији претраживачи подржавају најмање ECMAScript 3. <a href="https://www.ecma-international.org">ECMA International</a> је 17. јуна 2015. је објавила шесту верзију&nbsp; ECMAScript-а која је званично названа ECMAScript 2015, и иницијално се говорило о њој као&nbsp; ECMAScript 6 или ES6. Од тада,&nbsp; ECMAScript стандарди се објављују једном годишње. Ова документација се односи на последњу верзију у припреми, што је тренутно <a href="https://tc39.github.io/ecma262/">ECMAScript 2018</a>.</p>

<p>Не мешајте Јаваскрипт са <a href="https://en.wikipedia.org/wiki/Java_(programming_language)">програмским језиком Јава</a>. И "Јава" и "Јаваскрипт" су заштитни знаци или заштићени заштитни знаци компаније Оракл у САД и другим земљама. Ипак, ова два програмска језика имају веома различиту синтаксу, семантику и примену.</p>

<div class="column-container">
<div class="column-half">
<h2 id="Туторијали">Туторијали</h2>

<p>Научите да програмирате у Јаваскрипту с нашим водичима и туторијалима.</p>

<h3 id="За_комплетне_почетнике">За комплетне почетнике</h3>

<p>Идите на нашу <a href="/sr/docs/Learn/JavaScript">Learning Area JavaScript topic</a> ако желите да учите Јаваскрипт а немате претходног искуства у Јаваскрипту или у програмирању. Комплетна поглавља доступна тамо су:</p>

<dl>
 <dt><a href="/sr/docs/Learn/JavaScript/First_steps">Први кораци у Јаваскрипту</a></dt>
 <dd>Одговора на нека основна питања као што су "шта је Јаваскрипт?", "како изгледа?" и "шта може да уради?". Такође, даје објашњења о кључним особинама Јаваскрипта као што су променљиве, стрингови, бројеви и низови.</dd>
 <dt><a href="/en-US/docs/Learn/JavaScript/Building_blocks">Структурни блокови Јаваскрипта</a></dt>
 <dd>Наставља наше изучавање кључних особина Јаваскрипта, скреће пажњу на најчешће коришћене типове блокова кода као што су условни изрази, петље, функције и догађаји.</dd>
 <dt><a href="/en-US/docs/Learn/JavaScript/Objects">Увод у објекте Јаваскрипта</a></dt>
 <dd>Објектно оријентисана природа јаваскрипта је важна за разумевање ако желите да проширите знање језика и да пишете ефикаснији код, зато имамо ово поглавље да вам помогне у том циљу.</dd>
</dl>

<h3 id="Јаваскрипт_водич">Јаваскрипт водич</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide">Јаваскрипт водич</a></dt>
 <dd>Детаљнији водич у Јаваскрипт, за оне који имају претходно програмерско искуство било у Јаваскрипту или неком другом језику.</dd>
</dl>

<h3 id="Средњи_ниво">Средњи ниво</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript">Поновни увод у Јаваскрипт</a></dt>
 <dd>Преглед за оне који <em>мисле</em>да знају Јаваскрипт.</dd>
</dl>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures">Структуре података у Јаваскрипту</a></dt>
 <dd>Преглед доступних стуктура података у Јаваскрипту.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness">Поређење једнакости и једнакост</a></dt>
 <dd>Јаваскрипт обезбеђује три различита оператора&nbsp; за поређење вредности: строга једнакост користи <code>===</code>, мање строга једнакост <code>==</code>, и {{jsxref("Global_Objects/Object/is", "Object.is()")}} method.</dd>
</dl>

<h3 id="Напредно">Напредно</h3>

<dl>
 <dt><a href="/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain">Наслеђивање и ланац прототипова</a></dt>
 <dd>Објашњење погрешно схваћеног и потцењеног&nbsp; наслеђивања заснованог на прототиповима.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Strict_mode">Строги режим или "use strict"</a></dt>
 <dd>Строги режим каже да не можете користити ниједну променљиву пре него је иницијализујете. То је ограничена варијанта стандарда ECMAScript&nbsp;5, за боље перформансе и лакше дебаговање.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Typed_arrays">JavaScript typed arrays</a></dt>
 <dd>JavaScript typed arrays provide a mechanism for accessing raw binary data.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Memory_Management">Управљање меморијом</a></dt>
 <dd>Животни циклус меморије и сакупљање смећа у Јаваскрипту.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/EventLoop">Паралелизам и догађаји</a></dt>
 <dd>Јаваскрипт има модел паралелизма заснован на "петљи догађаја".</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Референца">Референца</h2>

<p>Претражите комплетну <a href="/en-US/docs/Web/JavaScript/Reference">JavaScript reference</a> документацију.</p>

<dl>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects">Стандардни објекти</a></dt>
 <dd>Упознајте стандардне уграђене објекте {{jsxref("Array")}}, {{jsxref("Boolean")}}, {{jsxref("Date")}}, {{jsxref("Error")}}, {{jsxref("Function")}}, {{jsxref("JSON")}}, {{jsxref("Math")}}, {{jsxref("Number")}}, {{jsxref("Object")}}, {{jsxref("RegExp")}}, {{jsxref("String")}}, {{jsxref("Map")}}, {{jsxref("Set")}}, {{jsxref("WeakMap")}}, {{jsxref("WeakSet")}}, и друге.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Operators">Изрази и оператори</a></dt>
 <dd>Научите више о понашању оператора у Јаваскрипту{{jsxref("Operators/instanceof", "instanceof")}}, {{jsxref("Operators/typeof", "typeof")}}, {{jsxref("Operators/new", "new")}}, {{jsxref("Operators/this", "this")}}, <a href="/en-US/docs/Web/JavaScript/Reference/Operators/Operator_Precedence">приоритет оператора</a>, и више.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Statements">Наредбе и декларације</a></dt>
 <dd>Научите како да {{jsxref("Statements/do...while", "do-while")}}, {{jsxref("Statements/for...in", "for-in")}}, {{jsxref("Statements/for...of", "for-of")}}, {{jsxref("Statements/try...catch", "try-catch")}}, {{jsxref("Statements/let", "let")}}, {{jsxref("Statements/var", "var")}}, {{jsxref("Statements/const", "const")}}, {{jsxref("Statements/if...else", "if-else")}}, {{jsxref("Statements/switch", "switch")}}, и још више наредби у Јаваскрипту и кључних речи.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Functions">Функције</a></dt>
 <dd>Научите како да радећи са функцијама у Јаваскрипту направите ваше апликације.</dd>
</dl>

<h2 id="Алатке_и_ресурси">Алатке и ресурси</h2>

<p>Корисне алатке за писање и дебаговање вашег кода у Јаваскрипту.</p>

<dl>
 <dt><a href="/en-US/docs/Tools">Firefox Developer Tools</a></dt>
 <dd><a href="/en-US/docs/Tools/Scratchpad">Scratchpad</a>, <a href="/en-US/docs/Tools/Web_Console">Web Console</a>, <a href="/en-US/docs/Tools/Profiler">JavaScript Profiler</a>, <a href="/en-US/docs/Tools/Debugger">Debugger</a>, и други.</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Shells">Јаваскрипт љуска - шел (Shell)</a></dt>
 <dd>Јаваскрипт шел вам омогућава да брзо проверите делове Јаваскрипт кода.</dd>
 <dt><a href="https://togetherjs.com/">TogetherJS</a></dt>
 <dd>Колаборацију чини лаком. Додавањем TogetherJS вашем сајту, корисници могу помоћи једни другима на веб сајту у реалном времену!</dd>
 <dt><a href="https://stackoverflow.com/questions/tagged/javascript">Stack Overflow</a></dt>
 <dd>Stack Overflow питања тагована са "JavaScript".</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/New_in_JavaScript">Верзије Јаваскрипта и белешке објава (release)</a></dt>
 <dd>Претражите историју карактеристика Јаваскрипта и њихов статус имплементације.</dd>
 <dt><a href="https://jsfiddle.net/">JSFiddle</a></dt>
 <dd>Мењајте JavaScript, CSS, HTML и видите резултате уживо. Користите онлајн ресурсе и сарађујте с вашим тимом.</dd>
</dl>
</div>
</div>

<p>{{CommunityBox("JavaScript", "dev-tech-js-engine-internals", "mozilla.dev.tech.js-engine.internals", "js", "ES discuss|https://esdiscuss.org/|esdiscuss.org|ECMAScript standard discussion mailing list||SpiderMonkey|https://wiki.mozilla.org/JavaScript|Project page|Contribute to the JavaScript Engine||Twitter|https://twitter.com/SpiderMonkeyJS|@SpiderMonkeyJS|SpiderMonkey updates on Twitter")}}</p>

<div class="s3gt_translate_tooltip" id="s3gt_translate_tooltip" is_mini="true" style="position: absolute; left: 23px; top: 1491px; opacity: 0;">
<div class="s3gt_translate_tooltip_mini" id="s3gt_translate_tooltip_mini_logo" title="Translate selected text">&nbsp;</div>

<div class="s3gt_translate_tooltip_mini" id="s3gt_translate_tooltip_mini_sound" title="Play" title_play="Play" title_stop="Stop">&nbsp;</div>

<div class="s3gt_translate_tooltip_mini" id="s3gt_translate_tooltip_mini_copy" title="Copy text to Clipboard">&nbsp;</div>
</div>

