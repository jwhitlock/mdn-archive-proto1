---
version: prototype1
revision_id: 1309101
locale: zh-CN
slug: Web/HTML
tags: "HTML" "HTML5" "HTML教程" "元素" "参考" "超文本" "Web"
title: HTML（超文本标记语言）
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>{{HTMLSidebar}}</p>

<p class="summary"><span class="seoSummary"><strong>HTML</strong>（超文本标记语言——HyperText Markup Language）是构成Web世界的基石。它描述并定义了一个网页的内容。其他除HTML以外的技术则通常用来描述一个网页的表现／展示效果（<a href="/zh-CN/docs/Web/CSS">CSS</a>）或功能（<a href="/zh-CN/docs/Web/JavaScript">JavaScript</a>）。</span></p>

<p>“超文本”是指在单个网站内或网站之间将网页彼此连接的链接。链接是网络的基础。只要将内容上传到互联网，并将其与他人创建的页面相链接，你就成为了万维网的积极参与者。</p>

<p>HTML使用“标记”来注明文本、图片和其他内容，以便于在Web浏览器中显示。HTML标记包含一些特殊“元素”如{{HTMLElement("head")}}，{{HTMLElement("title")}}，{{HTMLElement("body")}}，{{HTMLElement("header")}}，{{HTMLElement("footer")}}，{{HTMLElement("article")}}，{{HTMLElement("section")}}，{{HTMLElement("p")}}，{{HTMLElement("div")}}，{{HTMLElement("span")}}，{{HTMLElement("img")}}等等。</p>

<p>下面的文章会帮助你更好的了解HTML：</p>

<section class="cleared" id="sect1">
<ul class="card-grid">
 <li><span>HTML介绍</span>

  <p>如果您是Web开发新手，请务必阅读我们的<a href="/zh-CN/docs/Web/HTML/Introduction">HTML基础</a>以了解什么是HTML以及如何使用它。</p>
 </li>
 <li><span>HTML指南</span>
  <p>查看我们的<a href="/zh-CN/docs/Web/Guide/HTML">HTML学习区</a>来了解如何使用HTML，以及教程和完整的示例。</p>
 </li>
 <li><span>HTML参考</span>
  <p>在我们丰富的<a href="/zh-CN/docs/Web/HTML/Reference">HTML参考</a>中，你可以找到所有HTML元素和属性的详细信息。</p>
 </li>
</ul>

<div class="row topicpage-table">
<div class="section">
<h2 class="Tools" id="Tools" name="Tools">初学者教程</h2>

<p>我们的<a href="/zh-CN/docs/Learn/HTML">HTML学习区</a>含有许多富有特色的模块，可以在不需学习者掌握任何先前经验的情况下，令其从零开始，掌握HTML。</p>

<dl>
 <dt><a href="/zh-CN/docs/Learn/HTML/Introduction_to_HTML">HTML介绍</a></dt>
 <dd>这一模块将为你打下基础，并为进一步的学习铺平道路。在这里，你将掌握并适应一些重要的概念和语法，学习如何使文本与HTML相搭配、如何创建超链接以及运用HTML去构建一个网页。</dd>
 <dt><a href="/zh-CN/docs/Learn/HTML/Multimedia_and_embedding">多媒体与嵌入内容</a></dt>
 <dd>这个模块将带领你探索如何使用HTML在你的页面中包含多媒体内容，包括通过许多不同的方式嵌入图片，以及如何嵌入视频、音频甚至一整个其他页面。</dd>
 <dt><a href="/zh-CN/docs/Learn/HTML/Tables">HTML表格</a></dt>
 <dd>如何以一个可理解并易于访问的形式在网页中展示一个表格化数据一向都是个不小的挑战。这个模块涵盖了基本的表格table标记，以及一些更复杂的特性，比如使用标题和总结等。</dd>
 <dt><a href="/zh-CN/docs/Learn/HTML/Forms">HTML表单</a></dt>
 <dd>表单是构成Web世界的重要组成部分——他们提供了大量的你所需要用来与网站进行交互所需的功能。比如注册、登录、发送评论反馈、购买商品等等。这个模块将带领你建立一个客户端部分的表单。</dd>
 <dt><a href="https://developer.mozilla.org/zh-CN/docs/Learn/HTML/Howto">用HTML解决常见问题</a></dt>
 <dd>该部分提供了一些链接，这些链接指向那些在你构建Web页面的过程中最常遇到的问题的解决方法：如何处理网页标题、添加图片和视频、强调某些内容、建立基本的表单等。</dd>
</dl>

<h2 id="高级主题">高级主题</h2>

<dl>
 <dt class="landingPageList"><a href="/zh-CN/docs/Web/HTML/CORS_enabled_image">CORS 处理跨域图片</a></dt>
 <dd class="landingPageList"><code><a href="/zh-CN/docs/Web/HTML/Element/img#attr-crossorigin">crossorigin</a></code>属性在与一个得到恰当配置的<a class="glossaryLink" href="/zh-CN/docs/Glossary/CORS">CORS</a>头部相搭配时，可以使在{{HTMLElement("img")}}元素中定义并需要加载或者在{{HTMLElement("canvas")}}中所需使用的，来自外部来源的图片资源得到妥善的处理，使这些资源像是从本地源所加载一样。</dd>
 <dt class="landingPageList"><a href="/zh-CN/docs/Web/HTML/CORS_settings_attributes">CORS设置属性</a></dt>
 <dd class="landingPageList">一些HTML元素提供了对<a href="/zh-CN/docs/HTTP/Access_control_CORS">CORS</a>的支持，比如{{HTMLElement("img")}}或{{HTMLElement("video")}}，它们提供了<code>crossorigin</code>元素属性／attribute （<code>crossOrigin</code>对象属性／property），该属性使你能够对元素跨域获取资源的行为进行配置。</dd>
 <dt class="landingPageList"><a href="/zh-CN/docs/Web/HTML/Focus_management_in_HTML">HTML中的焦点管理</a></dt>
 <dd class="landingPageList">DOM元素的<code><a href="/zh-CN/docs/Web/API/Document/activeElement">activeElement</a></code>属性以及<code><a href="/zh-CN/docs/Web/API/Document/hasFocus">hasFocus()</a></code>方法可以帮助你跟踪并控制用户在网页中与各种元素的交互行为。</dd>
 <dt class="landingPageList"><a href="/zh-CN/docs/Web/HTML/Using_the_application_cache">使用应用缓存</a></dt>
 <dd class="landingPageList">应用程序缓存使得以网页为基础的程序可以离线运行。你可以使用<strong>Application Cache</strong>（<em>AppCache</em>）接口指定相应的资源令浏览器进行缓存，以使得用户可以离线使用该程序。缓存后的应用程序将能够被正确的加载并运行，即使用户在离线的状态下点击了刷新按钮也是如此。</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/zh-CN/docs/Web/HTML/Preloading_content">使用rel="preload"预加载页面内容</a></dt>
 <dd class="landingPageList">{{htmlelement("link")}}元素的{{htmlattrxref("rel", "link")}}的属性值<code>preload</code>，允许你在页面的{{htmlelement("head")}}部分进行一个资源预加载的声明。通过指定那些在页面加载后即刻需要的资源，将使得页面在生命周期的早期阶段对这些资源进行提前的预加载，甚至早于浏览器的主渲染机制介入之前。从而保证了这些资源的尽早可用并尽可能的减少对于页面初次渲染所造成的阻塞。这篇文章提供了关于<code>preload</code>作用机制的基本指导。</dd>
</dl>
</div>

<div class="section">
<h2 class="Documentation" id="Documentation" name="Documentation">参考</h2>

<dl>
 <dt class="landingPageList"><a href="/zh-CN/docs/Web/HTML/Reference">HTML参考</a></dt>
 <dd class="landingPageList">HTML由<strong>元素</strong>组成，每个元素都可以被多个<strong>属性</strong>修饰。HTML文档通过<a href="https://developer.mozilla.org/zh-CN/docs/Web/HTML/Link_types">链接</a>相互连接。</dd>
 <dt class="landingPageList"><a href="/zh-CN/docs/Web/HTML/Element">HTML元素参考</a></dt>
 <dd class="landingPageList">浏览一个完整的<a class="glossaryLink" href="/zh-CN/docs/Glossary/HTML">HTML</a><a class="glossaryLink" href="/zh-CN/docs/Glossary/Element">元素</a>列表。</dd>
 <dt class="landingPageList"><a href="/zh-CN/docs/Web/HTML/Attributes">HTML属性参考</a></dt>
 <dd class="landingPageList">HTML元素都含有<strong>元素属性</strong>。这些额外的属性值可以通过多种途径对元素进行配置或调整其行为。</dd>
 <dt class="landingPageList"><a href="/zh-CN/docs/Web/HTML/Global_attributes">全局属性</a></dt>
 <dd class="landingPageList">全局属性可以在所有<a href="/zh-CN/docs/Web/HTML/Element">HTML元素</a>上进行设置。<em>即使那些没有在相关标准中出现的元素也一样</em>。这就意味着那些非标准的元素也同样会实现这些属性，即使这些元素使得文档并不符合HTML5标准。</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Inline_elements">內联元素</a>和<a href="/zh-CN/docs/Web/HTML/Block-level_elements">块级元素</a></dt>
 <dd class="landingPageList">HTML元素通常是"內联"或"块级"元素。一个內联元素仅会占用由定义它的标签所包裹起来的空间。而一个块级元素将会占用其父元素（容器）的全部空间，也就是创建一个“块”</dd>
 <dt class="landingPageList"><a href="/zh-CN/docs/Web/HTML/Link_types">链接类型</a></dt>
 <dd class="landingPageList">在HTML中，各种各样的链接类型被用来确立和定义两个文档之间的关系。不同类型的链接（Link）会通过包括<a href="/zh-CN/docs/Web/HTML/Element/a"><code>&lt;a&gt;</code></a>，<a href="/zh-CN/docs/Web/HTML/Element/area"><code>&lt;area&gt;</code></a>，and <a href="/zh-CN/docs/Web/HTML/Element/link"><code>&lt;link&gt;</code></a>等元素进行设置。</dd>
 <dt class="landingPageList"><a href="/zh-CN/docs/Web/HTML/Supported_media_formats">HTML的audio与video元素所支持的媒体格式</a></dt>
 <dd class="landingPageList"><a href="/zh-CN/docs/Web/HTML/Element/audio"><code>&lt;audio&gt;</code></a>和<a href="/zh-CN/docs/Web/HTML/Element/video"><code>&lt;video&gt;</code></a>元素允许你播放视频和音频媒体文件。这些元素提供了一个浏览器原生的对与Adobe Flash 和其他外挂组件的替代品。</dd>
 <dt class="landingPageList"><a href="/zh-CN/docs/Web/HTML/Kinds_of_HTML_content">其他HTML内容</a>（高级）</dt>
 <dd class="landingPageList">HTML包含了大量的不同类型的内容，每种内容在特定的情景上下文中有效，而在其他上下文中无效。类似地，每种内容也包含了一组关于其他类型内容的配置，包括哪些内容类型和元素可以或不可以被包含包含并使用。这里提供了一个关于这些分类的说明。</dd>
</dl>

<h2 class="landingPageList" id="相关主题">相关主题</h2>

<dl>
 <dt><a href="/zh-CN/docs/Web/HTML/Applying_color">使用CSS为HTML元素添颜色</a></dt>
 <dd>如果需要使用CSS为HTML内容增加颜色，这篇文章涵盖了绝大多数的途径和方式，并列举了哪部分HTML文档内容可以进行上色以及这一操作将会涉及到哪些CSS属性。同时包含了一些示例以及到一些配色建构工具的链接，以及一些其他内容</dd>
</dl>
</div>
</div>
<span class="alllinks"><a href="/zh-CN/docs/tag/HTML">查看所有...</a></span>

<p>{{CommunityBox("Web layout", "dev-tech-layout", "mozilla.dev.tech.layout", "", "Stack Overflow|http://stackoverflow.com/questions/tagged/html|HTML topics|Visit Stack Overflow, a collaboratively built and maintained Q&amp;A site. See if you can find an answer; if not, you can ask your question there.")}}</p>
</section>

<p>&nbsp;</p>

