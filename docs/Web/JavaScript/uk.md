---
version: prototype1
revision_id: 1300099
locale: uk
slug: Web/JavaScript
tags: "Мова" "Вчити" "Посібник" "JavaScript"
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

<p class="summary">JavaScript (JS) — це невибаглива до ресурсів мова програмування з {{Glossary("First-class Function", "функціями першого класу")}}, код якої інтерпретується або компілюється під час виконання. Хоча JavaScript насамперед відома як скриптова мова для веб-сторінок, вона також використовується у <a href="https://en.wikipedia.org/wiki/JavaScript#Uses_outside_Web_pages">багатьох небраузерних середовищах</a> на кшталт <a href="https://nodejs.org/">node.js</a>, <a href="https://couchdb.apache.org/">Apache CouchDB</a> та <a href="http://www.adobe.com/devnet/acrobat/javascript.html">Adobe Acrobat</a>. JavaScript — {{Glossary("Prototype-based programming", "прототип-орієнтована")}} {{glossary("Dynamic_programming_language", "динамічна мова")}}, що має декілька парадигм та підтримує {{glossary("OOP", "об'єктно-орієнтований")}}, <a href="https://uk.wikipedia.org/wiki/%D0%86%D0%BC%D0%BF%D0%B5%D1%80%D0%B0%D1%82%D0%B8%D0%B2%D0%BD%D0%B5_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D1%83%D0%B2%D0%B0%D0%BD%D0%BD%D1%8F">імперативний</a> та <a href="https://uk.wikipedia.org/wiki/%D0%94%D0%B5%D0%BA%D0%BB%D0%B0%D1%80%D0%B0%D1%82%D0%B8%D0%B2%D0%BD%D0%B5_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D1%83%D0%B2%D0%B0%D0%BD%D0%BD%D1%8F">декларативний</a> (тобто <a href="https://uk.wikipedia.org/wiki/%D0%A4%D1%83%D0%BD%D0%BA%D1%86%D1%96%D0%B9%D0%BD%D0%B5_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D1%83%D0%B2%D0%B0%D0%BD%D0%BD%D1%8F">функціональне програмування</a>) стилі. Розгорнуте визначення та докладний опис JavaScript <a href="/uk/docs/Learn/JavaScript">читайте за посиланням</a>.</p>

<p><span id="result_box" lang="uk">Ця частина сайту присвячена безпосередньо <span class="alt-edited">мові</span> <span>JavaScript</span><span>,</span> <span>і</span> <span>вона не</span> <span class="alt-edited">стосується</span> <span>тонкощів</span><span>,</span> <span>пов'язаних</span> <span>з</span> <span>веб</span><span>-</span><span>сторінками</span> <span>чи іншим</span>&nbsp;<span>оточенням</span><span>,</span> <span>у</span> <span>якому</span> <span class="alt-edited">виконується</span> <span>JavaScript</span></span>. Специфічну інформацію&nbsp;щодо {{Glossary("API","API")}} для&nbsp;<span class="short_text" id="result_box" lang="uk"><span>Веб</span><span>-</span><span>сторінок</span></span>&nbsp;дивіться, будь ласка, у підрозділах&nbsp;<a href="/uk/docs/Web/API">Web APIs</a> та <a href="/uk/docs/Glossary/DOM">DOM</a>.</p>

<p>Стандартом для JavaScript є <a href="/uk/docs/Web/JavaScript/Language_Resources">ECMAScript</a>. <span class="short_text" id="result_box" lang="uk"><span>Станом</span> <span>на 2012 рік</span></span>&nbsp;усі <a href="http://kangax.github.io/compat-table/es5/">сучасні браузери</a>&nbsp;вже мали повну підтримку&nbsp;ECMAScript 5.1. Застарілі браузери підтримують щонайменше ECMAScript 3. 17 <span class="short_text" lang="uk"><span>червня</span></span>&nbsp;2015 року&nbsp;<a href="http://www.ecma-international.org">ECMA International </a>випустилала шосту базову версію ECMAScript&nbsp;з&nbsp;офіційною&nbsp;назвою&nbsp;ECMAScript 2015, яка у попередніх обговореннях йменувалася ECMAScript 6 або ES6. Відтоді стандарти&nbsp;ECMAScript оновлюються раз на рік.&nbsp;Ця документація посилається на найсвіжішу версію чернетки, тобто&nbsp;<a href="http://tc39.github.io/ecma262/">ECMAScript 2017</a>&nbsp;на цей час.</p>

<p><span class="short_text" id="result_box" lang="uk"><span>Не варто&nbsp;</span><span>плутати</span></span> JavaScript з <a href="https://en.wikipedia.org/wiki/Java_(programming_language)">мовою програмування Java</a>. Обидві мови "Java" та "JavaScript" є товарними знаками чи&nbsp;<span class="short_text" id="result_box" lang="uk"><span>зареєстрованими</span> <span>торговими</span> <span>марками</span></span> Oracle у&nbsp;<span class="short_text" id="result_box" lang="uk"><span>Сполучених Штатах</span></span> та інших крїнах. <span id="result_box" lang="uk"><span>Проте</span> <span>ці</span> <span>дві мови</span> <span>програмування</span> <span>мають</span>&nbsp;великі розбіжності у&nbsp;<span>синтаксисі</span><span>,</span> <span>семантиці&nbsp;</span><span>та&nbsp;</span><span>застосуванні</span><span>.</span></span></p>

<div class="column-container">
<div class="column-half">
<h2 id="Навчальні_посібники">Навчальні посібники</h2>

<p>Навчайтесь&nbsp;програмуванню&nbsp;на&nbsp;JavaScript&nbsp;за допомогою путівників та&nbsp;посібників.</p>

<h3 id="Для_повних_новачків">Для повних новачків</h3>

<p>Якщо ви не маєте взагалі ніякого досвіду програмування&nbsp;на JavaScript, але маєте бажання навчитись, починайте&nbsp;<a href="https://developer.mozilla.org/uk-UA/docs/Learn/JavaScript">з підрозділу JavaScript у нашому&nbsp;Просторі&nbsp;навчальних матеріалів</a>. Цей підрозділ складається з наступних лекцій:</p>

<dl>
 <dt><a href="https://developer.mozilla.org/uk/docs/Web/JavaScript/Guide">Перші кроки&nbsp;з JavaScript</a></dt>
 <dd>Відповіді на деякі фундаментальні питання на кшталт "JavaScript —&nbsp;це що?", "На що він схожий?" та "Які має можливості?"&nbsp;з оглядом ключових компонентів &nbsp;JavaScript, таких як змінні, рядки, числа та масиви.</dd>
 <dt><a href="https://developer.mozilla.org/uk/docs/Learn/JavaScript/Building_blocks">Блоки, з яких складається JavaScript</a></dt>
 <dd>Продовжуємо огляд ключових компонентів &nbsp;JavaScript, цього разу спрямовуючи&nbsp;нашу увагу на зазвичай вживані&nbsp;типові блоки коду, такі як умовні&nbsp;викази, цикли, функції&nbsp;та події.</dd>
 <dt><a href="https://developer.mozilla.org/uk/docs/Web/JavaScript/Introduction_to_Object-Oriented_JavaScript">Знайомство з об'єктами у JavaScript</a></dt>
 <dd>Якщо ви маєте бажання надалі вдосконалювати свій рівень&nbsp;знань&nbsp;мови&nbsp;та створювати більш ефективний код, важливо розумітися на об'єктно-орієнтованій природі&nbsp;&nbsp;JavaScript, і&nbsp;ця&nbsp;лекція має стати&nbsp;вам у пригоді.</dd>
</dl>

<h3 id="Путівник_з_JavaScript">Путівник з JavaScript</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/uk/docs/Web/JavaScript/Guide">Путівник з JavaScript</a></dt>
 <dd>Детальний&nbsp;путівник з JavaScript для осіб, які<br />
 вже мають досвід&nbsp;програмування на JavaScript чи іншій мові.</dd>
</dl>

<h3 id="Середній_рівень">Середній рівень</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/uk/docs/Web/JavaScript/A_re-introduction_to_JavaScript">Введення у&nbsp;JavaScript наново</a></dt>
 <dd>Огляд для осіб, які&nbsp;<em>вважають</em>, що знають&nbsp;JavaScript.</dd>
</dl>

<dl>
 <dt><a href="https://developer.mozilla.org/uk/docs/Web/JavaScript/Data_structures">Структури даних у JavaScript</a></dt>
 <dd>Огляд структур даних, наявних у&nbsp;JavaScript.</dd>
 <dt><a href="/uk/docs/Web/JavaScript/Equality_comparisons_and_sameness">Порівняння рівностей та тотожність</a></dt>
 <dd>JavaScript пропонує три шляхи для порівняння значень: строга рівність з застосуванням <code>===</code>, нестрога з <code>==</code> та метод <code>{{jsxref("Global_Objects/Object/is", "Object.is()")}}</code>.</dd>
</dl>

<h3 id="Просунутий_рівень">Просунутий рівень</h3>

<dl>
 <dt><a href="/uk/docs/Web/JavaScript/Inheritance_and_the_prototype_chain">Успадкування та ланцюг&nbsp;прототипів</a></dt>
 <dd>Розтлумачення успадкування на базі прототипів, яке здебільшого&nbsp;невірно розуміють та недооцінюють.</dd>
 <dt><a href="/uk/docs/Web/JavaScript/Reference/Strict_mode">Суворий режим</a></dt>
 <dd>Використання будь-якої&nbsp;змінної без попередньої декларації&nbsp;у&nbsp;суворому режимі заборонено. Цей&nbsp;режим&nbsp;грунтується на&nbsp;ECMAScript&nbsp;5 з низкою обмежень для поліпшення&nbsp;швидкості&nbsp;й&nbsp;стабільності та спрощення зневадження (дослідження) коду.</dd>
 <dt><a href="https://developer.mozilla.org/uk/docs/Web/JavaScript/Typed_arrays">Типізовані&nbsp;масиви у JavaScript</a></dt>
 <dd>Типізовані масиви у JavaScript надають механізм доступу до необроблених бінарних даних.</dd>
 <dt><a href="https://developer.mozilla.org/uk/docs/Web/JavaScript/Memory_Management">Керування пам'яттю</a></dt>
 <dd>Життєвий цикл пам'яті та збирання сміття у JavaScript.</dd>
 <dt><a href="/uk/docs/Web/JavaScript/EventLoop">Мультипотокова модель та Цикл подій</a></dt>
 <dd>JavaScript має мультипотокову подель, яка грунтується на "циклі подій".</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Документація">Документація</h2>

<p>Перегляньте повну документацію по&nbsp;<a href="/uk/docs/Web/JavaScript/Reference">JavaScript</a>.</p>

<dl>
 <dt><a href="/uk/docs/Web/JavaScript/Reference/Global_Objects">Стандартні об'єкти</a></dt>
 <dd>Ознайомтесь&nbsp;зі стандартними&nbsp;вбудованими&nbsp;об'єктами&nbsp;{{jsxref("Array")}}, {{jsxref("Boolean")}}, {{jsxref("Date")}}, {{jsxref("Error")}}, {{jsxref("Function")}}, {{jsxref("JSON")}}, {{jsxref("Math")}}, {{jsxref("Number")}}, {{jsxref("Object")}}, {{jsxref("RegExp")}}, {{jsxref("String")}}, {{jsxref("Map")}}, {{jsxref("Set")}}, {{jsxref("WeakMap")}} , {{jsxref("WeakSet")}} та ін.</dd>
 <dt><a href="/uk/docs/Web/JavaScript/Reference/Operators">Вирази та оператори</a></dt>
 <dd>Дізнайтесь&nbsp;більше про особливості поведінки&nbsp;у JavaScript операторів {{jsxref("Operators/instanceof", "instanceof")}}, {{jsxref("Operators/typeof", "typeof")}}, {{jsxref("Operators/new", "new")}}, {{jsxref("Operators/this", "this")}}, <a href="/uk/docs/Web/JavaScript/Reference/Operators/Operator_Precedence">пріоритети операторів</a> тощо.</dd>
 <dt><a href="/uk/docs/Web/JavaScript/Reference/Statements">Викази та декларації</a></dt>
 <dd>Усвідомте, як працюють {{jsxref("Statements/do...while", "do-while")}}, {{jsxref("Statements/for...in", "for-in")}}, {{jsxref("Statements/for...of", "for-of")}}, {{jsxref("Statements/try...catch", "try-catch")}}, {{jsxref("Statements/let", "let")}}, {{jsxref("Statements/var", "var")}}, {{jsxref("Statements/const", "const")}}, {{jsxref("Statements/if...else", "if-else")}}, {{jsxref("Statements/switch", "switch")}} та інші викази й ключовики&nbsp;JavaScript.</dd>
 <dt><a href="/uk/docs/Web/JavaScript/Reference/Functions">Функції</a></dt>
 <dd>Навчіться застосовувати функції&nbsp;JavaScript для <span class="short_text" id="result_box" lang="uk"><span>розробки</span> власних&nbsp;<span>додатків</span></span>.</dd>
</dl>

<h2 id="Інструменти_та_ресурси">Інструменти та ресурси</h2>

<p>Корисні інструменти для створення та зневадження (дослідження) вашого коду JavaScript.</p>

<dl>
 <dt><a href="/uk/docs/Tools">Інструменти розробника у&nbsp;Firefox</a></dt>
 <dd><a href="/uk/docs/Tools/Scratchpad">Блокнот</a>, <a href="/uk/docs/Tools/Web_Console">Консоль</a>,&nbsp;<a href="/uk/docs/Tools/Profiler">Профілювання&nbsp;JavaScript</a>, <a href="/uk/docs/Tools/Debugger">Зневаджувач</a>&nbsp;та ін.</dd>
 <dt><a href="/uk/docs/Web/JavaScript/Shells">Оболонки&nbsp;JavaScript</a></dt>
 <dd>Надають Вам можливіть&nbsp;швидко протестувати сніпети JavaScript.</dd>
 <dt><a href="https://togetherjs.com/">TogetherJS</a></dt>
 <dd>
 <p>Спрощують командну роботу. Додайте TogetherJS до Вашого сайту, і Ваші відвідувачі матимуть можливість&nbsp;&nbsp;допомагати одне одному у реальному часі.</p>
 </dd>
 <dt><a href="http://stackoverflow.com/questions/tagged/javascript">Stack Overflow</a></dt>
 <dd>Питання з&nbsp;тегом&nbsp;"JavaScript" на ресурсі Stack Overflow.</dd>
 <dt><a href="/uk/docs/Web/JavaScript/New_in_JavaScript">Версії JavaScript та примітки до випуску</a></dt>
 <dd>Переглядайте історію розвитку компонентів JavaScript&nbsp;та поточний статус їхньої підтримки.</dd>
 <dt><a href="https://jsfiddle.net/">JSFiddle</a></dt>
 <dd>Наживо редагуйте JavaScript, CSS й&nbsp;HTML та миттєво отримуйте&nbsp;результати. Використовуйте зовнішні ресурси та співпрацюйте з вашою&nbsp;командою онлайн.</dd>
</dl>
</div>
</div>

<p>{{CommunityBox("JavaScript", "js-engine.internals", "mozilla.dev.tech.js-engine.internals", "js", "Обговорення ES|https://esdiscuss.org/|esdiscuss.org|Поштова розсилка з обговорення стандартів ECMAScript||SpiderMonkey|https://wiki.mozilla.org/JavaScript|Сторінка проекту|Беріть участь у розвиненні движка JavaScript||Twitter|https://twitter.com/SpiderMonkeyJS|@SpiderMonkeyJS|Оновлення SpiderMonkey у Twitter")}}</p>

