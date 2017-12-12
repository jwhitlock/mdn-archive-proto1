---
version: prototype1
revision_id: 1335980
locale: pl
slug: Web/JavaScript
tags: "Nauka"
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

<p class="summary"><strong>JavaScript</strong> (<strong>JS</strong>) to skryptowy (interpretowany lub kompilowany metodą <a href="https://pl.wikipedia.org/wiki/JIT_(informatyka)">JIT</a>)&nbsp;język programowania, w którym funcje "są obywatelami pierwszej kategorii" - są obiektami, które można przechowywać w zmiennych jako referencje i przekazywać jak każde&nbsp;inne&nbsp;obiekty. Chociaż JavaScript jest najbardzej znany&nbsp;jako język skryptowy dla stron internetowych, używa go również&nbsp;<a class="external" href="https://en.wikipedia.org/wiki/JavaScript#Uses_outside_Web_pages">wiele środowisk poza przeglądarką</a>, takich jak <a class="external" href="/en-US/docs/Glossary/Node.js">Node.js</a>, <a href="https://couchdb.apache.org/">Apache CouchDB</a>&nbsp;czy <a href="http://www.adobe.com/devnet/acrobat/javascript.html">Adobe Acrobat</a>. JavaScript jest językiem opartym na prototypach, wielu paradygmatach, dynamicznej składni, zorientowany obiektowo, o <a href="https://pl.wikipedia.org/wiki/Programowanie_imperatywne">stylu imperatywnym</a> i <a href="https://pl.wikipedia.org/wiki/Programowanie_deklaratywne">deklaratywnym</a> (np. <a href="https://pl.wikipedia.org/wiki/Programowanie_funkcyjne">programowanie funkcyjne</a>).&nbsp;</p>

<p>Ta sekcja naszego serwisu jest przeznaczona samemu językowi&nbsp;JavaScript, a nie zagadnieniom związanym&nbsp;ze stronami internetowymi lub innymi środowiskami hosta. Informacje dotyczące {{Glossary("interfejsów API","Interfejsy API")}} specificzne dla stron internetowych proszę szukać w źródłachach:&nbsp;<a href="/pl/docs/Web/API">Internetowe interfesy API</a>&nbsp;i <a href="/pl/docs/Glossary/DOM">DOM</a>.</p>

<p>Standardem dla JavaScript jest <a href="/pl/docs/Web/JavaScript/Language_Resources">ECMAScript</a>. Od roku 2012, wszystkie <a href="https://kangax.github.io/compat-table/es5/">nowoczesne przegladarki</a>&nbsp;całkowicie obsługują ECMAScript 5.1. Starsze przegladarki obsługują co najmniej ECMAScript 3. 17 czerwca 2015, <a href="https://www.ecma-international.org">ECMA International</a>&nbsp;opublikował szóstą główną wersję ECMAScript, którą oficjalnie nazywa się ECMAScript 2015 ale początkowo była nazywana też ECMAScript 6 lub&nbsp;ES6. Od tego czasu, standardy ECMAScript są wydawane w cyklach rocznych. Niniejszt dokument odnosi sie do szkicu najnowszej wersji, którą obecnie jest <a href="https://tc39.github.io/ecma262/">ECMAScript 2018</a>.</p>

<p>Nie należy mylić JavaScript z <a href="https://pl.wikipedia.org/wiki/Java">językiem programowania Java</a>. Zarówno "Java" jak i "JavaScript" są znakami towarowymi lub zastrzeżonymi znakami towarowymi Oracle w U.S. i innych krajach. Jednak obydwa te języki programowania mają bardzo różną składnię, sematyke i zastosowanie.</p>

<div class="column-container">
<div class="column-half">
<h2 id="Przewodniki">Przewodniki</h2>

<p>Naucz się programować w JavaScript studiując nasze przewodniki i samouczki.</p>

<h3 id="Dla_zupełnie_początkujących">Dla zupełnie początkujących</h3>

<p>Jeśli chcesz się nauczyć JavaScript, ale nie masz doświadczenia w JavaScript lub programowaniu, przejdź do naszych <a href="/pl/docs/Learn/JavaScript">tematów w strefie nauki JavaScript</a>. Dostępne są tu następujące moduły:</p>

<dl>
 <dt><a href="/pl/docs/Learn/JavaScript/First_steps">Pierwsze kroki w JavaScript</a></dt>
 <dd>Znajdziesz tu odpowiedź na kilka podstawowych pytań, takich jak: "Co to jest JavaScript?", "Jak wygląda?" czy "Co można z nim zrobić?" oraz omówienie kluczowych elementów JavaScript, takich jak zmienne, łańcuchy, liczby i tablice.</dd>
</dl>

<p><a href="/pl/docs/Learn/JavaScript/Building_blocks">Klocki JavaScript</a></p>

<dl>
 <dd>Kontynuujemy tu opis podstawowych elementów JavaScript, zwracając uwagę na często stosowane typy bloków kodu, takie&nbsp;jak wyrażenia warunkowe, pętle, funkcje i zdarzenia.</dd>
</dl>

<h3 id="Przewodnik_JavaScript">Przewodnik JavaScript</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/pl/docs/Web/JavaScript/Guide">Przewodnik JavaScript</a></dt>
 <dd>O wiele bardziej szczegółowy poradnik JavaScript, przeznaczony dla osób z wcześniejszym doświadczeniem programistycznym w innych jezykach.</dd>
</dl>

<h3 id="Dla_średnozaawansowanych">Dla średnozaawansowanych</h3>

<dl>
 <dt><a href="/pl/docs/Learn/JavaScript/Objects">Wprowadzenie do obiektów JavaScript</a></dt>
 <dd>Jest ważne, aby zrozumieć obiektowo zorientowaną naturę JavaScript, bo to pozwoli Ci bardziej zgłebic tajniki tego języka i tworzyć w przyszłości bardziej efektywny kod. Ten moduł ma Ci w tym pomóc.</dd>
 <dt><a href="/pl/docs/Learn/JavaScript/Client-side_web_APIs">Interfejsy API po stronie klienta</a></dt>
 <dd>Jeśli chcesz pisać kod JavaScript działający po stronie klienta dla stron internetowych lub aplikacji, nie zajdziesz daleko, zanim nie zaczniesz używać stosownych interfejsów&nbsp;API — interfejsów do manipulowania róznymi aspektami i systemu operacyjnego w którym przeglądarka działa a nawet manipulowania danymi pochodzącymi z innych witryn lub serwisów internetowych. W tym podule dowiesz się, jakie są interfejsy API działające po stronie klienta i jak korzystać z najbardziej popularnych interfejsów API.&nbsp;</dd>
</dl>

<dl>
 <dt><a href="https://developer.mozilla.org/pl/docs/Web/JavaScript/A_re-introduction_to_JavaScript">Ponowne wprowadzenie do JavaScript</a></dt>
 <dd>Przegląd zagadnień związanych z JavaScript, przeznaczony dla tych, co "wiedzą wszystko".</dd>
</dl>

<dl>
 <dt>&nbsp;<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures">Struktura danych JavaScript</a></dt>
 <dd>Przegląd dostępnych w JavaScript struktur danych.</dd>
 <dt><a href="/pl/docs/Web/JavaScript/Equality_comparisons_and_sameness">Porównanie a identyczność</a></dt>
 <dd>JavaScript zapewnia trzy różne operacje porównywania wartości: ścisłą równość&nbsp;przy użyciu operatoa&nbsp;&nbsp;<code>===</code>, luźną równość przy uzyciu operatoa&nbsp;<code>==&nbsp; i metodę&nbsp;</code>{jsxref("Global_Objects/Object/is", "Object.is()")}}.</dd>
</dl>

<h3 id="Dla_zaawansowanych">Dla zaawansowanych</h3>

<dl>
 <dt><a href="/pl/docs/Web/JavaScript/Inheritance_and_the_prototype_chain">Dziedziczenie i łańcuch prototypowania</a></dt>
 <dd>Wyjaśnienie powszechnie nierozumianego i niedocenianego dziedziczenia prototypowego.</dd>
 <dt><a href="/pl/docs/Web/JavaScript/Reference/Strict_mode">Tryb&nbsp;ścisły</a></dt>
 <dd>Tryb ścisły powoduje, że nie można użyć jakichkolwiek zmiennych przed ich inicjowaniem. Jest to ścisły wariant ECMAScript&nbsp;5, zwiekszający wydajność i łatwość debugowania.</dd>
 <dt><a href="https://developer.mozilla.org/pl/docs/Web/JavaScript/Typed_arrays">Tablice typowane JavaScript</a></dt>
 <dd>Tablice typowane JavaScript dostarczają mechanizm dostępu do surowych danych binarnych.</dd>
 <dt><a href="https://developer.mozilla.org/pl/docs/Web/JavaScript/Memory_Management">Zarządzanie pamięcią</a></dt>
 <dd>Cykl życia pamięci i odśmiecanie kolekcji w&nbsp;JavaScript.</dd>
 <dt><a href="/pl/docs/Web/JavaScript/EventLoop">Model współbieżności i pętla zdarzeń</a></dt>
 <dd>JavaScript ma model współbieżny oparty na "pętli zdarzeń".</dd>
 <dt><a href="/pl/docs/Web/JavaScript/Introduction_to_using_XPath_in_JavaScript">Wprowadzenie do stosowania&nbsp;XPath w JavaScript</a></dt>
 <dd>W tym dokumencie opisano interfejs do używania w JavaScript biblioteki&nbsp;<a href="/en-US/docs/XPath" title="en/XPath">XPath</a>, w rozszerzeniach i witrynach internetowych.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Informatory">Informatory</h2>

<p>Przejrzyj kompletną dokumentację&nbsp;<a href="/en-US/docs/Web/JavaScript/Reference">informacyjną&nbsp;JavaScript </a>.</p>

<dl>
 <dt><a href="/pl/docs/Web/JavaScript/Reference/Global_Objects">Obiekty standardowe</a></dt>
 <dd>Poznaj standardowe obiekty wbudowane {{jsxref("Array")}}, {{jsxref("Boolean")}}, {{jsxref("Date")}}, {{jsxref("Error")}}, {{jsxref("Function")}}, {{jsxref("JSON")}}, {{jsxref("Math")}}, {{jsxref("Number")}}, {{jsxref("Object")}}, {{jsxref("RegExp")}}, {{jsxref("String")}}, {{jsxref("Map")}}, {{jsxref("Set")}}, {{jsxref("WeakMap")}}, {{jsxref("WeakSet")}} i inne</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/Reference/Operators">Wyrażenia i operatory</a></dt>
 <dd>Dowiedz się więcej o zachowywaniu się operatorów JavaScript {{jsxref("Operators/instanceof", "instanceof")}}, {{jsxref("Operators/typeof", "typeof")}}, {{jsxref("Operators/new", "new")}}, {{jsxref("Operators/this", "this")}}, <a href="/pl/docs/Web/JavaScript/Reference/Operators/Operator_Precedence">pierwszeństwo&nbsp;opertaorów</a>&nbsp;itd.</dd>
 <dt><a href="/pl/docs/Web/JavaScript/Reference/Statements">Instrukcje&nbsp;i deklaracje</a></dt>
 <dd>Zapoznaj się jak działają {{jsxref("Statements/do...while", "do-while")}}, {{jsxref("Statements/for...in", "for-in")}}, {{jsxref("Statements/for...of", "for-of")}}, {{jsxref("Statements/try...catch", "try-catch")}}, {{jsxref("Statements/let", "let")}}, {{jsxref("Statements/var", "var")}}, {{jsxref("Statements/const", "const")}}, {{jsxref("Statements/if...else", "if-else")}}, {{jsxref("Statements/switch", "switch")}} i inne instrukcje i słowa kluczowe JavaScript.</dd>
 <dt><a href="/pl/docs/Web/JavaScript/Reference/Functions">Funkcje</a></dt>
 <dd>Dowiedz się jak pracować z funkcjami JavaScript przy tworzeniu swoich aplikacji.</dd>
</dl>

<h2 id="Narzędzia_i_zasoby">Narzędzia i zasoby</h2>

<p>Przydatne narzędzia do pisania i debugowani kodu <strong>JavaScript</strong>.</p>

<dl>
 <dt><a href="/pl/docs/Tools">Narzędzia programistyczne Firefox</a></dt>
 <dd><a href="/pl/docs/Tools/Scratchpad">Scratchpad</a>, <a href="/pl/docs/Tools/Web_Console">Web Console</a>, <a href="/pl/docs/Tools/Profiler">JavaScript Profiler</a>, <a href="/pl/docs/Tools/Debugger">Debugger</a>&nbsp;itd.</dd>
 <dt><a href="/pl/docs/Web/JavaScript/Shells">Powłoki JavaScript</a></dt>
 <dd>Powłoka JavaScript (konsola linii poleceń) pozwala szybko przetestować fragmenty kodu JavaScript.</dd>
 <dt><a href="https://togetherjs.com/">TogetherJS</a></dt>
 <dd>Ułatwia współpracę. Dodając TogetherJS do swojej witryny, można wpomóc współpracę, poprzez wzajemną komunikację uzytkowników w czasie rzeczywistym.</dd>
 <dt><a href="https://stackoverflow.com/questions/tagged/javascript">Stack Overflow</a></dt>
 <dd>Oznaczanie zapytań dotyczących przepełnienia stosu tagiem "JavaScript".</dd>
 <dt><a href="/en-US/docs/Web/JavaScript/New_in_JavaScript">Wersje JavaScript i uwagi do wydań</a></dt>
 <dd>Przeglądaj historię wydań JavaScript i stan implementacji.</dd>
 <dt><a href="https://jsfiddle.net/">JSFiddle</a></dt>
 <dd>Edytowanie JavaScript, CSS i HTML z z natychmiastowym podglądem wyników. Pozwala na używanie zasobów zewnętrznych i pracę zespołową.</dd>
 <dt><a href="/pl/docs/Web/JavaScript/JavaScript_templates">Szablony JavaScript</a></dt>
 <dd>Na tej stronie omawia sie najpopularniejsze systemy szablonowania stosowane w JavaScript.</dd>
 <dt><a href="https://plnkr.co/">Plunker</a></dt>
 <dd>Plunker to internetowa społeczność, która tworzy, współpacuje i dzieli się pomysłami na tworzenie strom internetowych&nbsp;Edytuj w przegladarce swoje pliki JavaScript, CSS i&nbsp;HTML i ogladaj na żywo wyniki swojej pracy i strukturę plików.</dd>
</dl>
</div>
</div>

<p>{{CommunityBox("JavaScript", "dev-tech-js-engine-internals", "mozilla.dev.tech.js-engine.internals", "js", "ES discuss|https://esdiscuss.org/|esdiscuss.org|ECMAScript standard discussion mailing list||SpiderMonkey|https://wiki.mozilla.org/JavaScript|Project page|Contribute to the JavaScript Engine||Twitter|https://twitter.com/SpiderMonkeyJS|@SpiderMonkeyJS|SpiderMonkey updates on Twitter")}}</p>

