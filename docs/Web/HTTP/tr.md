---
version: prototype1
revision_id: 1218787
locale: tr
slug: Web/HTTP
tags: "HTTP" "Web" "HTTP nedir"
title: HTTP
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<div>{{HTTPSidebar}}</div>

<p class="summary"><span class="seoSummary"><strong><dfn>Hypertext Transfer Protocol (HTTP) hipermedya belgelerinin "HTML gibi" iletilmesi için oluşturulmuş bir <a class="external" href="https://tr.wikipedia.org/wiki/Uygulama_tabakas%C4%B1">uygulama katmanı</a> protokolüdür. HTTP web tarayıcıları ve web sunucuları arasında iletişim için dizayn edilmiştir, fakat diğer amaçlar için kullanılabilir. HTTP klasik <a class="external" href="https://tr.wikipedia.org/wiki/%C4%B0stemci-sunucu">istemci-sunucu modeline</a> uyar, bir istemci bir istek yapmak için bağlantı kurar ve ardından bir yanıt alana kadar bekler. HTTP <a class="external" href="https://en.wikipedia.org/wiki/Stateless_protocol">durumsuz protokoldür</a>, yani sunucu iki istek arasında herhangi bir veri (durum) tutmaz. Genellikle TCP/UP katmanına dayalı olsa da, herhangi bir güvenilir <a class="external" href="http://en.wikipedia.org/wiki/Transport_Layer">taşıma katmanının</a>, mesajları sessizce kaybetmeyen bir protokol "UDP gibi", üzerinde kullanılabilir.</dfn></strong></span></p>

<div class="column-container">
<div class="column-half">
<h2 id="Dersler">Dersler</h2>

<p>HTTP'yi rehberler ve dersler ile öğrenin.</p>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Overview">HTTP'ye Genel Bakış</a></dt>
 <dd>İstemci-Sunucu protokolünün temel özellikleri, ne yapabileceği ve kullanım amaçları.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Caching">HTTP Önbellek</a></dt>
 <dd>Önbellekleme hızlı Web siteleri için çok önemlidir. Bu yazı, farklı önbellekleme metodlarını ve HTTP başlıklarının önbellekleme kontrolü için nasıl kullanılacağını açıklamaktadır.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Cookies">HTTP Çerezleri</a></dt>
 <dd>How cookies work is defined by <a class="external" href="http://tools.ietf.org/html/rfc6265">RFC 6265</a>. When serving an HTTP request, a server can send a <code>Set-Cookie</code> HTTP header with the response. The client then returns the cookie's value with every request to the same server in the form of a <code>Cookie</code> request header. The cookie can also be set to expire on a certain date, or restricted to a specific domain and path.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Access_control_CORS">HTTP Access Control (CORS)</a></dt>
 <dd><strong>Cross-site HTTP requests</strong> are HTTP requests for resources from a <strong>different domain</strong> than the domain of the resource making the request. For instance, an HTML page from Domain A (<code>http://domaina.example/</code>) makes a request for an image on Domain B (<code>http://domainb.foo/image.jpg</code>) via the <code>img</code> element. Web pages today very commonly load cross-site resources, including CSS stylesheets, images, scripts, and other resources. CORS allows web developers to control how their site reacts to cross-site requests.</dd>
</dl>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Basics_of_HTTP/Evolution_of_HTTP">Evolution of HTTP</a></dt>
 <dd>A brief description of the changes between the early versions of HTTP, to the modern HTTP/2 and beyond.</dd>
 <dt><a href="https://wiki.mozilla.org/Security/Guidelines/Web_Security">Mozilla web security guidelines</a></dt>
 <dd>A collection of tips to help operational teams with creating secure web applications.</dd>
</dl>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Messages">HTTP Messages</a></dt>
 <dd>Describes the type and structure of the different kind of messages of HTTP/1.x and HTTP/2.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Session">A typical HTTP session</a></dt>
 <dd>Shows and explains the flow of a usual HTTP session.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Connection_management_in_HTTP_1.x">Connection management in HTTP/1.x</a></dt>
 <dd>Describes the three connection management models available in HTTP/1.x, their strengths, and their weaknesses.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Başvuru_Belgeleri">Başvuru Belgeleri</h2>

<p>Ayrıntılı HTTP başvuru belgelerine göz atın.</p>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Headers">HTTP Başlıkları</a></dt>
 <dd>HTTP mesaj başlıkları, bir kaynağı ya da sunucu veya istemcinin davranışını tanımlamak için kullanılır. Özel başlıklar X- öneki ile birlikte eklenebilir diğerleri ise orijinal içeriği <a class="external" href="http://tools.ietf.org/html/rfc4229">RFC 4229</a>'da tanımlı olan <a class="external" href="https://www.iana.org/assignments/message-headers/message-headers.xhtml">IANA kayıtlarında</a> gösterilmiştir. IANA, aynı zamanda <a class="external" href="https://www.iana.org/assignments/message-headers/message-headers.xhtml">yeni önerilen HTTP mesaj başlıklarının</a> kaydını bulundurur.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Methods">HTTP İstek Metodları</a></dt>
 <dd>HTTP ile yapılabilen farklı işlemler:<br />
 {{HTTPMethod("GET")}}, {{HTTPMethod("POST")}}, ve daha az yaygın olan istek metodları,&nbsp;{{HTTPMethod("OPTIONS")}}, {{HTTPMethod("DELETE")}}, veya&nbsp;{{HTTPMethod("TRACE")}}.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Response_codes">HTTP Status Response Codes</a></dt>
 <dd>HTTP response codes indicate whether a specific HTTP request has been successfully completed. Responses are grouped in five classes: informational responses, successful responses, redirections, client errors, and servers errors.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Headers/Content-Security-Policy">CSP directives</a></dt>
 <dd>The {{HTTPHeader("Content-Security-Policy")}} response header fields allows web site administrators to control resources the user agent is allowed to load for a given page. With a few exceptions, policies mostly involve specifying server origins and script endpoints.</dd>
</dl>

<h2 id="Tools_resources">Tools &amp; resources</h2>

<p>Helpful tools and resources for understanding and debugging HTTP.</p>

<dl>
 <dt><a href="/en-US/docs/Tools">Firefox Developer Tools</a></dt>
 <dd><a href="/en-US/docs/Tools/Network_Monitor">Network monitor</a></dd>
 <dt><a href="https://observatory.mozilla.org/">Mozilla Observatory</a></dt>
 <dd>
 <p>A project designed to help developers, system administrators, and security professionals configure their sites safely and securely.</p>
 </dd>
 <dt><a class="external" href="https://redbot.org/">RedBot</a></dt>
 <dd>Tools to check your cache-related headers</dd>
 <dt><a href="http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/">How Browsers Work</a></dt>
 <dd>A very comprehensive article on browser internals and request flow through HTTP protocol. A MUST-READ for any web developer.</dd>
</dl>
</div>
</div>

