---
version: prototype1
revision_id: 1239863
locale: zh-TW
slug: Web/CSS
tags: 
title: CSS
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p><span class="seoSummary"><strong>層疊樣式表（Cascading Style Sheets, CSS）</strong>， 是用來描述 <a href="/zh-TW/docs/HTML" title="HyperText Markup Language">HTML</a> 或 <a href="/zh-TW/docs/XML" title="zh-TW/docs/XML">XML</a>（包含 <a href="/zh-TW/docs/SVG" title="zh-TW/docs/SVG">SVG</a> 或&nbsp;<a href="/zh-TW/docs/XHTML" title="zh-TW/docs/XHTML">XHTML</a> 等各種 XML 變形）文件外觀的<a href="/zh-TW/docs/DOM/stylesheet">樣式表</a>語言。</span>CSS 會描述文件裡的結構化元素，該如何呈現在螢幕、紙、語音報讀、或其他媒介上。</p>

<p><strong>CSS</strong> 是<em>開放網路</em>的核心語言之一，具有標準化的 <a class="external" href="http://w3.org/Style/CSS/#specs">W3C 規範</a>。歷經不同層級的開發，CSS1 目前已被棄用、CSS2.1 是建議規範，而 <a href="/zh-TW/docs/CSS/CSS3" title="CSS3">CSS3</a> 目前被分作數個較小的模組，持續在標準化的路上行進。</p>

<section id="sect1">
<ul class="card-grid">
 <li><span>CSS 參考</span>

  <p>這是給經驗豐富的網頁開發者的<a href="/zh-TW/docs/Web/CSS/Reference" title="zh-TW/docs/CSS/CSS_Reference">完整參考資訊</a>，說明 CSS 的每一個屬性與概念。</p>
 </li>
 <li><span>CSS 教學</span>
  <p>我們的 <a href="/zh-TW/docs/Learn/CSS">CSS 學習專區</a>包含所有必要的基礎資訊，能讓你從完全新手開始，帶向熟悉 CSS。</p>
 </li>
 <li><span>CSS 介紹</span>
  <p>若你剛接觸網路開發，請確定自己讀過我們的 <a href="/zh-TW/docs/Learn/Getting_started_with_the_web/CSS_basics">CSS 基礎</a> 以了解何謂 CSS 並知道要怎麼用。</p>
 </li>
</ul>

<div class="row topicpage-table">
<div class="section">
<h2 class="Documentation" id="教學">教學</h2>

<p>我們的 <a href="/zh-TW/docs/Learn/CSS">CSS 學習專區</a>有很多從頭教起的 CSS 模組。你不需要背景知識。</p>

<dl>
 <dt><a href="/zh-TW/docs/Learn/CSS/Introduction_to_CSS">CSS 介紹</a></dt>
 <dd>此模組讓你理解 CSS 工作原理，包含選擇器與屬性、撰寫 CSS 規則、在 HTML 套用 CSS、如何在 CSS 指定長度、色彩、還有其它單位、階層與繼承、box model 基礎、以及針對 CSS 除錯。</dd>
 <dt><a href="/zh-TW/docs/Learn/CSS/Styling_text">樣式化文字</a></dt>
 <dd>Here we look at text styling fundamentals, including setting font, boldness, and italics, line and letter spacing, and drop shadows and other text features. We round off the module by looking at applying custom fonts to your page, and styling lists and links.</dd>
 <dt><a href="/zh-TW/docs/Learn/CSS/Styling_boxes">Styling boxes</a></dt>
 <dd>Next up, we look at styling boxes, one of the fundamental steps towards laying out a web page. In this module we recap the box model then look at controlling box layouts by setting padding, borders and margins, setting custom background colors, images and other features, and fancy features such drop shadows and filters on boxes.</dd>
 <dt><a href="/zh-TW/docs/Learn/CSS/CSS_layout">CSS layout</a></dt>
 <dd>At this point we've already looked at CSS fundamentals, how to style text, and how to style and manipulate the boxes that your content sits inside. Now it's time to look at how to place your boxes in the right place in relation to the viewport, and one another. We have covered the necessary prerequisites so can now dive deep into CSS layout, looking at different display settings, traditional layout methods involving float and positioning, and new fangled layout tools like flexbox.</dd>
</dl>
</div>

<div class="section">
<h2 class="Tools" id="參考">參考</h2>

<ul>
 <li><a href="/zh-TW/docs/Web/CSS/Reference">CSS 參考</a>: An exhaustive reference for seasoned Web developers describing every property and concept of CSS.</li>
 <li>CSS key concepts:
  <ul>
   <li>The <a href="/zh-TW/docs/CSS/Syntax">syntax and forms of the language</a></li>
   <li><a href="/zh-TW/docs/CSS/Specificity">Specificity</a> and <a href="/zh-TW/docs/CSS/inheritance">inheritance</a></li>
   <li><a href="/zh-TW/docs/CSS/box_model">Box model</a> and <a href="/zh-TW/docs/CSS/margin_collapsing">margin collapse</a></li>
   <li><a href="/zh-TW/docs/CSS/Understanding_z-index/The_stacking_context" title="The stacking context">Stacking</a> and <a href="/zh-TW/docs/CSS/block_formatting_context" title="block formatting context">block-formatting</a> contexts</li>
   <li><a href="/zh-TW/docs/CSS/initial_value">Initial</a>, <a href="/zh-TW/docs/CSS/computed_value">computed</a>, <a href="/zh-TW/docs/CSS/used_value">used</a>, and <a href="/zh-TW/docs/CSS/actual_value">actual</a> values</li>
   <li><a href="/zh-TW/docs/CSS/Shorthand_properties">CSS shorthand properties</a></li>
   <li><a href="/zh-TW/docs/Web/CSS/CSS_Flexible_Box_Layout">CSS Flexible Box Layout</a></li>
   <li><a href="https://developer.mozilla.org/zh-TW/docs/Web/CSS/CSS_Grid_Layout">CSS 格線配置</a></li>
  </ul>
 </li>
</ul>

<h2 class="Tools" id="CSS_開發工具">CSS 開發工具</h2>

<ul>
 <li>The <a class="external" href="http://jigsaw.w3.org/css-validator/">W3C CSS 驗證服務</a> 能檢查 CSS 的有效性。<a href="http://www.onlinewebcheck.com/">OnlineWebCheck.com</a> 也在做相同的事情。它們都是很重要的除錯工具。</li>
 <li><a href="/zh-TW/docs/Tools">Firefox 開發者工具</a>能透過<a href="/zh-TW/docs/Tools/Page_Inspector">頁面檢測器</a>與<a href="/zh-TW/docs/Tools/Style_Editor">樣式編輯器</a>直接觀察、編輯網頁的 CSS。</li>
 <li>Firefox 的<a class="link-https" href="https://addons.mozilla.org/zh-TW/firefox/addon/1843">Firebug 套件</a>，navigator 裡面，能直接觀察、編輯網頁的 CSS 的人氣套件。要測試某些變化的時候會非常實用，而這套件還能做得更多。</li>
 <li>Firefox 的<a class="link-https" href="https://addons.mozilla.org/zh-TW/firefox/addon/60">Web Developer 套件</a> 也能能直接觀察、編輯網頁的 CSS。與 Firebug 相比更簡單、但相比下也沒那麼強大。</li>
 <li><a href="/zh-TW/docs/Web/CSS/Tools">其他 CSS 工具。</a></li>
</ul>

<h2 id="Meta_錯誤">Meta 錯誤</h2>

<ul>
 <li>Firefox: {{bug(1323667)}}</li>
</ul>
</div>
</div>
</section>

<h2 id="參見">參見</h2>

<ul>
 <li><a href="/zh-TW/docs/Web/Demos_of_open_web_technologies#CSS">CSS demos</a>最新的 CSS 技術動向：給予創意的一拔。</li>
 <li>常與 CSS 相關聯的語言：<a href="/zh-TW/docs/HTML">HTML</a>、<a href="/zh-TW/docs/SVG">SVG</a>、<a href="/zh-TW/docs/XHTML">XHTML</a>、<a href="/zh-TW/docs/XML">XML</a>。</li>
 <li>廣泛運用 CSS 的 Mozilla 科技：<a href="/zh-TW/docs/Mozilla/Tech/XUL">XUL</a>、<a href="/zh-TW/Firefox">Firefox</a>及<a href="/zh-TW/docs/Mozilla/Thunderbird">Thunderbird</a>的<a href="/zh-TW/docs/Extensions">套件</a>與<a href="/zh-TW/Add-ons/Themes">佈景</a></li>
</ul>

<p>{{CommunityBox("Web layout", "dev-tech-layout", "mozilla.dev.tech.layout", "", "Stack Overflow|http://stackoverflow.com/questions/tagged/css|CSS topics|Visit Stack Overflow, a collaboratively built and maintained Q&amp;A site. See if you can find an answer; if not, you can ask your question there.||CSS-Discuss|http://www.css-discuss.org/|CSS-Discuss mailing list|Join the css-discuss mailing list, which is dedicated to discussing practical, real-world use of CSS.")}}</p>

