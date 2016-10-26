---
version: prototype1
revision_id: 1134589
locale: en-US
slug: Web/HTTP
tags: "HTTP" "Web" "Reference" "l10n:priority"
title: HTTP
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{HTTPSidebar}}</div>

<p class="summary"><strong><dfn>Hypertext Transfer Protocol (HTTP)</dfn></strong> is an <a class="external" href="http://en.wikipedia.org/wiki/Application_Layer">application-layer</a> protocol for transmitting hypermedia documents, such as HTML. It was designed for communication between web browsers and web servers, though it can be used for other purposes as well. It follows a classical <a class="external" href="https://en.wikipedia.org/wiki/Client%E2%80%93server_model">client-server model</a>, with a client opening a connection, making a request, and waiting until it receives a response. It is also a <a class="external" href="http://en.wikipedia.org/wiki/Stateless_protocol">stateless protocol</a>, meaning that the server does not keep any data (state) between two requests. Though often based on a TCP/IP layer, it can be used on any reliable <a class="external" href="http://en.wikipedia.org/wiki/Transport_Layer">transport layer</a>, that is a protocol that don't lose messages silently.</p>

<div class="column-container">
<div class="column-half">
<h2 id="Tutorials">Tutorials</h2>

<p>Learn how to use HTTP with guides and tutorials.</p>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Overview">Overview of HTTP</a></dt>
 <dd>Presents the basic features of the client-server protocol: what it can do and what its intended uses</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Basics_of_HTTP/Evolution_of_HTTP">Evolution of HTTP</a></dt>
 <dd>A brief description of the changes that happened in HTTP from the early versions to the modern HTTP/2 and beyond.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Messages">HTTP Messages</a></dt>
 <dd>Describes the type and structure of the different kind of messages of HTTP/1.x and HTTP/2.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Session">A typical HTTP session</a></dt>
 <dd>Shows and explains the flow of a usual HTTP session.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Connection_management_in_HTTP_1.x">Connection management in HTTP/1.x</a></dt>
 <dd>Describes the three connection management models available in HTTP/1.x, their strengths and their weaknesses.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Caching">HTTP Cache</a></dt>
 <dd>Caching is a major tool for right performance Web sites. This article presents the different kind of cache and how to use HTTP Headers to configure and control them.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Cookies">HTTP Cookies</a></dt>
 <dd>How cookies work is defined by <a class="external" href="http://tools.ietf.org/html/rfc6265">RFC 6265</a>. On&nbsp;receiving an HTTP request, a server can send a <code>Set-Cookie</code> header with the response. Afterward, the client returns the cookie value&nbsp;with every request&nbsp;to the same server in the form of a <code>Cookie</code> HTTP header. Additionally, an expiration delay can be specified. The cookie can also be restricted to a specific domain and path.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Access_control_CORS">HTTP Access Control (CORS)</a></dt>
 <dd><strong>Cross-site HTTP requests</strong> are HTTP requests for resources from a <strong>different domain</strong>&nbsp;other than the domain of the resource making the request. For instance, a resource loaded from Domain A (<code>http://domaina.example/</code>), such as an HTML web page, makes a request for a resource on Domain B (http://domainb.foo/), such as an image, using the <code>img</code> element (<code>http://domainb.foo/image.jpg</code>). This occurs very commonly on the web today — pages load many resources in a cross-site manner, including CSS stylesheets, images and scripts, and other resources.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Controlling_DNS_prefetching">Controlling DNS prefetching</a></dt>
 <dd>Firefox and most other modern browsers perform <strong>DNS prefetching</strong>. This is when browsers proactively perform domain name resolution on links that the user may choose to follow and resources referenced by the document, such as images, CSS, and JavaScript. This prefetching is performed in the background so that the DNS lookup is likely to have already been resolved by the time the referenced items are requested. This reduces latency when, for example, the user clicks a link.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Reference">Reference</h2>

<p>Browse through detailed HTTP reference documentation.</p>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Headers">HTTP Headers</a></dt>
 <dd>HTTP message headers are used to describe precisely the resource or the behavior of the server or the client. Custom proprietary headers can be added using the 'X-' prefix; others in an <a class="external" href="http://www.iana.org/assignments/message-headers/perm-headers.html">IANA registry</a>, whose original content was defined in <a class="external" href="http://tools.ietf.org/html/rfc4229">RFC 4229</a>. IANA also maintains a <a class="external" href="http://www.iana.org/assignments/message-headers/prov-headers.html">registry of proposed new HTTP message headers</a>.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Methods">HTTP Request Methods</a></dt>
 <dd>The different operation that can be done with HTTP: {{HTTPMethod("GET")}}, {{HTTPMethod("POST")}}, but also less common requests like {{HTTPMethod("OPTIONS")}}, {{HTTPMethod("DELETE")}} or {{HTTPMethod("TRACE")}}.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Response_codes">HTTP Status Response Codes</a></dt>
 <dd>HTTP response codes indicate whether a specific HTTP request has been successfully completed. Responses are grouped in five classes: informational responses, successful responses, redirections, client errors, and servers errors.</dd>
</dl>

<h2 id="Tools_resources">Tools &amp; resources</h2>

<p>Helpful tools for using and debugging your HTTP connections.</p>

<dl>
 <dt><a href="/en-US/docs/Tools">Firefox Developer Tools</a></dt>
 <dd><a href="/en-US/docs/Tools/Network_Monitor">Network monitor</a></dd>
 <dt><a href="https://redbot.org/">RedBot</a></dt>
 <dd>A tool to check your cache-related headers</dd>
 <dt><a href="http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/">How Browsers Work</a></dt>
 <dd>A very comprehensive article on browsers internals &amp; request flow through HTTP protocol. A MUST-READ article for any web developer.</dd>
</dl>
</div>
</div>

