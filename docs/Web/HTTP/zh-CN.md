---
version: prototype1
revision_id: 1283625
locale: zh-CN
slug: Web/HTTP
tags: "HTTP" "参考" "Web"
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

<p class="summary">超文本传输​​协议（HTTP）是用于传输诸如HTML的超媒体文档的<a href="https://en.wikipedia.org/wiki/Application_Layer">应用层协议</a>。它被设计用于Web浏览器和Web服务器之间的通信，但它也可以用于其他目的。 HTTP遵循经典的<a href="https://en.wikipedia.org/wiki/Client%E2%80%93server_model">客户端-服务端模型</a>，客户端打开一个连接以发出请求，然后等待它收到服务器端响应。 HTTP是<a href="http://en.wikipedia.org/wiki/Stateless_protocol">无状态协议</a>，意味着服务器不会在两个请求之间保留任何数据（状态）。虽然通常基于TCP / IP层，但可以在任何可靠的<a href="https://zh.wikipedia.org/wiki/%E4%BC%A0%E8%BE%93%E5%B1%82">传输层</a>上使用;也就是说，一个不会静默丢失消息的协议，如UDP。</p>

<div class="column-container">
<div class="column-half">
<h2 id="教程">教程</h2>

<p>通过以下指南和教程来学习如何使用 HTTP。</p>

<dl>
 <dt><a href="/zh-CN/docs/Web/HTTP/Overview">HTTP 概述</a></dt>
 <dd>介绍了客户端-服务器端协议的基本特征：它能够做什么以及它的设计意图。</dd>
 <dt><a href="/zh-CN/docs/Web/HTTP/Caching">HTTP 缓存</a></dt>
 <dd>缓存对高速 Web 站点来说是非常之重要的。这篇文章阐述了不同种类的缓存以及如何配置 HTTP 首部来控制它们。</dd>
 <dt><a href="/zh-CN/docs/Web/HTTP/Cookies">HTTP Cookie</a></dt>
 <dd><a class="external" href="http://tools.ietf.org/html/rfc6265">RFC 6265</a>&nbsp;定义了 cookies 是怎样工作的。&nbsp;当接收到一个 HTTP请求时，服务器可以在响应中发送一个 Set-Cookie 首部字段。接着，对于同一台服务器发起的每一个请求，客户端都会在 HTTP 请求头中以字段 Cookie 的形式将 cookie 的值发送过去。&nbsp;此外，还可以指定一个过期时间，也可以指定一个特定的域名和路径中使用。</dd>
 <dt><a href="/zh-CN/docs/Web/HTTP/Access_control_CORS">HTTP 访问控制（CORS） </a></dt>
 <dd><strong>跨站&nbsp;HTTP 请求</strong>就是从<strong>另一个域名</strong>，而不是资源所在的域名发起的 HTTP 请求。举例来说，在域名&nbsp;A&nbsp;(<code>http://domaina.example/</code>) 的 HTML 页面上使用 <code>img</code>&nbsp;元素 (&lt;img src="<code>http://domainb.foo/image.jpg"&gt;</code>) 来请求域名 B&nbsp;(http://domainb.foo/) 上的图片资源。这在当前的 web 页面上很常见 —— 页面通过跨域规则加载 CSS 样式表，图片，脚本以及其他资源。</dd>
 <dt><a href="/zh-CN/docs/Web/HTTP/Basics_of_HTTP/Evolution_of_HTTP">HTTP 的演变</a></dt>
 <dd>简单描述了从早期版本的 HTTP 到现在的 HTTP/2 以及未来的 HTTP 这个过程中发生的变更。</dd>
 <dt><a href="https://wiki.mozilla.org/Security/Guidelines/Web_Security">Mozilla web&nbsp;安全引导</a></dt>
 <dd>一系列用于帮助运营团队创建安全的 Web 应用程序的提示。</dd>
 <dt><a href="/zh-CN/docs/Web/HTTP/Messages">HTTP 消息 </a></dt>
 <dd>描述了 HTTP/1.x 和 HTTP/2.x 中不同种类消息的类型和结构。</dd>
 <dt><a href="/zh-CN/docs/Web/HTTP/Session">典型的 HTTP 会话 </a></dt>
 <dd>展现并解释了一个常见的 HTTP 会话流程。</dd>
 <dt><a href="/zh-CN/docs/Web/HTTP/Connection_management_in_HTTP_1.x">HTTP/1.x中的连接管理 </a></dt>
 <dd>描述了在 HTTP/1.x 中的三种连接管理模型，以及它们的优势和劣势。</dd>
</dl>
</div>

<div class="column-half">
<h2 id="参考">参考</h2>

<p>浏览详细的 HTTP 参考文档。</p>

<dl>
 <dt><a href="/zh-CN/docs/Web/HTTP/Headers">HTTP 首部</a></dt>
 <dd>HTTP 消息首部被用来描述资源信息，或是客户端和服务器的行为。自定义的专有首部可以加上 'X-' 前缀; &nbsp;其他的可以在&nbsp;<a class="external" href="http://www.iana.org/assignments/message-headers/perm-headers.html">IANA registry</a>&nbsp;找到，其原始定义在&nbsp;<a class="external" href="http://tools.ietf.org/html/rfc4229">RFC 4229</a>。IANA 同时也维护着一份&nbsp;<a class="external" href="http://www.iana.org/assignments/message-headers/prov-headers.html">registry of proposed new HTTP message headers</a>。</dd>
 <dt><a href="/zh-CN/docs/Web/HTTP/Methods">HTTP 请求方法 </a></dt>
 <dd>可以使用 HTTP: {{HTTPMethod("GET")}}，{{HTTPMethod("POST")}} 方法来完成不同操作，同时也有一些其他的方法，如 {{HTTPMethod("OPTIONS")}}，{{HTTPMethod("DELETE")}} 和&nbsp;{{HTTPMethod("TRACE")}}。</dd>
 <dt><a href="/zh-CN/docs/Web/HTTP/Response_codes">HTTP 状态返回码 </a></dt>
 <dd>HTTP 状态返回码用来表示指定的 HTTP 请求是否成功完成。响应被分为 5 种类型: 消息型响应，成功响应，重定向，客户端错误和服务器错误。</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Security-Policy">CSP 指令</a></dt>
 <dd>{{HTTPHeader("Content-Security-Policy")}} 响应头字段允许站点的管理者控制页面上哪些资源能够被用户代理程序加载。除了少数例外，此策略主要涉及源服务器和脚本终端。</dd>
</dl>

<h2 id="工具与资源">工具与资源</h2>

<p>有助于理解和调试&nbsp;HTTP 连接的工具和资源。</p>

<dl>
 <dt><a href="/zh-CN/docs/Tools">Firefox 开发者工具 </a></dt>
 <dd><a href="/zh-CN/docs/Tools/Network_Monitor">网络监视器</a></dd>
 <dt><a href="https://observatory.mozilla.org/">Mozilla Observatory</a></dt>
 <dd>
 <p>一个旨在帮助开发人员，系统管理员和安全专业人员安全地配置其网站的项目。</p>
 </dd>
 <dt><a href="https://redbot.org/">RedBot</a></dt>
 <dd>检查 Cache 相关 HTTP 首部的工具.</dd>
 <dt><a href="http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/">浏览器的工作原理</a></dt>
 <dd>一篇非常全面的关于浏览器内部实现与通过 HTTP 协议的请求流的文章。是所有 web 开发者的必读内容。</dd>
</dl>
</div>
</div>

