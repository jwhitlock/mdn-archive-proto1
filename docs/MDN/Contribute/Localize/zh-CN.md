---
version: prototype1
revision_id: 1343399
locale: zh-CN
slug: MDN/Contribute/Localize
tags: "MDN" "I10n" "Landing" "Localization"
title: MDN 本地化
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{IncludeSubnav("/zh-CN/docs/MDN")}}</div>

<p>MDN 被全世界的人们和 Firefox&nbsp;项目组内部用作 Web 技术的参考和指南。众多的本地化社区是 Mozilla 项目的一个关键部分，他们对文档的翻译和本地化工作可以帮助世界各地的人们开发开放 Web。如果你想更多地了解本地化相关的内容，或者准备开始一个新的本地化工作，你可以从这里开始。</p>

<h2 id="MDN_上的本地化类型">MDN 上的本地化类型</h2>

<p>MDN 上的本地化包含三个方面，它们位于不同的系统并要求不同访问权限。</p>

<h4 id="MDN_站点UI">MDN 站点的用户界面</h4>

<p>指的是每个或大多数 MDN 页面中都有的框架、导航和用户控制组件等部分。这些地方使用&nbsp;Mozilla&nbsp;<a href="https://developer.mozilla.org/zh-CN/docs/Localizing_with_Pontoon">Pontoon</a>&nbsp;系统自动翻译，<a href="https://pontoon.mozilla.org/projects/mdn/">这里</a>是该项目的主页。如果你所在地区的语言没有包含在&nbsp;MDN 中，你可以联系 Pontoon 管理员来启用。见<a href="https://developer.mozilla.org/zh-CN/docs/MDN/Contribute/Localize/Starting_a_localization">创建新的&nbsp;MDN&nbsp;本地化</a>。</p>

<h4 id="MDN_上的内容">MDN&nbsp;上的内容</h4>

<p>指 MDN&nbsp;页面中的主体内容，包含参考、指南和教程等文章。可以使用&nbsp;<a href="https://developer.mozilla.org/zh-CN/docs/MDN/Contribute/Localize/Translating_pages">MDN 内建的翻译接口</a>来翻译这些文章。如果你所在地区的语言没有包含在该接口所支持的语言列表中，可参考<a href="https://developer.mozilla.org/zh-CN/docs/MDN/Contribute/Localize/Starting_a_localization">创建新的&nbsp;MDN&nbsp;本地化</a>来了解如何操作。</p>

<h4 id="宏字符串">宏字符串</h4>

<p>这些字符串由<a href="https://developer.mozilla.org/zh-CN/docs/MDN/Contribute/Structures/Macros">宏模板</a>产生，以创建导航、消息或某些预定义的结构。因为修改模板可能会对已经使用该模板的所有页面产生影响，所以每次修改模板都需要通过<a href="https://developer.mozilla.org/zh-CN/docs/MDN/Contribute/Tools/Template_editing">提交一个&nbsp;pull&nbsp;request&nbsp;并经过评审</a>。</p>

<p>以下页面提供了 MDN 上本地化的更多信息：</p>

<p>{{LandingPageListSubpages}}</p>

<h2 id="MDN_上的本地化社区">MDN 上的本地化社区</h2>

<p>MDN 上的本地化活动由两个主体共同完成：独立的个人和一起工作的本地化小组，后者可能是一个更大的 Mozilla 本地化社区的一部分。MDN 上的本地化项目则由本地化带头人所领导。</p>

<ul>
 <li><a href="https://developer.mozilla.org/zh-CN/docs/MDN/Community/Roles/Localization_projects">本地化项目</a></li>
 <li><a href="https://developer.mozilla.org/zh-CN/docs/MDN/Community/Roles/Localization_driver_role">本地化带头人</a></li>
</ul>

<h2 id="中文翻译术语表和翻译规范">中文翻译术语表和翻译规范</h2>

<p>这篇文章列出了翻译中会遇到的一些术语以及翻译时推荐遵守的规范，推荐阅读：</p>

<p><a href="https://developer.mozilla.org/zh-CN/docs/Glossary_of_translation">翻译术语表和翻译规范</a></p>

<h2 id="本地化工具">本地化相关的工具</h2>

<p>这里介绍几个对你的本地化工作非常有用的工具：</p>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Mozilla/Localization/Localizing_with_Pontoon" title="/en-US/docs/Mozilla/Localization/Localizing_with_Verbatim">Pontoon</a></dt>
 <dd>用于多个 Mozilla 项目中的字符串的翻译，包括 MDN 用户界面和&nbsp;Firefox 用户界面。</dd>
 <dt><a href="http://transvision.mozfr.org/" title="http://transvision.mozfr.org/">Transvision</a></dt>
 <dd>由 Mozilla&nbsp;法国社区提供的一个工具。它可以搜索某个英文在 Mozilla&nbsp;代码中所有出现的地方，并列出针对目标语言的所有翻译。当需要确定某个单词或短语如何翻译更好时很有用。</dd>
</dl>

<h2 id="参阅">参阅</h2>

<ul>
 <li><a href="https://developer.mozilla.org/zh-CN/docs/Mozilla/Localization">Mozilla&nbsp;中的本地化</a></li>
 <li><a href="https://developer.mozilla.org/zh-CN/docs/Glossary_of_translation">翻译术语表和翻译规范</a></li>
</ul>

