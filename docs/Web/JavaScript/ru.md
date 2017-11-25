---
version: prototype1
revision_id: 1330150
locale: ru
slug: Web/JavaScript
tags: "Intro" "Learn" "Interface" "JavaScript" "l10n:exclude" "l10n:priority" "Intermediate" "Все_категории" "Infrastructure" "Internationalization"
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
<p><strong>JavaScript</strong><sup>®</sup> (часто просто <strong>JS</strong>) — это легкий, интерпретируемый или JIT-компилируемый, объектно-ориентированный язык с {{Glossary("First-class_Function", "функциями первого класса")}}. Наиболее широкое применение находит как язык сценариев веб-страниц, но также <a href="http://en.wikipedia.org/wiki/JavaScript#Uses_outside_web_pages">используется и в других программных продуктах</a>, например, <a href="http://nodejs.org" title="http://nodejs.org">node.js</a> или <a href="http://couchdb.apache.org" title="http://couchdb.apache.org">Apache CouchDB</a>. JavaScript это {{Glossary("Prototype-based_programming", "прототипно-ориентированный")}}, мультипарадигменный язык с динамической типизацией, который поддерживает объектно-ориентированный, императивный и декларативный (например, функциональное программирование) стили программирования. Подробнее <a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/%D0%9E_JavaScript">о JavaScript</a>.</p>
</div>

<p>Эта часть сайта посвящена самому языку JavaScript, и она не затрагивает тонкостей, связанных с веб-страницами или окружением, в котором исполняется JavaScript. Информация об {{Glossary("API")}}, относящихся к веб-страницам, находится в разделах, посвященных <a href="/ru/docs/Web/API">Веб-API</a> и <a href="/ru/docs/DOM">DOM</a>.</p>

<p>Стандартом языка JavaScript является <a href="https://developer.mozilla.org/ru/docs/JavaScript/Language_Resources" title="ECMAScript">ECMAScript</a>. По состоянию на 2012, все современные браузеры полностью поддерживают ECMAScript 5.1. Старые версии браузеров поддерживают по крайней мере - ECMAScript 3. 17 июня 2015 года состоялся выпуск шестой версии ECMAScript. Эта версия официально называется ECMAScript 2015, которую чаще всего называют ECMAScript 2015 или просто ES2015. С недавнего времени стандарты ECMAScript выпускаются ежегодно. Эта документация относится к последней версии черновика, которой является <a href="http://tc39.github.io/ecma262/">ECMAScript 2018</a>.</p>

<p>Не следует путать JavaScript c <a href="https://ru.wikipedia.org/wiki/Java">языком программирования Java</a>. И "Java", и "JavaScript" являются торговыми марками или зарегистрированными торговыми марками Oracle в США и других странах. Однако, у обоих языков различный синтаксис, семантика и применение.</p>

<div class="column-container">
<div class="column-half">
<h2 class="Documentation" id="Учебные_материалы">Учебные материалы</h2>

<p>Научитесь программировать на JavaScript вместе с нами.</p>

<h3 id="Для_абсолютных_новичков">Для абсолютных новичков</h3>

<p>Загляните в наш <a href="/ru/docs/Learn/JavaScript">Учебный План,</a> если вам&nbsp;хочется&nbsp;изучить JavaScript, но у вас нет опыта в JavaScript или программировании. &nbsp;Доступные разделы:&nbsp;</p>

<dl>
 <dt><a href="/ru/docs/Web/JavaScript/Guide">Первые шаги в JavaScript</a></dt>
 <dd>Отвечаем на такие вопросы, как "что такое JavaScript?", "как он выглядит?", "и что он может делать?", а также обсуждаем основные возможности&nbsp;JavaScript, такие, как переменнные, строки, числа и массивы.</dd>
 <dt><a href="/ru/docs/Learn/JavaScript/Building_blocks">Структурные элементы JavaScript</a></dt>
 <dd>Продолжаем наше изучение главных возможностей JavaScript, обращаем наше внимание на самые часто встречающиеся блоки кода, такие, как условные выражения, циклы, функции и события.</dd>
 <dt><a href="/ru/docs/Web/JavaScript/Introduction_to_Object-Oriented_JavaScript">Введение в объектно-ориентированный JavaScript</a></dt>
 <dd>Если Вы собираетесь и дальше изучать этот язык программирования, а также писать более эффективный код, то очень важно понимать объектно-ориентированные возможности JavaScript, поэтому мы предоставили этот раздел вам в помощь.</dd>
</dl>

<h3 id="Руководство_по_JavaScript">Руководство по JavaScript</h3>

<dl>
 <dt><a href="/ru/docs/Web/JavaScript/Guide">Руководство по JavaScript</a></dt>
 <dd>Более подробное руководство по языку программирования JavaScript, нацеленное на тех, кто уже имеет опыт программирования&nbsp;в JavaScript или любом другом языке.</dd>
</dl>

<h3 id="Средний_уровень">Средний уровень</h3>

<dl>
 <dt>&nbsp;</dt>
 <dt><a href="https://developer.mozilla.org/ru/docs/Learn/JavaScript/%D0%9E%D0%B1%D1%8A%D0%B5%D0%BA%D1%82%D1%8B">Введение в объекты JavaScript</a></dt>
 <dd>Объектно-ориентированная природа JavaScript важна для понимания, если вы хотите углубить знание языка и писать более эффективный код. Поэтому мы подготовили модуль, который поможет вам в этом.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs">Клиентские&nbsp;(браузерные)&nbsp;веб-API</a></dt>
 <dd>Когда вы пишите клиент веб-сайтов или приложений&nbsp;на JavaScript, вы не далеко уйдете без использования API - интерфейсов для взаимодействия с браузером и операционной системой, на который запущен сайт, или даже для операций с данными, полученными от других веб-сайтов и сервисов.&nbsp;В этом&nbsp;цикле статей мы разбираемся, что такое API и как использовать некоторые самые распространенные API, которые вам&nbsp;встречаетются при разработке.&nbsp;</dd>
 <dt><a href="/ru/docs/Web/JavaScript/A_re-introduction_to_JavaScript">Повторное введение в JavaScript</a></dt>
 <dd>Обзор для тех, кто <em>думает</em>, что знает JavaScript.</dd>
 <dt><a href="/ru/docs/Web/JavaScript/Data_structures">Структуры данных JavaScript</a></dt>
 <dd>Обзор существующих структур данных в JavaScript.</dd>
 <dt><a href="/ru/docs/Web/JavaScript/Equality_comparisons_and_sameness">Операторы сравнения и тождественности</a></dt>
 <dd>JavaScript предоставляет три различных оператора сравнения значений: строгое равенство <code>===</code>, с приведением типов <code>==</code> и метод {{jsxref("Global_Objects/Object/is", "Object.is()")}}.</dd>
</dl>

<h3 id="Продвинутый_уровень">Продвинутый уровень</h3>

<dl>
 <dt><a href="/ru/docs/Web/JavaScript/Guide/Inheritance_and_the_prototype_chain">Наследование и цепочка прототипов</a></dt>
 <dd>Статья разъясняет бытующие заблуждения и недооцененность наследования, основанного на прототипах.</dd>
 <dt><a href="/ru/docs/Web/JavaScript/Reference/Strict_mode">Строгий режим или "use strict"</a></dt>
 <dd>Строгий режим говорит, что вы не можете использовать какую-либо переменную до её объявления. Это ограниченный вариант ECMAScript 5, для более быстрой производительности и простой отладки.</dd>
 <dt><a href="/ru/docs/Web/JavaScript/Typed_arrays">Типизированные массивы</a></dt>
 <dd>Типизированные массивы предоставляют механизм для работы с необработанными двоичными данными в JavaScript.</dd>
 <dt><a href="/ru/docs/Web/JavaScript/Memory_Management">Управление памятью</a></dt>
 <dd>Жизненный цикл памяти и сборка мусора в JavaScript.</dd>
 <dt><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/EventLoop">Модель параллелизма (мультипоточности) и цикл событий</a></dt>
 <dd>В JavaScript есть модель параллелизма, основанная на "цикле событий".</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Introduction_to_using_XPath_in_JavaScript">Введение в использование&nbsp;XPath в&nbsp;JavaScript</a></dt>
 <dd>Этот документ описывает интерфейс для использования <a href="https://developer.mozilla.org/en-US/docs/XPath" title="en/XPath">XPath</a>&nbsp;в&nbsp;JavaScript - internally, in extensions, and from websites.</dd>
</dl>
</div>

<div class="column-half">
<h2 class="Tools" id="Справочник">Справочник</h2>

<p>Подробный <a href="/ru/docs/Web/JavaScript/Reference">справочник</a> по JavaScript.</p>

<dl>
 <dt><a href="/ru/docs/Web/JavaScript/Reference/Global_Objects">Стандартные встроенные объекты</a></dt>
 <dd>Узнайте о стандартных встроенных объектах {{jsxref("Array")}}, {{jsxref("Boolean")}}, {{jsxref("Date")}}, {{jsxref("Error")}}, {{jsxref("Function")}}, {{jsxref("JSON")}}, {{jsxref("Math")}}, {{jsxref("Number")}}, {{jsxref("Object")}}, {{jsxref("RegExp")}}, {{jsxref("String")}}, {{jsxref("Map")}}, {{jsxref("Set")}}, {{jsxref("WeakMap")}} , {{jsxref("WeakSet")}} и других.</dd>
 <dt><a href="/ru/docs/Web/JavaScript/Reference/Operators">Выражения и операторы</a></dt>
 <dd>Узнайте о поведении таких операторов в JavaScript, как {{jsxref("Operators/instanceof", "instanceof")}}, {{jsxref("Operators/typeof", "typeof")}}, {{jsxref("Operators/new", "new")}}, {{jsxref("Operators/this", "this")}}, <a href="/ru/docs/Web/JavaScript/Reference/Operators/Operator_Precedence">приоритете операторов</a> и многом другом.</dd>
 <dt><a href="/ru/docs/Web/JavaScript/Reference/Statements">Инструкции и объявления</a></dt>
 <dd>Узнайте о {{jsxref("Statements/do...while", "do-while")}}, {{jsxref("Statements/for...in", "for-in")}}, {{jsxref("Statements/for...of", "for-of")}}, {{jsxref("Statements/try...catch", "try-catch")}}, {{jsxref("Statements/let", "let")}}, {{jsxref("Statements/var", "var")}}, {{jsxref("Statements/const", "const")}}, {{jsxref("Statements/if...else", "if-else")}}, {{jsxref("Statements/switch", "switch")}} и многих других выражениях и ключевых словах в JavaScript.</dd>
 <dt><a href="/ru/docs/Web/JavaScript/Reference/Functions">Функции</a></dt>
 <dd>Узнайте, как работать с функциями в JavaScript, чтобы разрабатывать свои приложения.</dd>
</dl>

<h2 class="Tools" id="Инструменты_и_дополнительные_ресурсы">Инструменты и дополнительные ресурсы</h2>

<p>Полезные инструменты для написания и отладки вашего <strong>JavaScript </strong>кода.</p>

<dl>
 <dt><a href="/ru/docs/Tools">Инструменты разработчика Firefox</a></dt>
 <dd><a href="/ru/docs/Tools/Черновик">Простой редактор JavaScript</a>, <a href="/ru/docs/Tools/Web_Console">Веб-консоль</a>, <a href="/ru/docs/Tools/Profiler">JavaScript Профайлер</a>, <a href="/ru/docs/Tools/Debugger">Отладчик</a> и другие.</dd>
 <dt><a href="http://www.getfirebug.com/">Firebug</a></dt>
 <dd>Редактируйте, отлаживайте и проверяйте CSS, HTML и JavaScript вживую на любой странице.</dd>
 <dt><a href="/ru/docs/Web/JavaScript/JavaScript_шеллы">JavaScript шеллы</a></dt>
 <dd>JavaScript шеллы позволяют быстро проверять фрагменты JavaScript кода.</dd>
 <dt><a href="https://togetherjs.com/">TogetherJS</a></dt>
 <dd>Объединение усилий стало проще.</dd>
 <dt><a href="http://stackoverflow.com/questions/tagged/javascript">Stack Overflow</a></dt>
 <dd>Вопросы по JavaScript на Stack Overflow.</dd>
 <dt><a href="/ru/docs/Web/JavaScript/New_in_JavaScript">Версии JavaScript и информация о релизах</a></dt>
 <dd>Просмотрите историю возможностей JavaScript и их статус.</dd>
 <dt><a href="https://jsfiddle.net/">JSFiddle</a></dt>
 <dd>Редактируйте JavaScript, CSS, HTML и получайте живые результаты. Используйте экспериментальные ресурсы и взаимодействуйте с вашей командой онлайн.</dd>
</dl>

<dl>
 <dt><a href="https://plnkr.co/">Plunker</a></dt>
 <dd>Plunker - это онлайн-сообщество для создания, обмена и совместной работы над идеями, касающимися&nbsp;веб-разработки. Редактируйте ваши JavaScript, CSS, HTML файлы, смотрите результат&nbsp;их выполнения и организуйте их в файловую структуру.</dd>
</dl>

<p>&nbsp;</p>
</div>
</div>

<p>{{CommunityBox("JavaScript", "js-engine.internals", "mozilla.dev.tech.js-engine.internals", "js", "ES discuss|https://esdiscuss.org/|esdiscuss.org|Рассылка об обсуждении стандарта ECMAScript||SpiderMonkey|https://wiki.mozilla.org/JavaScript|Страница проекта|Внести вклад в JavaScript движок||Твиттер|https://twitter.com/SpiderMonkeyJS|@SpiderMonkeyJS|Обновления SpiderMonkey на Твиттере")}}</p>

