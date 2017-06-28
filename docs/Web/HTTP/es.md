---
version: prototype1
revision_id: 1266285
locale: es
slug: Web/HTTP
tags: "HTTP" "Web" "TopicStub" "Referencia" "NeedsTranslation"
title: HTTP
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{ HTTPSidebar }}</div>

<p class="summary"><strong><dfn>Hypertext Transfer Protocol (HTTP)</dfn></strong> o <strong><dfn>Protocolo de Transferencia de Hipertexto (HTTP)</dfn></strong> es un protocolo de la <a class="external" href="http://es.wikipedia.org/wiki/Capa_de_aplicaci%C3%B3n">capa de aplicación</a> para la transmisión de documentos hipermedia, como HTML. Fue diseñado para la comunicación entre los navegadores y servidores web, aunque puede ser utilizado para otros propósitos también. Sigue el clásico <a class="external" href="http://es.wikipedia.org/wiki/Cliente-servidor">modelo cliente-servidor</a>, en el que un cliente establece una conexión, realizando una petición a un servidor y espera una respuesta del mismo. Se trata de un <a class="external" href="http://es.wikipedia.org/wiki/Protocolo_sin_estado">protocolo sin estado</a>, lo que significa que el servidor no guarda ningún dato (estado) entre dos peticiones. Aunque en la mayoría de casos se basa en una conexión del tipo TCP/IP , puede usarse con cualquier otro protocolo del nivel de la <a class="external" href="http://es.wikipedia.org/wiki/Capa_de_transporte">capa de transporte</a> orientado a la conexión.</p>

<div class="column-container">
<div class="column-half">
<h2 id="Tutoriales">Tutoriales</h2>

<p>Aprende como utilizar HTTP con guías y tutoriales.</p>

<dl>
 <dt><a href="/es/docs/Web/HTTP/Overview">Generalidades de HTTP</a></dt>
 <dd>Se presentan las características básicas del protocolo, y su estructura cliente-servidor: que puede hacer y cuales son sus usos.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Basics_of_HTTP/Evolution_of_HTTP">Evolución de HTTP</a></dt>
 <dd>Una breve descripción de los cambios del protocolo HTTP desde sus primeras versiones hasta el actual HTTP/2 y posterior.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Messages">Mensajes HTTP</a></dt>
 <dd>Se describen los tipos de mensajes y distintas estructuras de los mensajes del protocolo HTTP/1.X y HTTP/2</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Session">&nbsp;La típica sesión HTTP</a></dt>
 <dd>Se muestra y explica como es una sesion HTTP típica.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Connection_management_in_HTTP_1.x">Gestión de la conexión en HTTP/1.X</a>&nbsp;</dt>
 <dd>Se describen los tres tipos de gestiones posibles en una sesión HTTP/1.x, sus principales ventajas e inconvenientes.</dd>
 <dt><a href="/en-US/docs/Mozilla/HTTP_cache">HTTP Cache</a></dt>
 <dd>La gestión de la Cache es fundamental para la eficiencia de sitios Web. En este artículo se presentan los distintos tipos de cache y como usar las cabeceras HTTP para su configuración y control.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Cookies">HTTP Cookies</a></dt>
 <dd>El funcionamiento de las cookies se define en&nbsp;<a class="external" href="http://tools.ietf.org/html/rfc6265">RFC 6265</a>. Al recibir una petición HTTP, un servidor puede enviar un:&nbsp; <code>Set-Cookie</code>&nbsp;con la respuesta. Posteriormente el cliente devuelve la cookie, con el valor de cada petición&nbsp;al mismo servidor en forma de cabecera HTTP Cookie. Incluso, se puede establecer una retardo de expiración si fuese necesario. La cookie, también puede estar restringida a un dominio especifico o a un path.</dd>
 <dt><a href="/en-US/docs/HTTP/Access_control_CORS">HTTP Access Control (CORS)</a></dt>
 <dd><strong>Cross-site HTTP requests&nbsp;</strong>son peticiones HTTP por recursos de un dominio distinto al dominio al que se hace la petición. Por ejemplo: un recurso cargado de un dominio A (http://domainA.ejemplo/), el cual tiene una página web, hace una petición por un recurso en un dominio B (http://domainB.foo/imagen.jpg). Esto ocurre muy habitualmente hoy en día en la web -- páginas web que cargan muchos recursos de manera cruzada (cross-site). Incluyendo hojas de estilo CSS, imágenes, scripts, y otros tipos de recursos.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Controlling_DNS_prefetching">Control de la precarga de DNS</a>&nbsp;</dt>
 <dd>Firefox y la mayoría de los otros navegadores modernos, realizan una precarga de DNS, esto es:&nbsp;cuando un navegador, de forma proactiva realiza una resolución de nombre de dominios&nbsp;en los links&nbsp;que usa, puede elegir seguir y actualizar los recursos referenciados por el documento, como pueden ser: imágenes, hojas de estilo CSS, y código JavaScript. Esta precarga se ejecuta en un plano secundario, con lo que la tabla de DNS puede estar resuelta para cuando los citados recursos sean pedidos. Esto reduce los tiempos de espera, por ejemplo, cuando el usuario, hace click en un link.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Referencias">Referencias</h2>

<p>Documentación de referencia del protocolo HTTP:</p>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Headers">Cabeceras HTTP</a>&nbsp;</dt>
 <dd>Las cabeceras de los mensajes HTTP, se usan para describir el recurso o comportamiento del servidor o del cliente. Cabeceras modificadas pueden usarse usando el prefijo 'X-'; otros en un registro <a class="external" href="http://www.iana.org/assignments/message-headers/perm-headers.html">IANA registry</a>&nbsp;que inicialmente fueron definidos en <a class="external" href="http://tools.ietf.org/html/rfc4229">RFC 4229</a>&nbsp;también pueden utilizarse. IANA mantiene también una lista de nuevas cabeceras HTTP propuestas.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Methods">Peticiones HTTP</a></dt>
 <dd>Con HTTP, se pueden realizar distintas funciones, con los métodos GET o POST, aunque también hay peticiones de otros métodos como OPTIONS, DELETE, o TRACE..</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Response_codes">Códigos de estado de respuesta HTTP</a></dt>
 <dd>Los códigos de estado de respuesta HTTP, indican si una determinada petición HTTP, se ha completado correctamente o no. Los estados de respuesta, se clasifican en cinco clases: respuestas informativas, respuestas de petición correcta, respuestas de redirección, respuestas de error en el cliente y respuestas de error en el servidor. .</dd>
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

