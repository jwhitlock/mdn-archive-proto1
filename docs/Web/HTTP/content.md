---
version: prototype1
revision_id: 1187221
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

<p class="summary"><span class="seoSummary"><strong><dfn>Hypertext Transfer Protocol (HTTP)</dfn></strong> is an <a class="external" href="https://en.wikipedia.org/wiki/Application_Layer">application-layer</a> protocol for transmitting hypermedia documents, such as HTML.</span> It was designed for communication between web browsers and web servers, but it can also be used for other purposes. HTTP follows a classical <a class="external" href="https://en.wikipedia.org/wiki/Client%E2%80%93server_model">client-server model</a>, with a client opening a connection to make a request, then waiting until it receives a response. HTTP is a <a class="external" href="https://en.wikipedia.org/wiki/Stateless_protocol">stateless protocol</a>, meaning that the server does not keep any data (state) between two requests. Though often based on a TCP/IP layer, it can be used on any reliable <a class="external" href="http://en.wikipedia.org/wiki/Transport_Layer">transport layer</a>; that is, a protocol that doesn't lose messages silently, such as UDP.</p>

<div class="column-container">
<div class="column-half">
<h2 id="Tutorials">Tutorials</h2>

<p>Learn how to use HTTP with guides and tutorials.</p>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Overview">Overview of HTTP</a></dt>
 <dd>The basic features of the client-server protocol: what it can do and its intended uses.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Caching">HTTP Cache</a></dt>
 <dd>Caching is very important for fast Web sites. This article describes different methods of caching and how to use HTTP Headers to control them.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Cookies">HTTP Cookies</a></dt>
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
<h2 id="Reference">Reference</h2>

<p>Browse through detailed HTTP reference documentation.</p>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Headers">HTTP Headers</a></dt>
 <dd>HTTP message headers are used to describe a resource, or the behavior of the server or the client. Custom proprietary headers can be added using the <code>X-</code> prefix; others in an <a class="external" href="http://www.iana.org/assignments/message-headers/perm-headers.html">IANA registry</a>, whose original content was defined in <a class="external" href="http://tools.ietf.org/html/rfc4229">RFC 4229</a>. IANA also maintains a <a class="external" href="http://www.iana.org/assignments/message-headers/prov-headers.html">registry of proposed new HTTP message headers</a>.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Methods">HTTP Request Methods</a></dt>
 <dd>The different operations that can be done with HTTP: {{HTTPMethod("GET")}}, {{HTTPMethod("POST")}}, and also less common requests like {{HTTPMethod("OPTIONS")}}, {{HTTPMethod("DELETE")}}, or {{HTTPMethod("TRACE")}}.</dd>
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

