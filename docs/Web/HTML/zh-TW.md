---
version: prototype1
revision_id: 1272649
locale: zh-TW
slug: Web/HTML
tags: "HTML" "HTML元素" "多媒體" "影像" "音樂"
title: HTML
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>{{HTMLSidebar()}}</p>

<p><span class="seoSummary">HTML 意指「超文字標記語言」（HyperText Markup Language），是打造網頁的基石，用來撰寫與視覺化地呈現網頁。它定義了網頁的內容，但不定義網頁的功能。</span></p>

<p>HTML 新增了「標記」（markup）到標準英文文件中。「超文字」是指從原網頁到另一網頁的連結，而這項技術造就了今日的全球資訊網。藉由撰寫與上載網頁到網際網路中，一旦您的網站上線，您就變成全球資訊網的積極參與者。HTML 不僅支援顯示影像，也支援其他媒體。借助於&nbsp;HTML，每一個人都能創建靜態以及動態網站。HTML 是一種描述網路文件的結構和語意內容的語言。網頁內容被加上的 HTML 元素標記，包括&nbsp;{{HTMLElement("head")}}、{{HTMLElement("title")}}、{{HTMLElement("body")}}、{{HTMLElement("article")}}、{{HTMLElement("section")}}、{{HTMLElement("p")}}、{{HTMLElement("div")}}、{{HTMLElement("span")}}、{{HTMLElement("img")}}、{{HTMLElement("picture")}} 等等。這些元素構成了網站的基石。</p>

<p><span class="seoSummary">以下這些文章為網路開發提供了參考資料。</span></p>

<section class="cleared" id="sect1">
<ul class="card-grid">
 <li><span>HTML 參考資料</span>

  <p>在我們的 <a href="/en-US/docs/Web/HTML/Reference">extensive reference</a>&nbsp;中，您將會找到構成 HTML 的每個元素和屬性的細節。</p>
 </li>
 <li><span>HTML 指南</span>
  <p>關於如何使用 HTML 以及 HTML 指導與完整例子，請參考我們的 <a href="/en-US/docs/Web/Guide/HTML">HTML developer guide</a>。</p>
 </li>
 <li><span>HTML 介紹</span>
  <p>如果您是網站開發的新手，請先閱讀我們的 <a href="https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Introduction">introduction</a>，以知道 HTML 是什麼並且如何使用。</p>
 </li>
</ul>

<div class="row topicpage-table">
<div class="section">
<h2 class="Documentation" id="Documentation" name="Documentation">參考資料</h2>

<dl>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/zh-TW/docs/Web/HTML/Block-level_elements">區塊層級元素(Block-Level Elements)</a></dt>
 <dd class="landingPageList">HTML (Hypertext Markup Language) 元素通常分為「區塊層級」（block-level）元素或是<a href="https://developer.mozilla.org/zh-TW/docs/HTML/Inline_elements">「行內」（inline）元素</a>。一個區塊層級的元素會佔據它的父級元素（container）的所有空間。因而創造了「區塊」（block）。這篇文章將會解釋這是什麼意思。</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/CORS_enabled_image">跨來源資源共享圖片(CORS enabled image)</a></dt>
 <dd class="landingPageList">HTML5 規格為圖片導入了<code><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img#attr-crossorigin">跨來源（crossorigin</a>）</code>的屬性，它搭配合適的 CORS 標頭（<a class="glossaryLink" href="https://developer.mozilla.org/en-US/docs/Glossary/CORS" title="CORS: It is insecure to allow a webpage to request any resources from any other domains without limitation. CORS (Cross-Origin Resource Sharing) is a system that determines whether to block or fulfill these requests.">CORS</a> header），允許從外站載入由 <code><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img" title="The HTML Image Element (&lt;img&gt;) represents an image of the document.">&lt;img&gt;</a></code> 元素所定義的圖片被用在畫布（canvas）上，看起來就像從本站載入。</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/CORS_settings_attributes">跨來源資源共享設定屬性(CORS settings attributes)</a></dt>
 <dd class="landingPageList">在HTML5中，有些HTML元素是支援 <a href="https://developer.mozilla.org/en-US/docs/HTTP/Access_control_CORS">CORS </a>的，如 <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img" title="The HTML Image Element (&lt;img&gt;) represents an image of the document."><code>&lt;img&gt;</code></a> 或 <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/video" title="The HTML &lt;video&gt; element is used to embed video content. It may contain several video sources, represented using the src attribute or the &lt;source&gt; element; the browser will choose the most suitable one."><code>&lt;video&gt;</code></a>，它們具有 <code>crossorigin</code> 的屬性(attribute)，可以讓你幫元素的接收資訊設定CORS的要求。</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Controlling_spell_checking_in_HTML_formsControlling_spell_checking_in_HTML_forms">在HTML表單中控制拼字檢查</a></dt>
 <dd class="landingPageList">Firefox 2 在表單中為 text areas 和 text fields 提供了拼字檢查的支援。使用者可以利用分頁 about:config 的介面設定是否要開啟拼字檢查，以及個別設定 text areas 與 text fields 是否要開啟。</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/DASH_Adaptive_Streaming_for_HTML_5_Video">DASH - 為HTML 5 Video 而生的自適性串流</a></dt>
 <dd class="landingPageList">Dynamic Adaptive Streaming over HTTP (DASH) 是一個自適性串流協定。這意味著它允許影音串流基於當下網路情況調整自己的位元速率，以讓影片持續播放。</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Focus_management_in_HTML">HTML中的 焦點(Focus) 管理</a></dt>
 <dd class="landingPageList">在HTML5的草案中，<code><a href="https://developer.mozilla.org/en/DOM/document.activeElement" title="en/DOM/document.activeElement">activeElement</a></code> DOM 屬性與 <code><a href="https://developer.mozilla.org/en/DOM/document.hasFocus" title="en/DOM/document.hasFocus">hasFocus()</a></code> DOM 方法給予開發者有能力去掌握網頁與使用者的互動。舉例來說，這兩者都可以拿來做統計的目的，追蹤網頁中特定連結的點擊次數，評估某個元素被使用者聚焦的時間......等。甚至如果與AJAX結合，它們可以幫助最小化向伺服器發出請求的次數(因使用者動作與網頁設計而定)。</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes">全域屬性</a></dt>
 <dd class="landingPageList">全域屬性是可以被應用在所有的 <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element">HTML elements&nbsp;</a>上的，即使它們可能沒有被列為標準。這意味著那些非標準的元素依然會具有這些屬性，即使這代表使用了它們就不再是HTML5相容的。舉例來說，HTML5相容的瀏覽器會隱藏類似 <code>...</code> 的內容，即使這並不是一個合法的HTML元素。</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes">HTML 屬性參考</a></dt>
 <dd class="landingPageList">HTML的元素都具有屬性(attribute)，可以用來給予額外的值以調整元素或是行為來符合使用者的需求。</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element">HTML 元素參考</a></dt>
 <dd class="landingPageList">本頁列出所有的&nbsp;<a class="glossaryLink" href="https://developer.mozilla.org/en-US/docs/Glossary/HTML" title="HTML: HTML (HyperText Markup Language) is a descriptive language that specifies webpage structure.">HTML</a> <a class="glossaryLink" href="https://developer.mozilla.org/en-US/docs/Glossary/Element" title="elements: An element is a part of a webpage. In XML and HTML, an element may contain a data item or a chunk of text or an image, or perhaps nothing. A typical element includes an opening tag, attributes, content, and a closing tag:">元素</a>。</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Reference">HTML reference</a></dt>
 <dd class="landingPageList">HTML is the language that describes the structure and the semantic content of a Web document; it consists of <strong>elements</strong>, each of which may be modified by some number of <strong>attributes</strong>.</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Inline_elemente">行內元素</a></dt>
 <dd class="landingPageList">HTML (Hypertext Markup Language) elements are usually "inline" elements or <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Block-level_elements">"block-level" elements</a>. An inline element occupies only the space bounded by the tags that define the inline element. The following example demonstrates the inline element's influence:</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Link_types">鏈結類型</a></dt>
 <dd class="landingPageList">In HTML, the following link types indicate the relationship between two documents, in which one links to the other using an , , or element.</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Supported_media_formats">HTML audio及video元素支援多媒體格式</a></dt>
 <dd class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/audio" title="The HTML &lt;audio&gt; element is used to embed sound content in documents. It may contain several audio sources, represented using the src attribute or the &lt;source&gt; element; the browser will choose the most suitable one."><code>&lt;audio&gt;</code></a>&nbsp;及&nbsp;<a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/video" title="The HTML &lt;video&gt; element is used to embed video content. It may contain several video sources, represented using the src attribute or the &lt;source&gt; element; the browser will choose the most suitable one."><code>&lt;video&gt;</code></a>&nbsp;元素針對播放音樂及影像等多媒體檔案提供支援，且不需要任何附加元件</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/microformats">Microformats</a></dt>
 <dd class="landingPageList"><span class="p-summary"><a class="external external-icon" href="http://microformats.org"><dfn>Microformats</dfn></a> (sometimes abbreviated <strong>μF</strong>) are small patterns of HTML for marking up entities like people, organizations, events, locations, blog posts, products, reviews, resumes, recipes, etc.</span><br />
 They are simple conventions to embed semantics in HTML and quickly provide an API to be used by search engines, aggregators, and other tools.</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Optimizing_your_pages_for_speculative_parsing">Optimizing your pages for speculative parsing</a></dt>
 <dd class="landingPageList">Traditionally in browsers the HTML parser has run on the main thread and has blocked after a tag until the script has been retrieved from the network and executed. The HTML parser in Firefox 4 and later supports speculative parsing off the main thread. It parses ahead while scripts are being downloaded and executed. As in Firefox 3.5 and 3.6, the HTML parser starts speculative loads for scripts, style sheets and images it finds ahead in the stream. However, in Firefox 4 and later the HTML parser also runs the HTML tree construction algorithm speculatively. The upside is that when a speculation succeeds, there's no need to reparse the part of the incoming file that was already scanned for scripts, style sheets and images. The downside is that there's more work lost when the speculation fails.</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Using_the_application_cache">Using the application cache</a></dt>
 <dd class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/HTML/HTML5" title="HTML/HTML5">HTML5</a> provides an <em>application caching</em> mechanism that lets web-based applications run offline. Developers can use the <strong>Application Cache</strong> (<em>AppCache</em>) interface to specify resources that the browser should cache and make available to offline users. Applications that are cached load and work correctly even if users click the refresh button when they are offline.</dd>
</dl>

<p><span class="alllinks"><a href="/en-US/docs/tag/HTML" title="Article tagged: HTML">View All...</a></span></p>
</div>

<p>&nbsp;</p>

<div class="section">
<h2 class="Tools" id="Tools" name="Tools">Guides and tutorials</h2>

<dl>
 <dt><a href="/en-US/docs/Web/Guide/HTML">HTML 開發者指南</a></dt>
 <dd>在 MDN 的文章中，不僅教導了用 HTML 撰寫網站的明確技術，也展示了其他您可能會覺得易於使用的文章與指導。 這個指南可以提供 HTML 開發上的編輯課程、技巧與資訊。</dd>
</dl>
</div>
</div>

<p>{{CommunityBox("Web layout", "dev-tech-layout", "mozilla.dev.tech.layout", "", "Stack Overflow|http://stackoverflow.com/questions/tagged/html|HTML topics|Visit Stack Overflow, a collaboratively built and maintained Q&amp;A site. See if you can find an answer; if not, you can ask your question there.")}}</p>
</section>

