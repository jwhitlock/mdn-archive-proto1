---
version: prototype1
revision_id: 1278905
locale: de
slug: Web/HTTP
tags: "HTTP" "TopicStub" "NeedsTranslation"
title: HTTP
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>Das Hypertext Transfer Protocol (HTTP) ist ein <a href="https://de.wikipedia.org/wiki/OSI-Modell#Schicht_7_.E2.80.93_Anwendungsschicht_.28Application_Layer.29">Anwendungsschicht</a>-Protokoll zum Transportieren von <a href="https://de.wikipedia.org/wiki/Hypermedia">Hypermedia</a> Dokumenten. Hauptsächlich wird es zur Kommunikation zwischen Webservern und Webbrowsern verwendet, jedoch könnte es theoretisch auch für andere Zwecke benutzt werden. Es folgt einem klassischen <a href="https://de.wikipedia.org/wiki/Client-Server-Modell">Client-Server-Modell</a>, mit einem Client der die Verbindung eröffnet, indem er eine Anfrage macht und dann wartet, bis es eine Antwort erhält. Außerdem ist es ein <a href="https://de.wikipedia.org/wiki/Zustandslosigkeit">zustandsloses</a> <a href="https://de.wikipedia.org/wiki/Netzwerkprotokoll">Protokoll</a>, was bedeutet, dass der Server keine Daten (Zustände) zwischen zwei Anfragen behält.<br />
 <br />
 Obwohl oft auf einer TCP/IP Schicht aufgebaut, könnte es auch auf jede andere verlässliche, verbindungsorientierte <a href="https://de.wikipedia.org/wiki/OSI-Modell#Schicht_4_.E2.80.93_Transportschicht">Transportschicht</a> aufbauen, sofern sie Nachrichten nicht leise verliert, wie es zum Beispiel bei <a href="https://de.wikipedia.org/wiki/User_Datagram_Protocol">UDP</a> der Fall ist.</p>

<h2 class="Documentation" id="Documentation" name="Documentation">Dokumentation</h2>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Headers" title="/en-US/docs/HTTP/Headers">HTTP Headers</a></dt>
 <dd>HTTP message headers are used to precisely describe the resource being fetched or the behavior of the server or the client. Custom proprietary headers can be added using the 'X-' prefix; others are listed in an <a class="external" href="http://www.iana.org/assignments/message-headers/perm-headers.html" title="http://www.iana.org/assignments/message-headers/perm-headers.html">IANA registry</a>, whose original content was defined in <a class="external" href="http://tools.ietf.org/html/rfc4229" title="http://tools.ietf.org/html/rfc4229">RFC 4229</a>. IANA also maintain a <a class="external" href="http://www.iana.org/assignments/message-headers/prov-headers.html" title="http://www.iana.org/assignments/message-headers/prov-headers.html">registry of proposed new HTTP&nbsp;message headers</a>.</dd>
 <dt><a href="/en/Web_Development/HTTP_cookies" title="HTTP cookies">HTTP cookies</a></dt>
 <dd>How cookies work is defined by the <a class="external" href="http://tools.ietf.org/html/rfc6265">RFC 6265</a>. When receiving an HTTP request, a server can send a <code>Set-Cookie</code> header with the response. Afterward, the cookie value is sent along with every request made to the same server in the form of a <code>Cookie</code> HTTP header. Additionally, an expiration delay can be specified. Restrictions to a specific domain and path can be specified as well.</dd>
 <dt><a href="/en-US/docs/HTTP/Basic_access_authentication" title="/en-US/docs/HTTP/Basic_access_authentication">Basic access authentication</a></dt>
 <dd>In the context of an HTTP transaction, <strong>basic access authentication</strong> is a method for an <a href="https://developer.mozilla.org/en-US/docs/Web/API/window.navigator.userAgent" title="HTTP user agent">HTTP user agent</a> to provide a user name and password when making a request.</dd>
 <dt><a href="/en/HTTP_Pipelining_FAQ" title="https://developer.mozilla.org/en/HTTP_Pipelining_FAQ">HTTP pipelining FAQ</a></dt>
 <dd>HTTP/1.1 Pipelining FAQ</dd>
 <dt><a href="/en-US/docs/HTTP/Access_control_CORS" title="/en-US/docs/HTTP/Access_control_CORS">HTTP access control (CORS)</a></dt>
 <dd><strong>Cross-site HTTP requests</strong> are <a href="https://developer.mozilla.org/en/HTTP" title="en/HTTP">HTTP</a> requests for resources from a <strong>different domain</strong> than the domain of the resource making the request. &nbsp;For instance, a resource loaded from Domain A (<code><span class="nowiki">http://domaina.example</span></code>) such as an HTML web page, makes a request for a resource on Domain B (<span class="nowiki">http://domainb.foo</span>), such as an image, using the <code>img</code> element (<code><span class="nowiki">http://domainb.foo/image.jpg</span></code>).&nbsp; This occurs very commonly on the web today — pages load a number of resources in a cross-site manner, including CSS&nbsp;stylesheets, images and scripts, and other resources.</dd>
 <dt><a href="/En/Controlling_DNS_prefetching" title="En/Controlling DNS prefetching">Controlling DNS&nbsp;prefetching</a></dt>
 <dd>Firefox 3.5 performs <strong>DNS&nbsp;prefetching</strong>.&nbsp; This is a feature by which Firefox proactively performs domain name resolution on both links that the user may choose to follow as well as URLs for items referenced by the document, including images, CSS, JavaScript, and so forth. This prefetching is performed in the background, so that the DNS is likely to already have been resolved by the time the referenced items are actually needed.&nbsp; This reduces latency when, for example, the user actually clicks a link.</dd>
 <dt><a href="/en-US/docs/HTTP/HTTP_response_codes" title="/en-US/docs/HTTP/HTTP_response_codes">HTTP response codes</a></dt>
 <dd>HTTP&nbsp;Response Codes indicate whether a specific <a href="https://developer.mozilla.org/en/HTTP" title="en/HTTP">HTTP</a> requests has been successfully completed. Responses are grouped in five classes: informational responses, successful responses, redirections, client errors, and servers errors.</dd>
</dl>

<h2 id="A_brief_history_of_HTTP">A brief history of HTTP</h2>

<p>Since its original conception, as a protocol with one single method (GET) and returning only HTML pages, the HTTP protocol went through several revisions. The first documented version was HTTP/0.9 in 1991, corresponding to the original version. Very simple, it has a rudimentary search capability via the HTML&nbsp;{{ HTMLElement("isindex") }} element and an extension of the URL using the '<span style="font-family:Courier New">?</span>' character.</p>

<p>Then, in 1992, a version was published that became, with some minor changes, HTTP/1.0 (finalized in <a class="external" href="http://tools.ietf.org/html/rfc1945" title="http://tools.ietf.org/html/rfc1945">RFC 1945</a> in May 1996). One major improvement over the previous version was the ability to transmit files of different types, like images, videos, scripts, CSS documents, and so on, instead of only HTML files: this is achieved by using <a class="external" href="http://en.wikipedia.org/wiki/Mime_types" title="http://en.wikipedia.org/wiki/Mime_types">MIME types</a> in conjunction with the <code>Content-Type:</code> header.</p>

<p>In 1995, the <a class="external" href="http://www.ietf.org/" title="http://www.ietf.org/">IETF</a>&nbsp; began developing a new version of HTTP, which would become HTTP/1.1. It quickly spread into wide usage, and it was officially standardized in 1997 in <a class="external" href="http://tools.ietf.org/html/rfc2068" title="http://tools.ietf.org/html/rfc2068">RFC 2068</a>, with minor fixes in <a class="external" href="http://tools.ietf.org/html/rfc2616" title="http://tools.ietf.org/html/rfc2616">RFC 2616</a> two years later.</p>

<p>HTTP/1.1 brought the ability to reuse established connections for subsequent requests, greatly improving the performance of the protocol by lowering the latency between them; this is especially useful with complex HTML&nbsp;documents that need to fetch several subsequent files, like images or style sheets. It also brought the <code>Host:</code> header, which allows a single server, listening on a specific port, to receive requests for several websites; this paved the way for colocating numerous websites on one single server, greatly reducing the cost of hosting.</p>

<p>Since then, the HTTP protocol evolved by adding new <a href="/en/HTTP/Headers" title="en/HTTP/Headers">headers</a>, defining new behaviors without the need to fundamentally change the protocol. Unknown headers are simply ignored by servers or clients.</p>

<p>HTTP/1.1 is currently being revised by the <a class="external" href="http://tools.ietf.org/wg/httpbis/" title="http://tools.ietf.org/wg/httpbis/">IETF&nbsp;HTTPbis&nbsp;Working Group</a>.</p>

<h2 id="An_HTTP_session">An HTTP session</h2>

<p>Because HTTP is a client-server protocol, an HTTP session consists of three phases:</p>

<ol>
 <li>The client establishes a TCP connection (or the appropriate connection if the transport layer is not TCP).</li>
 <li>The client sends its request and then waits for the answer.</li>
 <li>The server processes the request and sends back its answer, containing a status code and the appropriate data.</li>
</ol>

<p>Starting with HTTP/1.1, the connection is no longer closed after the third phase, as the client is allowed to issue another request at this point: the second and third phases can therefore be done several times.</p>

<h3 id="Establishing_a_connection">Establishing a connection</h3>

<p>Because HTTP is a client-server protocol, it always is the client that establishes the connection. Opening a connection in&nbsp;HTTP really is establishing a connection in the underlying transport layer, usually TCP.</p>

<p>With TCP, the default port for an HTTP server on a computer is port 80, though others are often used, like 8000 or 8080. The URL of a page to fetch contains both the domain name and the port number, though the latter can be omitted if it is 80.</p>

<div class="note"><strong>Note:</strong> The client-server model does not allow the server to send data to the client without an explicit request of for it. To work around this problem, web developers use several techniques: pinging the server periodically via the <a href="/en/DOM/XMLHttpRequest" title="en/XMLHTTPRequest">XMLHTTPRequest</a> Javascript object, using the HTML <a href="/en/WebSockets" title="en/WebSockets">WebSockets API</a>, or similar protocols.</div>

<h3 id="Sending_a_client_request">Sending a client request</h3>

<p>Once the connection is established, the user-agent can send its request. (A user-agent is typically a web browser, but need not be.) A client request consists of text directives, separated by CRLF (carriage return, followed by line feed), divided in three blocks:</p>

<ol>
 <li>The first line contains a request method followed by its parameters:
  <ul>
   <li>the path of the document, i.e., an absolute URL without the protocol and the domain name</li>
   <li>the HTTP protocol version used</li>
  </ul>
 </li>
 <li>The subsequent lines each represent a specific HTTP&nbsp;header, giving the server some information about what kind of data is appropriate (e.g., what language, what MIME types) or some data altering its behavior (e.g., not sending an answer if it is already cached). These HTTP headers form a block that ends with an empty line.</li>
 <li>The final block is the optional data block, which contains further data and is mainly used by the POST method.</li>
</ol>

<h4 id="Examples_of_requests">Examples of requests</h4>

<ul>
 <li>Fetching the root page of developer.mozilla.org, i.e. <a class="linkification-ext external" href="/" title="Linkification: http://developer.mozilla.org/">http://developer.mozilla.org/</a>, and telling the server that the user-agent would prefer the page in French, if possible:

  <pre>
GET / HTTP/1.1
Host: developer.mozilla.org
Accept-Language: fr 

</pre>

  <p>Note the final empty line, separating the data block from the headers block. As there is no <code>Content-Length:</code> HTTP&nbsp;header, the data block is empty and the server can process the request as soon as it receives the empty line marking the end of the headers.</p>
 </li>
 <li>Sending the result of a form:
  <pre>
POST /contact_form.php HTTP/1.1
Host: developer.mozilla.org
Content-Length: 64
Content-Type: application/x-www-form-urlencoded

name=Joe%20User&amp;request=Send%20me%20one%20of%20your%20catalogue
</pre>
 </li>
</ul>

<h3 id="Structure_of_a_server_response">Structure of a server response</h3>

<p>After the connected agent has sent its request, the web server handles it, and finally sends a response back. Similarly to a client request, a server response is formed of text directives, separated by CRLF, though divided in three different blocks:</p>

<ol>
 <li>The first line, the <em>status line</em>, consists of an acknowledgment of the HTTP&nbsp;version used followed by a status request (and its meaning in human-readable text).</li>
 <li>The subsequent lines each represent a specific HTTP&nbsp;header giving the client some information about the data sent (e.g., type, data size, compression algorithm used, hints about caching). Similarly to the block of HTTP&nbsp;headers for a client request, these HTTP headers form a block that ends with an empty line.</li>
 <li>The final block is the data block, which contains the data (if any).</li>
</ol>

<h4 id="Examples_of_responses">Examples of responses</h4>

<ul>
 <li>Successful reception of a web page:
  <pre>
HTTP/1.1 200 OK
Date: Sat, 09 Oct 2010 14:28:02 GMT
Server: Apache
Last-Modified: Tue, 01 Dec 2009 20:18:22 GMT
ETag: "51142bc1-7449-479b075b2891b"
Accept-Ranges: bytes
Content-Length: 29769
Content-Type: text/html

&lt;!DOCTYPE html... <em><strong>(here comes the 29769 bytes of the requested web page)</strong></em>

</pre>
 </li>
 <li>Notification that the requested resource has been permanently moved:
  <pre>
HTTP/1.1 301 Moved Permanently
Server: Apache/2.2.3 (Red Hat)
Content-Type: text/html; charset=iso-8859-1
Date: Sat, 09 Oct 2010 14:30:24 GMT
Location: <a class="linkification-ext" href="../../../../" title="Linkification: https://developer.mozilla.org/">https://developer.mozilla.org/</a> <strong><em>(this is the</em><em> new link to the resource; it is expected that the user-agent will fetch it)</em></strong>
Keep-Alive: timeout=15, max=98
Accept-Ranges: bytes
Via: Moz-Cache-zlb05
Connection: Keep-Alive
X-Cache-Info: caching
X-Cache-Info: caching
Content-Length: 325 <em>(<strong>the content contains a default page to display if the user-agent is not able to follow the link)</strong></em>

&lt;!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN"&gt;
&lt;html&gt;&lt;head&gt;
&lt;title&gt;301 Moved Permanently&lt;/title&gt;
&lt;/head&gt;&lt;body&gt;
&lt;h1&gt;Moved Permanently&lt;/h1&gt;
&lt;p&gt;The document has moved &lt;a href="<a class="linkification-ext" href="../../../../" title="Linkification: https://developer.mozilla.org/">https://developer.mozilla.org/</a>"&gt;here&lt;/a&gt;.&lt;/p&gt;
&lt;hr&gt;
&lt;address&gt;Apache/2.2.3 (Red Hat) Server at developer.mozilla.org Port 80&lt;/address&gt;
&lt;/body&gt;&lt;/html&gt;
 
</pre>
 </li>
 <li>Notification that the requested resource doesn't exist:
  <pre>
HTTP/1.1 404 Not Found
Date: Sat, 09 Oct 2010 14:33:02 GMT
Server: Apache
Last-Modified: Tue, 01 May 2007 14:24:39 GMT
ETag: "499fd34e-29ec-42f695ca96761;48fe7523cfcc1"
Accept-Ranges: bytes
Content-Length: 10732
Content-Type: text/html

&lt;!DOCTYPE html... <strong><em>(contains a site-customized page helping the user to find the missing resource)</em></strong>

</pre>
 </li>
</ul>

<h3 id="Persistent_connections">Persistent connections</h3>

<p>Persistent connections were introduced in HTTP/1.1. They allow transmitting several requests on the same TCP connection (or on the specific connected transport layer if the HTTP&nbsp;is not built upon TCP/IP). This has several advantages:</p>

<ul>
 <li>Because the connection can be reused, requests can be <a href="/en/HTTP_Pipelining_FAQ" title="en/HTTP Pipelining FAQ">pipelined</a> to save part of the connection latency.</li>
 <li>By opening and closing fewer TCP connections, CPU&nbsp;time is saved.</li>
 <li>Network congestion is diminished by lowering the total amount of TCP&nbsp;packets (fewer opening and closing TCP&nbsp;packets).</li>
 <li>The TCP&nbsp;stack has more time to detect network congestion and to adapt its sending and receiving windows.</li>
 <li>HTTP&nbsp;is more adaptive: the cost for trying a feature is considerably lowered as an error response no longer leads to closing the connection.</li>
</ul>

<h2 id="HTTP_request_methods">HTTP request methods</h2>

<p>The request method indicates the action to be performed by the server. The HTTP/1.1 standard defines seven methods and allows other methods to be added later. Over the years, a few ones have been added in standards like <a href="/en/WebDAV" title="en/WebDAV">WebDAV</a>. The&nbsp; <a class="external" href="http://tools.ietf.org/wg/httpbis/" rel="external nofollow" target="_blank" title="http://tools.ietf.org/wg/httpbis/">IETF&nbsp;HTTPbis&nbsp;Working Group</a> is currently working on an IANA registry to list them all. If a server receives a request method that it doesn't know, it must return a <span style="font-family:Courier New"><a href="/en/HTTP/HTTP_response_codes#501" rel="internal" title="en/HTTP/HTTP response codes#501">501 Not implemented</a></span> response; if it knows the method but is configured not to answer it, it must return a <span style="font-family:Courier New"><a href="/en/HTTP/HTTP_response_codes#501" rel="internal" title="en/HTTP/HTTP response codes#501">405 Method not allowed</a></span> response. Two methods are required to be supported: HEAD&nbsp;and GET; all others are optional.</p>

<p>Two specific semantics are defined in the standard and are crucial for web developers: the <em>safety</em> property and the <em>idempotent</em> property.</p>

<h3 id="Safe_methods">Safe methods</h3>

<p>A <dfn>safe method</dfn> is a method that doesn't have any side-effects on the server. In other words, this property means that the method must be used only for <em>retrieval</em> of data. The safe HTTP methods defined in HTTP/1.1 are:</p>

<ul>
 <li>GET, used to retrieve information identified by the request URI. This information may be generated on the fly or the GET may be conditional if any of the {{ httpheader("If-Modified-Since") }}, {{ httpheader("If-Unmodified-Since") }}, {{ httpheader("If-Match") }}, {{ httpheader("If-None-Match") }} or {{ httpheader("If-Range") }} HTTP&nbsp;headers are set. In that latter case the information is only sent back if all the conditions are fulfilled.</li>
 <li>HEAD, which is identical to GET but without the message body sent.</li>
</ul>

<div class="note"><strong>Notes: </strong>

<ul>
 <li>Any safe method is also <em>idempotent</em>.</li>
 <li>Not having any side-effects means, for the GET method, that it&nbsp;<strong>must</strong> not be used to trigger an action outside the server, like an order in an e-commerce site. If a side-effect is wanted, a non-<em>idempotent</em> method should be used, like POST.</li>
 <li>When a page is generated on the fly by a script, the script engine may calculate the page as if it was requested by a GET and then strip the data block. This does not cause problem as long as the GET as implemented in the script is <em>safe</em>, but if it has any side-effects (like triggering an order on an e-commerce site), the HEAD method will trigger it too. It is up to the web developer to ensure that both the GET and HEAD method are safely implemented.</li>
</ul>
</div>

<h3 id="Idempotent_methods">Idempotent methods</h3>

<p>An <dfn>idempotent method</dfn> is a method such that the side-effects on the server of several identical requests with the method are the same as the side-effects of one single request.</p>

<ul>
 <li>HEAD and GET, like any safe method, are also idempotent, as a safe method doesn't have side-effects on the server.</li>
 <li>PUT is the way to upload a new resource on the server. If the resource already exists and is different, it is replaced; if it doesn't exist, it is created.</li>
 <li>DELETE removes a resource from the server.</li>
</ul>

<h3 id="Other_methods">Other methods</h3>

<ul>
 <li>POST is the way to trigger an action on the server. It has side-effects and can be used to trigger an order, to modify a database, to post a message in a forum, and so on.</li>
 <li>OPTIONS is a request for communication options available on the chain between the client and the server (through eventual proxies); this method is typically sent before any <a href="/En/HTTP_access_control#Preflighted_requests" title="en/HTTP access control#Preflighted requests">preflighted cross-origin request</a>, in order to know whether it is safe to do it.
  <div class="note"><strong>Note:</strong> <a href="/En/HTTP_access_control#Preflighted_requests" title="en/HTTP access control#Preflighted requests">Preflighted cross-origin requests</a> cannot be done on servers which don't allow or support the OPTIONS method.</div>
 </li>
 <li>TRACE is a kind of ping between the client and the server (through eventual proxies).</li>
</ul>

<p>Many more methods, such as PROPFIND or PATCH are defined in other standards-track RFCs of the IETF, like WebDAV.</p>

<p>The CONNECT method is defined in <a class="external" href="http://tools.ietf.org/html/rfc2817" title="http://tools.ietf.org/html/rfc2817">RFC&nbsp;2817</a>.</p>

<h3 id="HTTP_Requests_Methods_in_HTML_Forms">HTTP&nbsp;Requests Methods in&nbsp;HTML&nbsp;Forms</h3>

<p>In HTML, different HTTP&nbsp;request methods can be specified in the {{ htmlattrxref("method", "form") }} attribute of the {{ HTMLElement("form") }} element, but also to the {{ htmlattrxref("formmethod", "input") }} of the {{ HTMLElement("input") }} and {{ HTMLElement("button") }} elements. But not all HTTP methods can be used with these attributes; only GET and POST method are allowed by the HTML&nbsp;specification. See <a href="http://programmers.stackexchange.com/a/211790">this StackExchange answer why other HTTP request methods are not allowed by the HTML specification</a>.</p>

<div class="note"><strong>Note</strong>: The choice of a GET or POST method for HTML&nbsp;forms is not neutral. Because the GET method is a <a href="/en/HTTP#Safe_methods" title="https://developer.mozilla.org/en/HTTP#Safe_methods">safe method</a>, it should be used only in cases where no side-effect is expected; e.g., it shouldn't be used to transmit an order, as this order is a side-effect. In all cases where such side-effects are expected, the POST&nbsp;method should be used.</div>

<h2 id="HTTP_response_codes">HTTP response codes</h2>

<p>When answering a client request, the server sends back a three-digit number indicating whether the request was successfully processed. These codes can be grouped in five categories:</p>

<ul>
 <li><dfn>Informational responses</dfn> (of the form <code>1xx</code>) are provisional responses. Most of the time neither the end user, nor the web developer or webmaster should have to bother with these. The most common is the <span style="font-family:Courier New"><a href="/en/HTTP/HTTP_response_codes#100" title="en/HTTP/HTTP response codes#100">100 Continue</a></span> response, indicating that the client should continue to send its request.

  <div class="note"><strong>Note:</strong> No information response codes were defined in the HTTP/1.0, and therefore they must not be sent back when this version of the protocol is used.</div>
 </li>
 <li><dfn>Success responses</dfn> (of the form <code>2xx</code>) are for successfully processed requests. The <span style="font-family:Courier New"><a href="/en/HTTP/HTTP_response_codes#200" title="en/HTTP/HTTP response codes#200">200 OK</a></span>&nbsp;response is by far the most common of these responses, but the <span style="font-family:Courier New"><a href="/en/HTTP/HTTP_response_codes#206" title="en/HTTP/HTTP response codes#206">206 Partial Content</a></span> is also often seen when fetching a file or some media data like video or audio.</li>
 <li><dfn>Redirection responses</dfn> (of the form <code>3xx</code>) indicate that the resource that the client requested has moved and the server is not able to serve it directly. Most of these responses contain some location information telling where to find the requested resource; user-agents often then retrieve it without further user interaction. The most common responses of this type are <span style="font-family:Courier New"><a href="/en/HTTP/HTTP_response_codes#301" title="en/HTTP/HTTP response codes#301">301 Moved Permanently</a></span>, indicating that the URI given is no longer valid and has been moved to another place, and <span style="font-family:Courier New"><a href="/en/HTTP/HTTP_response_codes#302" title="en/HTTP/HTTP response codes#302">302 Found</a></span> which indicates that the resource has been <em>temporarily</em> moved to another place.
  <div class="note"><strong>Note:</strong> For webmasters, it is recommended to set up a <span style="font-family:Courier New"><a href="/en/HTTP/HTTP_response_codes#301" title="en/HTTP/HTTP response codes#301">301 Moved Permanently</a></span> redirection when moving pages to another URI, during a site reorganization for example. That allows users following links to still reach the resource and it also teaches search engines and other services the new location of the resource, so that they can transfer their metadata to it. It is also important to add adequate cache headers to the <span style="font-family:Courier New"><a href="/en/HTTP/HTTP_response_codes#301" title="en/HTTP/HTTP response codes#301">301 Moved Permanently</a></span> response so that this information is cached by the client and prevents it from making unnecessary requests to the original URI prior to fetching the resource itself.</div>
 </li>
 <li><dfn>Client error responses</dfn> (of the form <code>4xx</code>) indicate that the request sent by the client is either invalid, incomplete, or doesn't have enough rights to be performed. The most common such response is <span style="font-family:Courier New"><a href="/en/HTTP/HTTP_response_codes#404" title="en/HTTP/HTTP response codes#404">404 Not Found</a></span> which is sent back when the URI requested doesn't exist, but a few others are often presented to the end user, like <span style="font-family:Courier New"><a href="/en/HTTP/HTTP_response_codes#400" title="en/HTTP/HTTP response codes#400">400 Bad Request</a></span> sent when the request isn't a valid HTTP request (as this shouldn't happen but may indicate a bug into the user agent or, less likely, the server) or <span style="font-family:Courier New"><a href="/en/HTTP/HTTP_response_codes#403" title="en/HTTP/HTTP response codes#403">403 Forbidden</a></span>, sent when the client request a resource that does exist but isn't allowed to be transmitted (like a directory content).</li>
 <li><dfn>Server error responses</dfn> (of the form <code>5xx</code>) indicate that the server had a problem handling the valid client request. The two most common such responses are <span style="font-family:Courier New"><a href="/en/HTTP/HTTP_response_codes#500" title="en/HTTP/HTTP response codes#500">500 Internal Server Error</a></span>, a generic error code indicating a bug in the server or <span style="font-family:Courier New"><a href="/en/HTTP/HTTP_response_codes#503" title="en/HTTP/HTTP response codes#503">503 Service Unavailable</a></span> indicating that the server cannot process the request due to a temporary problem, like a disabled service for maintenance purposes or the non-availability of a database.</li>
</ul>

<p>A web developer shouldn't encounter many other response codes, but people building requests using the <code><a href="/en/nsIXMLHttpRequest" title="en/XMLHttpRequest">XMLHTTPRequest</a></code> function may hit <a href="/en/HTTP/HTTP_response_codes" title="en/HTTP/HTTP response codes">less usual response codes</a>.</p>

<h3 id="More_on_redirection_responses">More on redirection responses</h3>

<p>Starting in Gecko 9.0 {{ geckoRelease("9.0") }}, redirections (such as 301 and 307) that specify a <code>javascript:</code> URI are no longer performed. Instead, a bad connection error is presented. This helps avoid cross-site scripting attacks. See {{ bug(255119) }} if you want more details.</p>

<h2 id="HTTP_headers">HTTP headers</h2>

<p>HTTP headers allow the client and the server to pass additional information with the request or the response. A request header consists of its case-insensitive name followed by a colon ':', then by its value (without CRLF in it). Leading white space before the value is ignored.</p>

<p>Headers are grouped according the context in which they may appear:</p>

<dl>
 <dt>General headers</dt>
 <dd>These headers apply to both requests and responses but are unrelated to the data eventually transmitted in the body. They therefore apply only to the message being transmitted. There are only a few of them and new ones cannot been added without increasing the version number of the HTTP&nbsp;protocol. The exhaustive list for HTTP/1.1 is {{ httpheader("Cache-Control") }}, {{ httpheader("Connection") }}, {{ httpheader("Date") }}, {{ httpheader("Pragma") }}, {{ httpheader("Trailer") }}, {{ httpheader("Transfer-Encoding") }}, {{ httpheader("Upgrade") }}, {{ httpheader("Via") }} and {{ httpheader("Warning") }}.</dd>
 <dt>Request headers</dt>
 <dd>These headers give more precise information about the resource to be fetched or about the client itself. Among them one find <a href="/en/HTTP_Caching_FAQ" title="en/HTTP Caching FAQ">cache-related headers</a>, transforming a GET method in a conditional GET, like {{ httpheader("If-Modified-Since") }}, user-preference information like {{ httpheader("Accept-Language") }} or {{ httpheader("Accept-Charset") }} or plain client information like {{ httpheader("User-Agent") }}. New request headers cannot officially be added without increasing the version number of the HTTP protocol. But, it is common for new request headers to be added if both the server and the client agree on their meaning. In that case, a client should not assume that they will be handled adequately by the server; unknown request headers are handled as <em>entity headers</em>.</dd>
 <dt>Response headers</dt>
 <dd>These headers give more information about the resource sent back, like its real location ({{ httpheader("Location") }}) or about the server itself, like its name and version ({{ httpheader("Server") }}). New response headers cannot be added without increasing the version number of the HTTP protocol. But, it is common for new response headers to be added if both the server and the client agree on their meaning. In that case, a server should not assume that they will be handled adequately by the client ; unknown response headers are handled as <em>entity headers</em>.</dd>
 <dt>Entity headers</dt>
 <dd>These headers give more information about the body of the entity, like its length ({{ httpheader("Content-Length") }}), an identifying hash ({{ httpheader("Content-MD5") }}), or its MIME-type ({{ httpheader("Content-Type") }}). New entity headers can be added without increasing the version number of the HTTP protocol.</dd>
</dl>

<p>Headers can also be grouped according to how caching and non-caching proxies handle them:</p>

<dl>
 <dt>End-to-end headers</dt>
 <dd>These headers must be transmitted to the final recipient of the message; that is, the server for a request message or the client for a response message. Such a header means that intermediate proxies must retransmit it unmodified and also that caches must store it.</dd>
 <dt>Hop-by-hop headers</dt>
 <dd>These headers are meaningful only for a single transport-level connection and must not be retransmitted by proxies or cached. Such headers are: {{ httpheader("Connection") }}, {{ httpheader("Keep-Alive") }}, {{ httpheader("Proxy-Authenticate") }}, {{ httpheader("Proxy-Authorization") }}, {{ httpheader("TE") }}, {{ httpheader("Trailers") }}, {{ httpheader("Transfer-Encoding") }} and {{ httpheader("Upgrade") }}. Note that only hop-by-hop headers may be set using the {{ httpheader("Connection") }} general header.</dd>
</dl>

<p>In order to learn about the specific semantic of each header, see its entry in the <a href="/en/HTTP/Headers" title="en/HTTP/Headers">comprehensive list of HTTP&nbsp;headers</a>.</p>

<h3 id="Useful_request_headers">Useful request headers</h3>

<p>Among the numerous <a href="/en/HTTP/Headers" title="en/HTTP/Headers">HTTP request headers</a>, several are especially useful when set correctly. If you are building your own requests, by using <code><a href="/en/DOM/XMLHttpRequest" title="en/XMLHTTPRequest">XMLHTTPRequest</a></code> or when writing an extension and sending <a href="/en/Setting_HTTP_request_headers" title="en/Setting HTTP request headers">custom HTTP requests via XPCOM</a>, then it is important to ensure the presence of headers that are often set by browsers based on the preferences of the user.</p>

<dl>
 <dt>Controlling the language of the resource</dt>
 <dd>Most user-agents, like Firefox, allow the user to set a preference for the language for receiving a resource. The browser translate this into an {{ httpheader("Accept-Language") }} header. It is good practice for web developers, when building specific HTTP&nbsp;requests, to include such a header too.</dd>
 <dt>Using conditional GET</dt>
 <dd>Caching is a major tool to accelerate the display of web pages. Even when parts of a webpage are refreshed via an&nbsp;<code><a href="/en/DOM/XMLHttpRequest" title="en/XMLHTTPRequest">XMLHTTPRequest</a></code>:, it is a good idea to use the {{ httpheader("If-Modified-Since") }} header (and other similar ones) in order to fetch the new content only if it has changed. This approach lowers the burden on the network.</dd>
</dl>

<h3 id="Useful_response_headers">Useful response headers</h3>

<p>The configuration of a web server is a critical part to ensure good performance and optimal security of a web site. Among the <a href="/en/HTTP/Headers" title="en/HTTP/Headers">numerous HTTP response headers</a>, several are of specific importance and should be configured on the server</p>

<h4 id="Restricting_framing">Restricting framing</h4>

<p>Several cross-site scripting (XSS) attacks take advantage of the ability to put third-party content inside an {{ HTMLElement("frame") }} or {{ HTMLElement("iframe") }}. In order to mitigate that risk, modern browsers have introduced the <code><a href="/en/Security/CSP/CSP_policy_directives#frame-ancestors" title="en/The X-FRAME-OPTIONS response header">CSP frame-ancestors directive</a></code>. By setting it with the value <code>'none'</code>, it prevents the browser from displaying this resource inside of a frame. Using it on critical resources (like those containing a formularies or critical information) will reduce the risk caused by XSS attacks. Note that this specific HTTP response header is not the only way to mitigate XSS risks; other techniques, like setting some <a href="/en/Security/CSP/Introducing_Content_Security_Policy" title="en/Security/CSP/Introducing Content Security Policy">Content Security Policies</a>, may be helpful too.</p>

<h4 id="Compression">Compression</h4>

<p>Minimizing the amount of data transferred accelerates the display of a web page. Though most techniques, like <a href="/en/CSS/CSS_Sprites" title="en/CSS/CSS Sprites">CSS Sprites</a>, should be applied on the site itself, compression of data must be set at the web server level. If set, resources requested by the client with an {{ httpheader("Accept-Encoding") }} request header are compressed using the appropriate method and sent back with a {{ httpheader("Content-Encoding") }} response header. Setting these in Apache 2 servers is done by using the <a class="external" href="http://httpd.apache.org/docs/2.0/mod/mod_deflate.html" title="http://httpd.apache.org/docs/2.0/mod/mod_deflate.html">mod_deflate module</a>.</p>

<div class="note"><strong>Note:</strong> Be aware that not all data formats can be efficiently compressed. Already-compressed media data, like JPEG images or most audio and video formats, do not shrink using another pass of compression. In fact, they often become larger due to the overhead of the compression method. It is important not to try to compress these resource types any further; there is no advantage in size and the compression/decompression mechanism is resource-intensive.</div>

<h4 id="Controlling_cache">Controlling cache</h4>

<p><a href="/en/HTTP_Caching_FAQ" title="en/HTTP Caching FAQ">HTTP&nbsp;Caching</a> is a technique that prevents the same resource from being fetched several times if it hasn't change. Configuring the server with the correct response headers allows the user-agent to adequately cache the data. In order to do that, be sure that:</p>

<ul>
 <li>Any static resource provides an {{ httpheader("Expires") }} response header that is set to far in the future. That way, the resource may stay in the cache until the user-agent flushes it for its own reasons (like reaching its cache size limit).
  <div class="note"><strong>Note:&nbsp;</strong>On Apache, use the ExpiresDefault directive in your .htaccess to define a relative expires: <code>ExpiresDefault "access plus 1 month"</code>.</div>
 </li>
 <li>Any dynamic resource provides a {{ httpheader("Cache-control") }} response header. Theoretically, any HTTP request done through a <a href="/en/HTTP#Safe_Methods" title="en/HTTP#Safe Methods">safe method</a> (GET or HEAD) or even through a solely <a href="/en/HTTP#Idempotent_Methods" title="en/HTTP#Idempotent Methods">idempotent one</a> (DELETE, PUT) may be cached; but in practice careful study is needed to determine if the caching of the response may lead to inappropriate side-effects.</li>
</ul>

<h4 id="Setting_the_correct_MIME_types">Setting the correct MIME types</h4>

<p>The MIME type is the mechanism to tell the client the kind of document transmitted: the extension of a file name has no meaning on the web. It is therefore important that the server is correctly set up so that the correct MIME&nbsp;type is transmitted with each document: user-agents often use this MIME-type to determine what default action to do when a resource is fetched.</p>

<div class="note"><strong>Note: </strong>

<ul>
 <li>On Apache, one can match file extensions with a given MIME type in the .htaccess using the <font face="Verdana,Helvetica,Arial"><span style="font-family:Courier New"><code>AddType</code></span> type directive like</font><code> AddType image/jpeg jpg.</code></li>
 <li>Most web servers send unknown-type resources using the default <code>application/octet-stream</code> MIME&nbsp;type; for security reasons, most browsers, like Firefox, do not allow setting a custom default action for such resources and force the user to store it to disk in order to use it. Some common cases of often incorrectly configured servers happens for the following file types:
  <ul>
   <li>
    <p>Rar-encoded files. The ideal would be to be able to set the real type of the encoded files; this often is not possible (as it may not be known to the server and these files may contains several resource of different types). In that case, configure the server to send the <code>application/x-rar-compressed </code>MIME type or some users won't be able to define a useful default action for them.</p>
   </li>
   <li>
    <p>Audio and video files. Only resources with the proper MIME&nbsp;Type will be recognized and played, using a {{ HTMLElement("video") }} or {{ HTMLElement("audio") }} elements. Be sure to <a href="/En/Media_formats_supported_by_the_audio_and_video_elements" title="En/Media formats supported by the audio and video elements">use the correct MIME type for audio and video resources</a>.</p>
   </li>
   <li>
    <p>Proprietary file types. Pay special attention when serving a proprietary file type. Be sure not to forget to add an x-prefixed type for it; otherwise, special handling won't be possible. This is especially true with resources using the <a class="external" href="http://en.wikipedia.org/wiki/Keyhole_Markup_Language" title="http://en.wikipedia.org/wiki/Keyhole_Markup_Language">Keyhole Markup Language</a>, which should be served as <code>application/vnd.google-earth.kml+xml </code>for an optimal user experience.</p>
   </li>
  </ul>
 </li>
</ul>
</div>

<h2 id="See_also">See also</h2>

<ul>
 <li><a href="/En/Controlling_DNS_prefetching" title="En/Controlling DNS prefetching">Controlling DNS&nbsp;prefetching</a></li>
 <li>The <a href="/en/HTTP_Pipelining_FAQ" title="https://developer.mozilla.org/en/HTTP_Pipelining_FAQ">HTTP pipelining FAQ</a></li>
 <li><a href="/en/Web_Development/HTTP_cookies" title="HTTP cookies">HTTP cookies</a></li>
 <li><a href="/en-US/docs/HTTP/Headers" title="/en-US/docs/HTTP/Headers">HTTP Headers</a></li>
 <li><a href="/en-US/docs/HTTP/Basic_access_authentication" title="/en-US/docs/HTTP/Basic_access_authentication">Basic access authentication</a></li>
 <li><a href="/en-US/docs/HTTP/Access_control_CORS" title="/en-US/docs/HTTP/Access_control_CORS">HTTP access control (CORS)</a></li>
</ul>

<p>{{ languages( { "ja": "ja/HTTP"} ) }}</p>

