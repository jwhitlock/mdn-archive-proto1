---
version: prototype1
revision_id: 1307569
locale: ar
slug: Web/HTTP
tags: 
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

<p class="summary" dir="rtl"><strong>بروتوكول نقل النص التشعبي Hypertext Transfer Protocol أو ما&nbsp;</strong>يعرف إختصاراً بـ (<strong>HTTP</strong>) هو عبارة عن بروتوكول من نوع طبقة التطبيقات (<strong>Application-layer</strong>) مهمّته نقل مستندات الوسائط الفائقة، على سبيل المثال <strong>HTML</strong>. صُمّمَ للتواصل فيما بين متصفّحات الويب (<strong>web browsers</strong>) وخوادم الويب (<strong>web servers</strong>) لكن أيضاً يُمكن إستخدامه لأغراضٍ أُخرى. يتبع <strong>HTTP</strong> ما يعرف بـ <a href="https://ar.wikipedia.org/wiki/%D9%86%D9%85%D9%88%D8%B0%D8%AC_%D8%B7%D9%84%D8%A8_%D8%A7%D9%84%D8%AE%D8%AF%D9%85%D8%A9">نموذج العميل/الخادم</a>&nbsp;(<strong>client-server model</strong>) حيث يقوم بإرسال طلب (<strong>request</strong>) ثم ينتظر&nbsp;ليتلقّى إجابة (<strong>response</strong>) على هذا الطلب. <strong>HTTP</strong> هو بروتوكول <a href="https://ar.wikipedia.org/wiki/%D8%A8%D8%B1%D9%88%D8%AA%D9%88%D9%83%D9%88%D9%84_%D8%B9%D8%AF%D9%8A%D9%85_%D8%A7%D9%84%D8%AD%D8%A7%D9%84%D8%A9">عديم الحالة</a> (<strong>stateless protocol</strong>) هذا يعني أن الخادم (<strong>server</strong>) لن يحتفظ بأيّ بيانات (حالة) عن الطلبات. بالرغم من أنَّ HTTP مبني على طبقة <strong>TCP/IP</strong> إلّا أنّه يمكن إستخدامه على أي<a href="https://ar.wikipedia.org/wiki/%D8%B7%D8%A8%D9%82%D8%A9_%D8%A7%D9%84%D9%86%D9%82%D9%84"> طبقة نقل</a> موثوقة؛ هذا هو، بروتوكول لن يفقد الرسائل بصمت كما يفعل <strong>UDP</strong>.</p>

<div class="column-container">
<div class="column-half">
<h2 id="الدروس">الدروس</h2>

<p>دروس وإرشادات لتعليم كيفية إستخدام HTTP.</p>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview">لمحة عن HTTP</a></dt>
 <dd>The basic features of the client-server protocol: what it can do and its intended uses.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Caching">HTTP Cache</a></dt>
 <dd>Caching is very important for fast Web sites. This article describes different methods of caching and how to use HTTP Headers to control them.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies">HTTP Cookies</a></dt>
 <dd>How cookies work is defined by&nbsp;<a href="http://tools.ietf.org/html/rfc6265">RFC 6265</a>. When serving an HTTP request, a server can send a&nbsp;<code>Set-Cookie</code>&nbsp;HTTP header with the response. The client then returns the cookie's value with every request to the same server in the form of a&nbsp;<code>Cookie</code>&nbsp;request header. The cookie can also be set to expire on a certain date, or restricted to a specific domain and path.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Access_control_CORS">HTTP Access Control (CORS)</a></dt>
 <dd><strong>Cross-site HTTP requests</strong>&nbsp;are HTTP requests for resources from a <strong>different domain</strong> than the domain of the resource making the request. For instance, an HTML page from Domain A (<code>http://domaina.example/</code>) makes a request for an image on Domain B (<code>http://domainb.foo/image.jpg</code>) via the&nbsp;<code>img</code>&nbsp;element. Web pages today very commonly load cross-site resources, including CSS stylesheets, images, scripts, and other resources. CORS allows web developers to control how their site reacts to cross-site requests.</dd>
</dl>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/Evolution_of_HTTP">Evolution of HTTP</a></dt>
 <dd>A brief description of the changes between the early versions of HTTP, to the modern HTTP/2 and beyond.</dd>
 <dt><a href="https://wiki.mozilla.org/Security/Guidelines/Web_Security">Mozilla web security guidelines</a></dt>
 <dd>A collection of tips to help operational teams with creating secure web applications.</dd>
</dl>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">HTTP Messages</a></dt>
 <dd>Describes the type and structure of the different kind of messages of HTTP/1.x and HTTP/2.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Session">A typical HTTP session</a></dt>
 <dd>Shows and explains the flow of a usual HTTP session.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Connection_management_in_HTTP_1.x">Connection management in HTTP/1.x</a></dt>
 <dd>Describes the three connection management models available in HTTP/1.x, their strengths, and their weaknesses.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="المراجع">المراجع</h2>

<p>تصفَّح وثائق HTTP المرجعيَّة المفصَّلة</p>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers">HTTP Headers</a></dt>
 <dd>HTTP message headers are used to describe a resource, or the behavior of the server or the client. Custom proprietary headers can be added using the&nbsp;<code>X-</code>&nbsp;prefix; others in an&nbsp;<a href="http://www.iana.org/assignments/message-headers/perm-headers.html">IANA registry</a>, whose original content was defined in&nbsp;<a href="http://tools.ietf.org/html/rfc4229">RFC 4229</a>. IANA also maintains a&nbsp;<a href="http://www.iana.org/assignments/message-headers/prov-headers.html">registry of proposed new HTTP message headers</a>.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods">HTTP Request Methods</a></dt>
 <dd>The different operations that can be done with HTTP: {{HTTPMethod("GET")}}, {{HTTPMethod("POST")}}, and also less common requests like {{HTTPMethod("OPTIONS")}}, {{HTTPMethod("DELETE")}}, or {{HTTPMethod("TRACE")}}.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Response_codes">HTTP Status Response Codes</a></dt>
 <dd>HTTP response codes indicate whether a specific HTTP request has been successfully completed. Responses are grouped in five classes: informational responses, successful responses, redirections, client errors, and servers errors.</dd>
</dl>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Headers/Content-Security-Policy">CSP directives</a></dt>
 <dd>The {{HTTPHeader("Content-Security-Policy")}} response header fields allows web site administrators to control resources the user agent is allowed to load for a given page. With a few exceptions, policies mostly involve specifying server origins and script endpoints.</dd>
</dl>

<h2 id="Tools_resources">الأدوات والموارد</h2>

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

