---
version: prototype1
revision_id: 1329420
locale: es
slug: Web/JavaScript
tags: "Aprender" "JavaScript"
title: JavaScript
summary: 
keywords: 
needs_technical_review: True
needs_editorial_review: True
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>
<p>{{JsSidebar}}</p>

<p class="summary"><strong>JavaScript</strong> (<strong>JS</strong>) es un lenguaje ligero e interpretado, orientado a objetos con&nbsp;<strong style="background-color:#f4f7f8; font-weight:bold; line-height:1.5">&nbsp;</strong><a href="https://en.wikipedia.org/wiki/First-class_functions" style="line-height: 1.5; font-weight: bold; background-color: rgb(244, 247, 248);" title="https://en.wikipedia.org/wiki/First-class_functions">funciones de primera clase</a><span style="line-height:1.5">, más conocido como el lenguaje de script para páginas web, pero también </span><a href="http://en.wikipedia.org/wiki/JavaScript#Uses_outside_web_pages" style="line-height: 1.5;" title="http://en.wikipedia.org/wiki/JavaScript#Uses_outside_web_pages">usado en muchos entornos sin navegador</a><span style="line-height:1.5">, tales como &nbsp;</span><strong style="background-color:#f4f7f8; font-weight:bold; line-height:1.5">&nbsp;</strong><a class="external external-icon" href="http://nodejs.org/" style="line-height: 1.5; white-space: pre-line; font-weight: bold; background-color: rgb(244, 247, 248);">node.js</a><strong style="background-color:#f4f7f8; font-weight:bold; line-height:1.5">&nbsp;o&nbsp;</strong><a href="http://couchdb.apache.org/" style="line-height: 1.5; font-weight: bold; background-color: rgb(244, 247, 248);">Apache CouchDB</a><strong style="background-color:#f4f7f8; font-weight:bold; line-height:1.5">. </strong>Es un lenguaje script multi-paradigma,&nbsp;<a class="mw-redirect" href="https://en.wikipedia.org/wiki/Prototype-based" style="font-weight: bold; background-color: rgb(244, 247, 248);" title="Prototype-based">basado en prototipos</a>,&nbsp; dinámico, soporta estilos de programación funcional, orientada a objetos e imperativa.&nbsp;<a href="/es/docs/JavaScript/Acerca_de_JavaScript" style="line-height: 1.5;" title="JavaScript/Acerca_de_JavaScript">Leer más sobre JavaScript</a><span style="line-height:1.5">.</span></p>

<p>Esta sección de la web está dedicada al lenguaje JavaScript, a las partes que no son específicas de las páginas web u otros entornos de servidor. Para información sobre las API específicas de las páginas web, consulte <a href="/es/docs/DOM" title="DOM">DOM</a>. Para saber más sobre cómo encajan DOM y JavaScript, dispone de la <a href="/es/docs/Referencia_DOM_de_Gecko/Introducción#DOM_y_JavaScript" title="Referencia_DOM_de_Gecko/Introducción#DOM_y_JavaScript">referencia de DOM</a>.</p>

<p>El estándar de JavaScript es <a href="/en-US/docs/JavaScript/Language_Resources">ECMAScript</a>. Desde el 2012, todos los navegadores modernos soportan completamente ECMAScript 5.1. Los navegadores más antiguos soportan por lo menos ECMAScript 3. La sexta edición, conocida<span class="short_text" id="result_box" lang="es"><span> inicialmente como ECMAScript 6 o ES6, </span></span> se liberó el 17 de Julio de 2017. Desde entonces, <span id="result_box" lang="es"><span>los estándares ECMAScript están en ciclos de lanzamiento anuales</span></span><span lang="es"><span>.</span> <span>Esta documentación se refiere a la última versión del borrador, que actualmente es <a href="https://tc39.github.io/ecma262/">ECMAScript 2018</a>.</span></span></p>

<p>JavaScript no debe ser confundido con el&nbsp;<a href="http://en.wikipedia.org/wiki/Java_(programming_language)">lenguaje de programación Java</a>. Java es una marca registrada de Oracle en Estados Unidos y otros países. <span id="result_box" lang="es"><span>Sin embargo, l</span></span>os dos lenguajes de programación tienen muchas diferencias en las sintaxis, semantica y usos.</p>
</div>

<table class="topicpage-table">
 <tbody>
  <tr>
   <td>
    <h2 class="Documentation" id="Documentation" name="Documentation">Documentación</h2>

    <dl>
     <dt><a href="/es/docs/Referencia_de_JavaScript_1.5" title="Referencia_de_JavaScript_1.5">Referencia de JavaScript</a></dt>
     <dd>Esta referencia de JavaScript incluye documentación completa de JavaScript 1.5 y posteriores actualizaciones.</dd>
     <dt><a href="/es/docs/Guía_JavaScript_1.5" title="Guía_JavaScript_1.5">Guía de JavaScript</a></dt>
     <dd>Nuestra guía principal sobre cómo programar con JavaScript.</dd>
     <dt><a href="/en/JavaScript_technologies_overview" title="./Guide">Vista general de las Tecnologías JavaScript</a></dt>
     <dd>Introducción al escenario de los navegadores JavaScript</dd>
     <dt><a class="internal" href="/En/JavaScript/ECMAScript_5_support_in_Mozilla" title="JavaScript/ECMAScript 5 support in Mozilla">Implementación en Mozilla de ECMAScript 5</a></dt>
     <dd>Un vistazo de la implementación actual — y planificada — de ECMAScript 5.</dd>
     <dt><a href="/es/docs/Novedades_en_JavaScript_1.6" title="Novedades_en_JavaScript_1.6">Novedades en JavaScript 1.6</a></dt>
     <dd>JavaScript 1.6 (incluido en Firefox 1.5 y otras aplicaciones basadas en Mozilla 1.8) añade métodos para localizar y recorrer matrices, funciones Array y String para usarse en otros tipos, e implementación de <a href="/es/docs/E4X" title="E4X">E4X</a> que incluye <code>for each</code>...<code>in</code>.</dd>
     <dt><a href="/es/docs/Novedades_en_JavaScript_1.7" title="Novedades_en_JavaScript_1.7">Novedades en JavaScript 1.7</a></dt>
     <dd>JavaScript 1.7 (incluido en Firefox 2) añade generadores e iteradores, arrays basados en otros (comprensión de arrays), bloques de ámbito con <code>let</code>, y asignación estructurada.</dd>
     <dt><a href="/es/docs/Novedades_en_JavaScript_1.8" title="Novedades_en_JavaScript_1.8">Novedades en JavaScript 1.8</a></dt>
     <dd>JavaScript 1.8 (incluido en Firefox 3.0) añade cierres de expresión (clousures), generador de expresiones, y los métodos <a class="internal" href="/es/docs/Referencia_de_JavaScript_1.5/Objetos_globales/docs/Array/reduce" title="Referencia_de_JavaScript_1.5/Objetos_globales/docs/Array/reduce"><code>reduce()</code></a> y <a class="internal" href="/es/docs/Referencia_de_JavaScript_1.5/Objetos_globales/docs/Array/reduceRight" title="Referencia_de_JavaScript_1.5/Objetos_globales/docs/Array/reduceRight"><code>reduceRight()</code></a> en matrices.</dd>
     <dt><a class="internal" href="/En/JavaScript/New_in_JavaScript/1.8.1" title="./New in JavaScript/1.8.1">Novedades en JavaScript 1.8.1</a></dt>
     <dd>JavaScript 1.8.1 (incluido en Firefox 3.5) añade de manera nativa la codificación y decodificación de JSON, <code><a class="internal" href="/en/JavaScript/Reference/Global_Objects/Object/GetPrototypeOf" title="Core JavaScript 1.5 Reference/Global Objects/Object/GetPrototypeOf">Object.getPrototypeOf</a></code>, y los métodos recorte de cadenas; <code><a class="internal" href="/en/JavaScript/Reference/Global_Objects/String/Trim" title="Core JavaScript 1.5 Reference/Global Objects/String/Trim">trim()</a></code>, <code><a class="internal" href="/en/JavaScript/Reference/Global_Objects/String/TrimLeft" title="Core JavaScript 1.5 Reference/Global Objects/String/TrimLeft">trimLeft()</a></code>, y <code><a class="internal" href="/en/JavaScript/Reference/Global_Objects/String/TrimRight" title="Core JavaScript 1.5 Reference/Global Objects/String/TrimRight">trimRight()</a></code>.</dd>
     <dt><a class="internal" href="/en/JavaScript/New_in_JavaScript/1.8.5" title="./New in JavaScript/1.8.5">Novedades en JavaScript 1.8.5</a></dt>
     <dd>JavaScript 1.8.5 (la última versión, incluida en Firefox 4) añade la implementación de ECMAScript 5 para <a href="/es/docs/Referencia_de_JavaScript_1.5/Objetos_globales/docs/Object" title="Referencia_de_JavaScript_1.5/Objetos_globales/docs/Object"><code>Object</code></a> y métodos <code>Object.prototype</code>, <code>Array.isArray</code>, <code>Function.prototype.bind</code> así como <a href="/en/JavaScript/Reference/Functions_and_function_scope/Strict_mode" title="JavaScript/Strict mode">modo estricto</a></dd>
     <dt><a href="/en/JavaScript/Language_Resources" title="./Language Resources">Recursos del lenguaje JavaScript</a></dt>
     <dd>Una descripción de los estándares del lenguaje JavaScript.</dd>
     <dt><a href="http://wiki.ecmascript.org/lib/exe/fetch.php?id=resources:resources&amp;cache=cache&amp;media=resources:jscriptdeviationsfromes3.pdf">JScript desviaciones del ES3</a> (PDF)</dt>
     <dd>Describe las diferencias entre el estándar ECMAScript ed. 3 y la implementación de Microsoft (JScript). También incluye información de otros navegadores (Opera, Firefox y Safari).</dd>
    </dl>

    <p><span class="alllinks"><a href="/es/docs/tag/JavaScript" title="tag/JavaScript">Ver todo...</a></span></p>
   </td>
   <td>
    <h2 class="Community" id="Community" name="Community">Comunidad</h2>

    <ul>
     <li><a href="https://www.mozilla-hispano.org/foro/viewforum.php?f=20" title="http://www.mozillaes.org/foros/viewforum.php?f=13">Foro de desarrollo</a> comunitario.</li>
     <li>Visita los foros de Mozilla en inglés... {{ DiscussionList("dev-tech-javascript", "mozilla.dev.tech.javascript") }}</li>
     <li><a class="link-irc" href="irc://irc.mozilla.org/js">#js en el irc.mozilla.org</a></li>
    </ul>

    <h2 class="Tools" id="Featured_tools" name="Featured_tools">Herramientas destacadas</h2>

    <ul>
     <li><a href="http://www.getfirebug.com/">Firebug</a> - Depuración y perfilado de JavaScript</li>
     <li><a href="/en/Venkman" title="Venkman">Venkman</a> - Depurador de JavaScript</li>
     <li><a href="/en/JavaScript/Shells" title="./Shells">JavaScript Shells</a> - Fragmentos de código de prueba</li>
     <li><a href="http://www.jslint.com/lint.html">JSLint</a> - Verificador de sintáxis</li>
     <li><a href="http://jshint.com" title="http://jshint.com/">JSHint</a> - Verificador de sintáxis hecho por la comunidad.</li>
     <li><a href="http://code.google.com/p/jsdoc-toolkit/" title="http://code.google.com/p/jsdoc-toolkit/">JSDoc</a> - Generador de documentación a partir del código.</li>
     <li><a href="http://www.aptana.com" title="http://www.aptana.com">Aptana Studio</a> - IDE de código abierto que maneja Ajax y JavaScript (basado en eclipse)</li>
     <li><a href="http://netbeans.org/features/docs/javascript/">Netbeans</a> - IDE de código abierto que incluye una implementación sofisticada de JavaScript</li>
     <li><a href="http://www.eclipse.org/downloads/packages/docs/eclipse-ide-javascript-web-developers/heliossr2" title="http://www.eclipse.org/downloads/packages/docs/eclipse-ide-javascript-web-developers/heliossr2">Eclipse</a> - IDE de código abierto que incluye un toolkit de desarrollo de JavaScript</li>
     <li><a class="link-https" href="https://addons.mozilla.org/en-US/firefox/addon/7434">Extensiones de desarrolladores de extensiones</a> - Ofrece un entorno y shell para JS</li>
     <li><a href="/en/JavaScript/Other_JavaScript_tools" title="./Other JavaScript tools">Otras herramientas JavaScript</a></li>
    </ul>

    <p><span class="alllinks"><a href="/es/docs/tag/JavaScript:Tools" title="tag/JavaScript:Tools">Ver todo...</a></span></p>

    <h2 id="Related_Topics" name="Related_Topics">Otros recursos:</h2>

    <dl>
     <dt><a href="http://bonsaiden.github.com/JavaScript-Garden/" title="http://bonsaiden.github.com/JavaScript-Garden/">JavaScript Garden</a></dt>
     <dd>Un sitio con información muy útil sobre las partes más esotéricas de JavaScript.</dd>
    </dl>

    <h2 class="Related_Topics" id="Related_Topics" name="Related_Topics">Temas relacionados:</h2>

    <ul>
     <li><a href="/es/docs/AJAX" title="AJAX">AJAX</a>, <a href="/es/docs/DOM" title="DOM">DOM</a>, <a class="internal" href="/en-US/docs/JavaScript/Server-Side_JavaScript" title="Server-Side JavaScript">Server-Side JavaScript</a>, <a href="/es/docs/DHTML" title="DHTML">DHTML</a>, <a href="/es/docs/E4X" title="E4X">E4X</a>, <a href="/es/docs/SpiderMonkey" title="SpiderMonkey">SpiderMonkey</a>, <a href="/es/docs/HTML/Canvas" title="HTML/Canvas">Canvas</a></li>
    </ul>
   </td>
  </tr>
 </tbody>
</table>

<p>&nbsp;</p>

