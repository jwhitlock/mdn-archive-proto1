---
version: prototype1
revision_id: 1274571
locale: vi
slug: Web/HTTP
tags: "HTTP" "Web" "TopicStub" "Reference" "l10n:priority" "NeedsTranslation"
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

<p class="summary"><strong><dfn>Hypertext Transfer Protocol (HTTP)</dfn></strong>&nbsp;là một giao thức thuộc&nbsp;<a href="https://vi.wikipedia.org/wiki/T%E1%BA%A7ng_%E1%BB%A9ng_d%E1%BB%A5ng">tầng ứng dụng</a> được dùng để truyền tải các tài liệu đa phương tiện, ví dụ như HTML. Giao thức này được thiết kế để truyền thông giữa các trình duyệt web và máy chủ web, tuy nhiên nó cũng được dùng cho nhiều mục đích khác. HTTP tuân theo một&nbsp;<a href="https://vi.wikipedia.org/wiki/Client-server">mô hình client-server</a>&nbsp;truyền thống, với một client mở một kết nối (connection) để tạo ra một yêu cầu (request), sau đó chờ đợi cho đến khi nó nhận được phản một phản hồi (response). HTTP là một giao thức không lưu lại trạng thái (<a href="https://en.wikipedia.org/wiki/Stateless_protocol">stateless protocol</a>), có nghĩa là máy chủ không lưu giữ bất cữ dữ liệu (state) gì giữa các yêu cầu. Bởi thường được dựa trên một lớp TCP/IP, nó có thể được sử dụng trên bất cứ <a href="https://vi.wikipedia.org/wiki/T%E1%BA%A7ng_giao_v%E1%BA%ADn">tầng giao vận</a> đáng tin cậy nào&nbsp;(reliable transport layer)&nbsp;- những giao thức không bị mất dữ liệu, như là UDP.</p>

<div class="column-container">
<div class="column-half">
<h2 id="Tutorials">Hướng dẫn</h2>

<p>Learn how to use HTTP with guides and tutorials.</p>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Overview">Tổng quan về HTTP</a></dt>
 <dd>Các chức năng cơ bản của giao thức client-server: nó có thể làm gì và mục đích sử dụng của nó.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Caching">HTTP Cache</a></dt>
 <dd>Caching rất quan trọng với tốc độ của các trang web. Bài viết này mô tả các cách thức cache khác nhau cũng như cách sử dụng HTTP Headers để điều khiển chúng.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Cookies">HTTP Cookies</a></dt>
 <dd>Cookies hoạt động như thế nào được định nghĩa trong&nbsp;<a class="external" href="http://tools.ietf.org/html/rfc6265">RFC 6265</a>. Khi phục vụ một yêu cầu HTTP (HTTP request), một máy chủ (server) có thể gửi một&nbsp;<code>Set-Cookie</code> HTTP header đính kèm trong phản hồi (response). Máy khách (client) sau đó sẽ gửi trả&nbsp;giá trị của cookie trong mỗi yêu cầu đến máy chủ&nbsp;(server) đó trong Cookie header của yêu cầu (request). Cookie cũng có thể được quy định ngày hết hạn hoặc hạn chế với một tên miền và đường dẫn.</dd>
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

