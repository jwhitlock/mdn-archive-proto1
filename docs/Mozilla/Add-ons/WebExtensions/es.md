---
version: prototype1
revision_id: 1312409
locale: es
slug: Mozilla/Add-ons/WebExtensions
tags: "Complementos" "Dónde empezar" "WebExtensions" "extensiones"
title: Extensiones del navegador
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<p>Las extensiones pueden extender y modificar la capacidad de un navegador. Las extensiones para Firefox son construidas utilizando las APIs de WebExtension, un sistema para el desarrollo de extensiones multi-navegador. En gran medida, el sistema es compatible con la <a class="external-icon external" href="https://developer.chrome.com/extensions">API de extensión</a> soportada por Google Chrome, Opera y el <a href="https://browserext.github.io/browserext/">borrador del grupo de la comunidad del W3C</a>. Las extensiones escritas para estos navegadores se ejecutarán en la mayoría de los casos en Firefox o <a href="https://developer.microsoft.com/en-us/microsoft-edge/platform/documentation/extensions/">Microsoft Edge</a> con sólo <a href="https://developer.mozilla.org/es/Add-ons/WebExtensions/Porting_from_Google_Chrome">unos pocos cambios</a>. La API también es totalmente compatible con <a href="https://developer.mozilla.org/es/Firefox/Multiprocess_Firefox">multiprocesos de Firefox</a>.</p>

<p>Si tiene alguna idea, pregunta, o necesita ayuda en el proceso de migración de un complemento heredado al uso de las APIs de WebExtension, puede ponerse en contacto con nosotros a través de la <a href="https://mail.mozilla.org/listinfo/dev-addons">lista de correo dev-addons</a> o en el canal <a href="irc://irc.mozilla.org/extdev">#extdev</a> de <a href="https://wiki.mozilla.org/IRC">IRC</a>.</p>

<div class="row topicpage-table">
<div class="section">
<h2 id="Primeros_pasos">Primeros pasos</h2>

<ul>
 <li><a href="/es/Add-ons/WebExtensions/What_are_WebExtensions">¿Qué son las extensiones?</a></li>
 <li><a href="/es/Add-ons/WebExtensions/Your_first_WebExtension">Tu primera extensión</a></li>
 <li><a href="/es/Add-ons/WebExtensions/Your_second_WebExtension">Tu segunda extensión</a></li>
 <li><a href="/es/Add-ons/WebExtensions/Anatomy_of_a_WebExtension">Anatomía de una extensión</a></li>
 <li><a href="/es/Add-ons/WebExtensions/Examples">Ejemplos de extensiones</a></li>
</ul>

<h2 id="Cómo">Cómo</h2>

<ul>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/Intercept_HTTP_requests">Interceptar solicitudes HTTP</a></li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/Modify_a_web_page">Modificar una página web</a></li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/Add_a_button_to_the_toolbar">Agregar un botón a la barra de herramientas</a></li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/Implement_a_settings_page">Implementar una página de configuración</a></li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/Interact_with_the_clipboard">Interactuar con el portapapapeles</a></li>
</ul>

<h2 id="Interfaz_de_usuario">Interfaz de usuario</h2>

<ul>
 <li>Introducción</li>
 <li>Botón en la barra de herramientas del navegador</li>
 <li>Botón en barra de herramientas del navegador con una ventana emergente</li>
 <li>Botón en la barra de direcciones</li>
 <li>Botón en barra de direcciones con una ventana emergente</li>
 <li>Elementos en el menú contextual</li>
 <li>Barras laterales</li>
 <li>Página de opciones</li>
 <li>Páginas web embebidas</li>
 <li>Notificaciones</li>
 <li>Sugerencias en la barra de direcciones</li>
 <li>Paneles de herramientas para desarrolladores</li>
</ul>

<h2 id="Conceptos">Conceptos</h2>

<ul>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/API">Descripción general de la API JavaScript</a></li>
 <li><a href="/es/Add-ons/WebExtensions/Content_scripts">Scripts de contenido</a></li>
 <li><a href="/es/Add-ons/WebExtensions/Match_patterns">Patrones de coincidencia</a></li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/Internationalization">Internacionalización</a></li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/Content_Security_Policy">Política de seguridad de contenido</a></li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/Native_messaging">Mensajería nativa</a></li>
 <li>Utilización de las APIs de devtools</li>
 <li>Buenas prácticas para la experiencia de usuario</li>
</ul>

<h2 id="Portado">Portado</h2>

<ul>
 <li><a href="/es/Add-ons/WebExtensions/Porting_from_Google_Chrome">Portar una extensión de Google Chrome</a></li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">Portar un complemento heredado de Firefox</a></li>
 <li>Desarrollo para Firefox para Android</li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/Embedded_WebExtensions">WebExtensions integradas</a></li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_the_Add-on_SDK">Comparación con el complemento SDK</a></li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_XUL_XPCOM_extensions">Comparación con las extensiones XUL/XPCOM</a></li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/Chrome_incompatibilities">Incompatibilidades con Chrome</a></li>
 <li>Diferencias entre el escritorio y Android</li>
</ul>

<h2 id="Flujo_de_trabajo_de_Firefox">Flujo de trabajo de Firefox</h2>

<ul>
 <li>Experiencia de usuario</li>
 <li><a href="/es/Add-ons/WebExtensions/Temporary_Installation_in_Firefox">Instalación</a></li>
 <li><a href="/es/Add-ons/WebExtensions/Debugging">Depuración</a></li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/Getting_started_with_web-ext">Primeros pasos con web-ext</a></li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/web-ext_command_reference">Referencia del comando web-ext</a></li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/WebExtensions_and_the_Add-on_ID">Extensiones y el ID del complemento</a></li>
 <li>Opciones alternativas de distribución</li>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/Publishing_your_WebExtension">Publicar su extensión</a></li>
</ul>
</div>

<div class="section">
<h2 id="Referencia">Referencia</h2>

<ul>
 <li><a href="/es/docs/Mozilla/Add-ons/WebExtensions/API">Descripción general de la API JavaScript</a></li>
 <li><a href="/es/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">Tablas de compatibilidad del navegador para las API de JavaScript</a></li>
</ul>

<h4 id="APIs_de_JavaScript">APIs de JavaScript</h4>

<div class="twocolumns">{{ ListSubpages ("/en-US/Add-ons/WebExtensions/API") }}</div>

<h4 id="Manifest_keys">Manifest keys</h4>

<div class="twocolumns">{{ ListSubpages ("/en-US/Add-ons/WebExtensions/manifest.json") }}</div>
</div>
</div>

