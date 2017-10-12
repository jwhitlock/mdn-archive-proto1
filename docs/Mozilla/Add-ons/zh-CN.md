---
version: prototype1
revision_id: 1318070
locale: zh-CN
slug: Mozilla/Add-ons
tags: "扩展" "附加组件" "Add-ons" "Mozilla" "Extension"
title: 附加组件
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<p>附加组件允许开发者们去扩展和修改 Firefox 的功能。开发者们能使用标准的 Web 技术「JavaScript，HTML 以及 CSS」再加上一些专用的 JavaScript APIs 来开发附加组件。除此之外，附加组件还能：</p>

<ul>
 <li>改变指定网站的外观或者内容</li>
 <li>修改 Firefox 的用户界面</li>
 <li>给 Firefox 加上新功能</li>
</ul>

<p>有几种附件组件类型，但最常见类型是扩展。</p>

<h2 id="开发扩展">开发扩展</h2>

<p>在过去，有几种工具集用于开发 Firefox 扩展，但是到 2017 年 11 月底，扩展必须使用 <a href="https://developer.mozilla.org/zh-CN/Add-ons/WebExtensions">WebExtensions APIs</a> 构建。其余工具集「包括 overlay add-ons、bootstrapped add-ons 和 Add-on SDK」将会同时被废弃。</p>

<p>如果你在编写一个新的扩展，请使用 <a href="https://developer.mozilla.org/zh-CN/Add-ons/WebExtensions">WebExtensions APIs</a>。</p>

<p>使用 Firefox WebExtensions APIs 编写的扩展设计为跨浏览器兼容。在大多数情况下它也能在 Chrome，Edge 和 Opera 中运行，几乎没有任何变化。它们也完全兼容多进程 Firefox。</p>

<p><a href="https://developer.mozilla.org/zh-CN/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">查看目前在火狐和其他浏览器中支持的 APIs</a>. 我们将继续设计并改进新的 API 以满足开发人员的需求。</p>

<p>绝大多数的 WebExtensions APIs 对于 Firefox Android 版也是可用的。</p>

<h3 id="迁移现有扩展">迁移现有扩展</h3>

<p>如果你正在维护一个旧式扩展，比如 XUL overlay、bootstrapped，或者基于 Add-on SDK 的扩展，我们建议你使用 WebExtension APIs 移植它。这里有一些&nbsp;<a href="https://developer.mozilla.org/zh-CN/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on"> MDN 中的移植教程</a>。</p>

<p style="position: relative; max-width: 400px; margin-bottom: 70px;">我们在 wiki 页面收集了一些<a href="https://wiki.mozilla.org/Add-ons/developer/communication">教程</a>来支持开发者们过渡。在开始之前，请使用兼容性<a href="https://compatibility-lookup.services.mozilla.com/">检测工具</a>来查看你的附加组件是否受影响。</p>

<h2 id="发布附加组件">发布附加组件</h2>

<p><a href="https://addons.mozilla.org">Addons.mozilla.org</a>，俗称 「AMO」，是 Mozilla 官方的官方站点, 方便开发者发布扩展组件和用户查找。通过上传附加组件到&nbsp; AMO， 你可以加入我们的用户和开发者社区，为你的附加组件找到订阅者。</p>

<p>你不需要在 AMO 上发布你的附加组件，但你的附加组件必须要经过 Mozilla 签名，否则用户不能安装它。</p>

<p>为你发布的附加组件添加概述，请查看<a href="https://developer.mozilla.org/zh-CN/Add-ons/Distribution">签名和部署你的附加组件</a>。</p>

<h2 id="其他类型的附加组件">其他类型的附加组件</h2>

<p>通常，当人们谈起附加组件时是指扩展工具，但是这里也有一些其他类型的附加组件允许用户定制 Firefox.&nbsp; 这些附加组件包括：</p>

<ul>
 <li><a href="https://developer.mozilla.org/Add-ons/Themes/Background">轻量主题</a> 是一种简单的方式来提供有限的 Firefox 定制；</li>
 <li><a href="https://developer.mozilla.org/zh-CN/Add-ons/Firefox_for_Android">移动附加组件</a> 是给 Firefox 的 Android 版使用的。注意，虽然如此，我们仍打算弃用这些 API 依赖的一些技术。在将来，Firefox 的 Android 版将会在一定程度上完全支持 WebExtension APIs；</li>
 <li><a href="https://developer.mozilla.org/zh-CN/docs/Creating_OpenSearch_plugins_for_Firefox">搜索引擎插件</a> 可以添加新的搜索引擎到浏览器的搜索栏；</li>
 <li><a href="https://developer.mozilla.org/zh-CN/docs/Mozilla/Creating_a_spell_check_dictionary_add-on">用户字典</a> 是可以进行各种语言的拼写检查的插件；</li>
 <li><a href="https://support.mozilla.org/kb/use-firefox-interface-other-languages-language-pack">语言包</a> 让你有更多可用的语言用于Firefox的界面。</li>
</ul>

<h2 id="联系我们">联系我们</h2>

<p>你可以从以下链接获得帮助，时刻关注关于附加组件的最新消息，并且给予我们反馈。</p>

<h3 id="附加组件论坛">附加组件论坛</h3>

<p>到 <a href="https://discourse.mozilla-community.org/c/add-ons">附加组件交流论坛</a> 讨论附加组件的任何方面并获得帮助。</p>

<h3 id="邮件列表">邮件列表</h3>

<p>通过 <strong>dev-addons</strong> 列表来讨论附加组件生态系统的发展，包括 WebExtensions 系统和 AMO。</p>

<ul>
 <li><a href="https://mail.mozilla.org/listinfo/dev-addons">dev-addons list info</a></li>
 <li><a href="https://mail.mozilla.org/pipermail/dev-addons/">dev-addons archives</a></li>
</ul>

<h3 id="IRC">IRC</h3>

<p>如果你更喜欢使用 IRC，你可以在以下 channel 和其他人交流：</p>

<ul>
 <li><a href="irc://irc.mozilla.org/addons">#addons</a> (附加组件生态系统的讨论)</li>
 <li><a href="irc://irc.mozilla.org/extdev">#extdev</a> (附加组件的发展战略的讨论)</li>
 <li><a href="irc://irc.mozilla.org/webextensions">#webextensions</a> (对WebExtensions具体的讨论)</li>
</ul>

