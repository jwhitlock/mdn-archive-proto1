---
version: prototype1
revision_id: 1292649
locale: es
slug: Web/HTTP
tags: "HTTP" "Web" "TopicStub" "Referencia" "NeedsTranslation"
title: HTTP
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: True
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<div>{{ HTTPSidebar }}</div>

<p class="summary"><strong><dfn>Hypertext Transfer Protocol (HTTP)</dfn></strong> (o <strong><dfn>Protocolo de Transferencia de Hipertexto en español)</dfn></strong> es un protocolo de la <a class="external" href="http://es.wikipedia.org/wiki/Capa_de_aplicaci%C3%B3n">capa de aplicación</a> para la transmisión de documentos hipermedia, como HTML. Fue diseñado para la comunicación entre los navegadores y servidores web, aunque puede ser utilizado para otros propósitos también. Sigue el clásico <a class="external" href="http://es.wikipedia.org/wiki/Cliente-servidor">modelo cliente-servidor</a>, en el que un cliente establece una conexión, realizando una petición a un servidor y espera una respuesta del mismo. Se trata de un <a class="external" href="http://es.wikipedia.org/wiki/Protocolo_sin_estado">protocolo sin estado</a>, lo que significa que el servidor no guarda ningún dato (estado) entre dos peticiones. Aunque en la mayoría de casos se basa en una conexión del tipo TCP/IP, puede ser usado sobre cualquier <a class="external" href="http://es.wikipedia.org/wiki/Capa_de_transporte">capa de transporte</a> segura o de confianza, es decir, sobre cualquier protocolo que no pierda mensajes silenciosamente, tal como UDP.</p>

<div class="column-container">
<div class="column-half">
<h2 id="Tutoriales">Tutoriales</h2>

<p>Aprende como utilizar HTTP con guías y tutoriales.</p>

<dl>
 <dt><a href="/es/docs/Web/HTTP/Overview">Generalidades de HTTP</a></dt>
 <dd>Se presentan las características básicas del protocolo y su estructura cliente-servidor: qué puede hacer y cuáles son sus usos.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Basics_of_HTTP/Evolution_of_HTTP">Evolución de HTTP</a></dt>
 <dd>Una breve descripción de los cambios del protocolo HTTP desde sus primeras versiones hasta el moderno HTTP/2 y más allá.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Messages">Mensajes HTTP</a></dt>
 <dd>Se describen los tipos de mensajes y distintas estructuras de los mensajes del protocolo HTTP/1.X y HTTP/2</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Session">&nbsp;La típica sesión HTTP</a></dt>
 <dd>Se muestra y explica como es una sesion HTTP típica.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Connection_management_in_HTTP_1.x">Manejo de conexión en HTTP/1.X</a>&nbsp;</dt>
 <dd>Se describen los tres tipos de gestiones posibles en una sesión HTTP/1.x, sus principales ventajas e inconvenientes.</dd>
 <dt><a href="/en-US/docs/Mozilla/HTTP_cache">HTTP Cache</a></dt>
 <dd>La gestión de la Cache es fundamental para la eficiencia de sitios Web. En este artículo se presentan los distintos tipos de cache y como usar las cabeceras HTTP para su configuración y control.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Cookies">HTTP Cookies</a></dt>
 <dd>El funcionamiento de las cookies se define en&nbsp;<a class="external" href="http://tools.ietf.org/html/rfc6265">RFC 6265</a>. Al recibir una petición HTTP, un servidor puede enviar una cabecera <code>Set-Cookie</code> junto con la respuesta. Posteriormente el cliente devuelve el valor de la cookie en cada petición&nbsp;al mismo servidor en forma de cabecera de solicitud <code>Cookie</code>. La cookie también puede tener una fecha de expiración determinada, o puede estar restringida a un dominio y path específico.</dd>
 <dt><a href="/en-US/docs/HTTP/Access_control_CORS">Control de Acceso HTTP (CORS)</a></dt>
 <dd>Las <strong>Solicitudes Inter-Sitio HTTP </strong>(Cross-site HTTP requests en inglés), son peticiones HTTP por recursos pertenecientes a un dominio distinto al dominio del recurso que está haciendo la petición. Por ejemplo, una página HTML de un dominio A (http://dominioa.ejemplo/) hace una solicitud por una imagen en un dominio B (http://dominiob.foo/imagen.jpg) a través del elemento <code>img</code>. Hoy en día, las webs utilizan recursos de otros orígenes muy a menudo, incluyendo hojas de estilo CSS, imágenes, scripts y otros recursos. El Control de Acceso HTTP posibilita a los desarrolladores web a controlar cómo su sitio web responde a solicitudes de otros orígenes.</dd>
</dl>

<dl>
 <dt><a href="https://wiki.mozilla.org/Security/Guidelines/Web_Security">Consejos de Seguridad Web de Mozilla</a></dt>
 <dd>Una colección de tips para ayudar a equipos de desarrollo con la creación de aplicaciones web seguras.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Referencias">Referencias</h2>

<p>Navega la documentación detallada del protocolo HTTP.</p>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Headers">Cabeceras HTTP</a>&nbsp;</dt>
 <dd>Las cabeceras de mensaje HTTP se usan para describir un recurso, o el comportamiento del servidor o del cliente. Pueden agregarse cabeceras personalizadas usando el prefijo 'X-'; otras en un <a class="external" href="http://www.iana.org/assignments/message-headers/perm-headers.html">registro IANA</a>, cuyo contenido fue inicialmente definido en <a class="external" href="http://tools.ietf.org/html/rfc4229">RFC 4229</a>. IANA mantiene también un <a class="external external-icon" href="http://www.iana.org/assignments/message-headers/prov-headers.html">registro de nuevas cabeceras de mensaje HTTP propuestas</a>.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Methods">Métodos de Petición HTTP</a></dt>
 <dd>Las distintas operaciones que se pueden realizar con HTTP: {{HTTPMethod("GET")}}, {{HTTPMethod("POST")}}, y solicitudes menos comunes como {{HTTPMethod("OPTIONS")}}, {{HTTPMethod("DELETE")}}, o {{HTTPMethod("TRACE")}}.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Response_codes">Códigos de Respuesta de Estado HTTP</a></dt>
 <dd>Los códigos de respuesta HTTP indican si una determinada petición HTTP se ha completado correctamente o no. Las respuestas se clasifican en cinco clases: respuestas informativas, respuestas de petición correcta, redirecciones, error del cliente y error del servidor.</dd>
 <dt>&nbsp;</dt>
</dl>

<h2 id="Herramientas_y_recursos">Herramientas y recursos</h2>

<p>Herramientas útiles para usar y revisar conexiones HTTP.</p>

<dl>
 <dt><a href="/en-US/docs/Tools">Firefox Developer Tools</a></dt>
 <dd><a href="/en-US/docs/Tools/Network_Monitor">Network monitor</a>&nbsp;(monitor de red)</dd>
 <dt><a href="https://redbot.org/">RedBot</a></dt>
 <dd>Una herramienta para comprobar el estado de las cabeceras de cache.</dd>
</dl>
</div>
</div>

