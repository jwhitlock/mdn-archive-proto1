---
version: prototype1
revision_id: 1294481
locale: hu
slug: Web/JavaScript
tags: "Főoldal" "Tanulás" "JavaScript" "l10n:priority"
title: JavaScript
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p class="summary"><strong>A JavaScript</strong> (<strong>JS</strong>) egy kis erőforrásigényű értelmezett vagy JIT-fordított programozási nyelv {{Glossary("First-class Function", "első osztályú functiók")}}kal. Bár legtöbben weblodalak script nyelveként ismerik, sok webböngészőn kívüli környezetben is használják. Ilyen a <a class="external external-icon" href="https://nodejs.org/">node.js</a> és az <a href="https://couchdb.apache.org/">Apache CouchDB</a>. A JavaScript egy {{Glossary("Prototype-based programming", "prototípus-alapú")}}, multi-paradigma, dinamikus nyelv, ami támogatja az objektumorientált,&nbsp;imperativus, és deklaratív (pl.: funkcionális programozási) stílusokat. Többet itt olvashat <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/About_JavaScript">a JavaScriptről</a>.</p>

<p>Az oldal ezen része magáról, a JavaScript nyelvről szól, mintsem azokról a részekről, amik különböző weboldalaktól és környezetektől függnek. A weboldalaktól függő {{Glossary("API","API")}}-król lásd <a href="https://developer.mozilla.org/en-US/docs/Web/API">Web API-k</a> és a <a href="https://developer.mozilla.org/en-US/docs/Glossary/DOM">DOM</a>.</p>

<p>A JavaScript szabványa az <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Language_Resources">ECMAScript</a>. 2012-től kezdődően, mindegyik <a href="https://kangax.github.io/compat-table/es5/">modern böngésző</a> támogatja az ECMAScript 5.1.-et. Régebbi böngészők legalább az ECMAScript 3-at támogatják. 2015. június 17-én az <a href="https://www.ecma-international.org">ECMA International</a> kiadta az&nbsp;ECMAScript hatodik jelentősebb verzióját, amit hivatalosan ECMAScript 2015-nek neveznek, de eleinte az ECMAScript 6 és az ES6 nevekkel illették. Azóta az ECMAScript szabványokat éves ciklusokban adják ki. Ez a dokumentáció a legújabb tervezetre vonatkozik, ami jelenleg az <a href="https://tc39.github.io/ecma262/">ECMAScript 2018</a>.</p>

<p>A JavaScript nem összetévesztendő a&nbsp;<a href="https://en.wikipedia.org/wiki/Java_%28programming_language%29"> Java programozási nyev</a>vel. A "Java" és a "JavaScript" is az Oracle USA-ban és sok más országban regisztrált védjegye. Ettől függetlenül a két programozási nyelv szintaktikája, szematikája és alkalmazása jelentős mértékben eltér.</p>

<div class="column-container">
<div class="column-half">
<h2 id="Oktatóanyagok">Oktatóanyagok</h2>

<p>Tanulja meg a JavaScript-ben történő programozást útmutatók és bemutatók segítségével.</p>

<h3 id="Teljes_kezdőknek">Teljes kezdőknek</h3>

<p>Látogassa meg a <a href="https://developer.mozilla.org/en-US/docs/Learn/JavaScript">Tanulási területünk JavaScript tárgyát</a> ha nem rendekezik JavaScript vagy másféle programozási tapasztalattal. Ott megtalálhatóak az alábbi mudulok:</p>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps">JavaScript első lépések</a></dt>
 <dd>Az olyan kérdések megválaszolása, mint "mi a JavaScript?", "hogy néz ki?", és "mire képes?", emellett a JavaScript fő funkciójainak ismertetése, mint a változók, stringek, számok és tömbök.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks">JavaScript építőkockák</a></dt>
 <dd>Folytatja a JavaScript alapvető fő funkcióinak beszámolóját a figyelmet a gyakran előforduló típusú kód blokkok felé fordítva, mint az elágazások, ciklusok, függvények, és az esetek.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects">A JavaScript objektumok bemutatása</a></dt>
 <dd>A JavaScript objektumorientált jellegének megértése fontos, ha további tudást szeretne szerezni a nyelvről és ha hatékonyabb kódot szeretne írni. Ezért hoztuk létre ezt a modult, hogy segítsünk.</dd>
</dl>

<h3 id="JavaScript_útmutató">JavaScript útmutató</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide">JavaScript útmutató</a></dt>
 <dd>Egy sokkal részletesebb útmutató a JavaScript nyelvhez, amit olyanoknak szántunk, akik rendelkeznek már JavaScript vagy más programozási tapasztalattal.</dd>
</dl>

<h3 id="Középszint">Középszint</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript">A JavaScript újbóli bemutatása</a></dt>
 <dd>Egy áttekintés azoknak, akik azt <em>gondolják</em> hogy ismerik JavaScript-et.</dd>
</dl>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures">JavaScript adatstruktúrák</a></dt>
 <dd>A JavaScript-ben elérhető adatstruktúrák áttekintése.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness">Egyenlőség és azonosság</a></dt>
 <dd>A JavaScript-ben háromféle értékösszehasonító műveletet érhetünk el: a szigorú egyenlőséget a <code>=== </code>hasznlatával, a laza egyenlőséget a&nbsp; <code>== </code>használatával, és az {{jsxref("Global_Objects/Object/is", "Object.is()")}} függvényt.</dd>
</dl>

<h3 id="Haladó">Haladó</h3>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain">Öröklődés és a prototípus lánc</a></dt>
 <dd>A széleskörben félreértett és alábecsült prototípus alapú öröklődés értelmezése.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode">Szigorú mód</a></dt>
 <dd>A szigorú mód meghatározza, hogy nem lehet használni egy változót az inicializálását megelőzően. Ez az ECMAScript&nbsp;5 egy korlátozott változata, a gyorsabb teljesítmény és könnyebb hibakeresés érdekében.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Typed_arrays">JavaScript tipizált tömbök</a></dt>
 <dd>A JavaScript tipizált tömbök lehetővé teszik a nyers bináris adatok elérését.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Memory_Management">Memóriakezelés</a></dt>
 <dd>A memória életciklus és a szemétgyűjtés JavaScript-ben.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop">A párhuzamos modell és az eseményciklus</a></dt>
 <dd>JavaScript-ben van egy párhuzamos modell, ami egy "eseménycikluson" alapszik.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Referencia">Referencia</h2>

<p>A <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference">JavaScript referencia</a> documentáció böngészése.</p>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects">Az alapértelmezett objektumok</a></dt>
 <dd>Ismerje meg az alapértelmezett beépített objektumokat: {{jsxref("Array")}}, {{jsxref("Boolean")}}, {{jsxref("Date")}}, {{jsxref("Error")}}, {{jsxref("Function")}}, {{jsxref("JSON")}}, {{jsxref("Math")}}, {{jsxref("Number")}}, {{jsxref("Object")}}, {{jsxref("RegExp")}}, {{jsxref("String")}}, {{jsxref("Map")}}, {{jsxref("Set")}}, {{jsxref("WeakMap")}}, {{jsxref("WeakSet")}}, és másokat.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators">Kifejezések és operátorok</a></dt>
 <dd>Tudjon meg többet a JavaScript operátoroktól: {{jsxref("Operators/instanceof", "instanceof")}}, {{jsxref("Operators/typeof", "typeof")}}, {{jsxref("Operators/new", "new")}}, {{jsxref("Operators/this", "this")}}, az <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_Precedence">operátor elsőbbségről</a>, és másokról.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements">Állítások</a></dt>
 <dd>Ismerje meg, hogyan működnek a {{jsxref("Statements/do...while", "do-while")}}, {{jsxref("Statements/for...in", "for-in")}}, {{jsxref("Statements/for...of", "for-of")}}, {{jsxref("Statements/try...catch", "try-catch")}}, {{jsxref("Statements/let", "let")}}, {{jsxref("Statements/var", "var")}}, {{jsxref("Statements/const", "const")}}, {{jsxref("Statements/if...else", "if-else")}}, {{jsxref("Statements/switch", "switch")}}, és más JavaScript állítások és kulcsszavak.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions">Függvények</a></dt>
 <dd>Ismerje meg a JavaScript függvényeivel történő munkát alkalmazásfejlesztés során.</dd>
</dl>

<h2 id="Eszközök_és_források">Eszközök és források</h2>

<p>Hasznos eszközök <strong>JavaScript </strong>kód írásához és hibakereséséhez.</p>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Tools">Firefox Fejlesztői Eszközök</a></dt>
 <dd><a href="https://developer.mozilla.org/en-US/docs/Tools/Scratchpad">Jegyzettömb</a>, <a href="https://developer.mozilla.org/en-US/docs/Tools/Web_Console">Web Konzol</a>, <a href="https://developer.mozilla.org/en-US/docs/Tools/Profiler">JavaScript Profiler</a>, hibakereső, és mások.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Shells">JavaScript Héjak</a></dt>
 <dd>A JavaScript héjak lehetővé teszik JavaScript kódrészletek gyors tesztelését.</dd>
 <dt><a href="https://togetherjs.com/">TogetherJS</a></dt>
 <dd>Együttműkösdés egyszerűen. Ha hozzáadja a TogetherJS-t az oldalához, a felhasználók valós időben segíthetnek egymásnak az oldalon.</dd>
 <dt><a href="https://stackoverflow.com/questions/tagged/javascript">Stack Overflow</a></dt>
 <dd>Stack Overflow kérdések "JavaScript" címkével.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/New_in_JavaScript">JavaScript verziók és kiadási megjegyzések</a></dt>
 <dd>Böngéssze a JavaScript's funkciótörténetét és végrehajtási státuszát.</dd>
 <dt><a href="https://jsfiddle.net/">JSFiddle</a></dt>
 <dd>Szerkesszen JavaScript-et, CSS-t, HTML-t és kapjon élő eredményeket. Használjon külső forrásokat és működjön együtt a csapatával online.</dd>
</dl>
</div>
</div>

