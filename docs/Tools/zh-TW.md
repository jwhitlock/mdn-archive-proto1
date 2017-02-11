---
version: prototype1
revision_id: 1186543
locale: zh-TW
slug: Tools
tags: "Tools" "TopicStub" "NeedsMarkupWork" "Web Development" "NeedsTranslation" "Developing Mozilla" "Web Development:Tools" "NeedsTechnicalReview"
title: Firefox 開發者工具
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>在桌機與手機上檢查、編輯、並處理 HTML、CSS 與 JavaScript 的錯誤。要取得最新的開發者工具，請下載 <a href="https://www.mozilla.org/zh-TW/firefox/developer/">Firefox Developer Edition</a>。</p>

<h2 id="核心工具">核心工具</h2>

<hr />
<div class="column-container">
<div class="column-half">
<h3 id="頁面檢測器">頁面檢測器</h3>

<p><a href="/zh-TW/docs/Tools/Page_Inspector"><img alt="" src="https://mdn.mozillademos.org/files/14532/inspector.png" style="display:block; height:257px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>檢視並編輯網頁的內容與版面。視覺化各種東西，包括盒子模型、動畫、格線版面。</p>
</div>

<div class="column-half">
<h3 id="網路主控台">網路主控台</h3>

<p><a href="/zh-TW/docs/Tools/Web_Console"><img alt="" src="https://mdn.mozillademos.org/files/14528/console.png" style="display:block; height:257px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>檢查網頁紀錄的訊息、並透過 JavaScript 與網頁互動。</p>
</div>
</div>

<hr />
<div class="column-container">
<div class="column-half">
<h3 id="JavaScript_除錯器">JavaScript 除錯器</h3>

<p><a href="/zh-TW/docs/Tools/Debugger"><img alt="" src="https://mdn.mozillademos.org/files/14542/debugger.png" style="display:block; height:1026px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>停步、逐步、試驗、修改網頁的 JavaScript。</p>
</div>

<div class="column-half">
<h3 id="網路監控">網路監控</h3>

<p><a href="/zh-TW/docs/Tools/Network_Monitor"><img alt="" src="https://mdn.mozillademos.org/files/14534/network-monitor.png" style="display:block; height:257px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>看看網頁載入時發了什麼請求。</p>
</div>
</div>

<hr />
<div class="column-container">
<div class="column-half">
<h3 id="效能工具">效能工具</h3>

<p><a href="/zh-TW/docs/Tools/Performance"><img alt="" src="https://mdn.mozillademos.org/files/14536/performance.png" style="display:block; height:1026px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>分析網站的通常反應、JavaScript、還有布局效能。</p>
</div>

<div class="column-half">
<h3 id="適應性設計模式">適應性設計模式</h3>

<p><a href="/zh-TW/docs/Tools/Responsive_Design_Mode"><img alt="" src="https://mdn.mozillademos.org/files/14538/rdm.png" style="display:block; height:1542px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>看看網站或 app 在不同的設備與網路狀況下表現如何。</p>
</div>
</div>

<hr />
<h2 id="更多工具">更多工具</h2>

<p>Firefox 也內建了這些開發者工具，但通常不會像「核心工具」那麼常用。</p>

<div class="twocolumns">
<dl>
 <dt><a href="/zh-TW/docs/Tools/Memory">記憶體</a></dt>
 <dd>找出哪個物件是用了記憶體哪個地方。</dd>
 <dt><a href="/zh-TW/docs/Tools/Storage_Inspector">儲存空間</a></dt>
 <dd>檢查頁面存了什麼 cookie、本機的東西、indexedDB、session。</dd>
 <dt><a href="/zh-TW/docs/Tools/DOM_Property_Viewer">DOM 屬性檢查器</a></dt>
 <dd>檢查頁面的 DOM 屬性、函式之類的。</dd>
 <dt><a href="/zh-TW/docs/Tools/GCLI">開發者工具列</a></dt>
 <dd>開發者工具的命令行介面。</dd>
 <dt><a href="/zh-TW/docs/Tools/Eyedropper">Eyedropper</a></dt>
 <dd>選取網頁的顏色。</dd>
 <dt><a href="/zh-TW/docs/Tools/Scratchpad">速記本</a></dt>
 <dd>Firefox 裡面文字編輯器，讓你能撰寫並執行 JavaScript。</dd>
 <dt><a href="/zh-TW/docs/Tools/Style_Editor">樣式編輯器</a></dt>
 <dd>針對目前的頁面觀察與編輯 CSS 樣式。</dd>
 <dt><a href="/zh-TW/docs/Tools/Shader_Editor">Shader Editor</a></dt>
 <dd>查看與編輯 <a href="/zh-TW/docs/Web/WebGL">WebGL</a> 使用的 vertex 與 fragment shader。</dd>
 <dt><a href="/zh-TW/docs/Tools/Web_Audio_Editor">Web Audio Editor</a></dt>
 <dd>檢查音頻的節點圖形，並修改其參數。</dd>
</dl>
</div>

<hr />
<h2 id="連接開發者工具">連接開發者工具</h2>

<p>如果你透過<a href="/zh-TW/docs/Tools/Keyboard_shortcuts#Opening_and_closing_tools">鍵盤快捷鍵</a>或等同的選單選項啟動了開發者工具，它的目標會針對目前頁籤的文件。不過，你也可以把工具連接到其他目標，不論是不是相同的瀏覽器、甚至是不是相同的設備。</p>

<div class="twocolumns">
<dl>
 <dt><a href="/zh-TW/docs/Tools/about:debugging">about:debugging</a></dt>
 <dd>針對附加元件、內容頁籤、還有瀏覽器運行的 worker。</dd>
 <dt><a href="/zh-TW/docs/Tools/Remote_Debugging/Debugging_Firefox_for_Android_over_Wifi">連接到 Firefox for Android</a></dt>
 <dd>連接開發者工具到在 Android 運行的 Firefox 實例。</dd>
 <dt><a href="/zh-TW/docs/Tools/Working_with_iframes">連接到 iframes</a></dt>
 <dd>把開發者工具連接到頁面內指定的 iframe。</dd>
 <dt><a href="/zh-TW/docs/Tools/Valence">連接到其他瀏覽器</a></dt>
 <dd>把開發者工具連接到 Android 的 Chrome 與 iOS 的 Safari。</dd>
</dl>
</div>

<hr />
<h2 id="給瀏覽器除錯">給瀏覽器除錯</h2>

<p>開發者工具預設上是附加在網頁或網路 app 的。不過，你可以把它與瀏覽器作為一個整體連結起來。這在瀏覽器與附加元件開發方面會很有用。</p>

<div class="twocolumns">
<dl>
 <dt><a href="/zh-TW/docs/Tools/Browser_Console">瀏覽器控制台</a></dt>
 <dd>看看瀏覽器附加元件紀錄的訊息，然後運行 JavaScript 程式碼。</dd>
 <dt><a href="/zh-TW/docs/Tools/Browser_Toolbox">瀏覽器工具箱</a></dt>
 <dd>將開發者工具附加到瀏覽器本身。</dd>
</dl>
</div>

<hr />
<h2 id="擴展開發者工具">擴展開發者工具</h2>

<p>開發者工具都設計為易於擴展的。Firefox 附加元件可以取用開發者工具與其元件，擴展現有工具或加入新工具。使用遠端除錯協定，可以建立自己的除錯用戶端與伺服器，讓你可以使用自己的工具為網站除錯，或針對不同的目標平台應用 Firefox 工具。</p>

<div class="twocolumns">
<dl>
 <dt><a href="/zh-TW/docs/Tools/Example_add-ons">開發用附加元件示例</a></dt>
 <dd>透過實例理解如何作出一個開發用的附加元件。</dd>
 <dt><a href="/zh-TW/docs/Tools/Adding_a_panel_to_the_toolbox">給開發者工具加一個面板</a></dt>
 <dd>給開發者工具寫一個添加新面板的附加元件。</dd>
 <dt><a href="https://wiki.mozilla.org/Remote_Debugging_Protocol">遠端除錯協定</a></dt>
 <dd>協定用於連接 Firefox 開發者工具到如 Firefox 或 Firefox OS 設備之類的除錯目標。</dd>
 <dt><a href="/zh-TW/docs/Tools/Editor">原始碼編輯器</a></dt>
 <dd>Firefox 內建，能嵌入到附加元件的原始碼編輯器。</dd>
 <dt><a href="/zh-TW/docs/Tools/Debugger-API"><code>Debugger</code> 介面</a></dt>
 <dd>可以讓 JavaScript 程式碼觀察其他 JavaScript 程式碼的 API。Firefox 開發者工具利用該 API 實做了 JavaScript 程式碼除錯器。</dd>
 <dt><a href="/zh-TW/docs/Tools/Web_Console/Custom_output">自訂網頁主控台輸出</a></dt>
 <dd>如何擴展與自訂 <a href="/zh-TW/docs/Tools/Web_Console">Web Console</a> 和 <a href="/zh-TW/docs/Tools/Browser_Console">Browser Console</a> 的輸出。</dd>
</dl>
</div>

<hr />
<h2 id="貢獻">貢獻</h2>

<p>如果你想幫忙改進開發者工具，這些資源能幫助你。</p>

<div class="twocolumns">
<dl>
 <dt><a href="https://wiki.mozilla.org/DevTools/GetInvolved">Get Involved</a></dt>
 <dd>告訴你如何參與其中的 Mozilla wiki 頁面。</dd>
 <dt><a href="http://firefox-dev.tools/">firefox-dev.tools</a></dt>
 <dd>能幫你找到目前在處理的錯誤。</dd>
</dl>
</div>

<hr />
<div>{{CommunityBox("Developer tools", "dev-developer-tools", "mozilla.dev.developer-tools", "devtools", "Team info|https://wiki.mozilla.org/DevTools|Dev tools wiki|Designs and plans for the dev tools||Blog|https://hacks.mozilla.org/|Hacks blog|Hacks blog", "FirefoxDevTools", "firefox-developer-tools")}}</div>

<h2 id="Subnav">Subnav</h2>

<ol>
 <li><a href="#">Core Tools</a>

  <ol>
   <li><a href="/zh-TW/docs/Tools/Page_Inspector">Page Inspector</a></li>
   <li><a href="/zh-TW/docs/Tools/Web_Console">Web Console</a></li>
   <li><a href="/zh-TW/docs/Tools/Debugger">JavaScript Debugger</a></li>
   <li><a href="/zh-TW/docs/Tools/Network_Monitor">Network Monitor</a></li>
   <li><a href="/zh-TW/docs/Tools/Performance">Performance</a></li>
   <li><a href="/zh-TW/docs/Tools/Responsive_Design_Mode">Responsive Design Mode</a></li>
   <li><a href="/zh-TW/docs/Tools/Tips">Tips</a></li>
  </ol>
 </li>
 <li><a href="#">More Tools</a>
  <ol>
   <li><a href="/zh-TW/docs/Tools/Memory">Memory</a></li>
   <li><a href="/zh-TW/docs/Tools/Storage_Inspector">Storage Inspector</a></li>
   <li><a href="/zh-TW/docs/Tools/DOM_Property_Viewer">DOM Property Viewer</a></li>
   <li><a href="/zh-TW/docs/Tools/GCLI">Developer Toolbar</a></li>
   <li><a href="/zh-TW/docs/Tools/Eyedropper">Eyedropper</a></li>
   <li><a href="/zh-TW/docs/Tools/Scratchpad">Scratchpad</a></li>
   <li><a href="/zh-TW/docs/Tools/Style_Editor">Style Editor</a></li>
   <li><a href="/zh-TW/docs/Tools/Shader_Editor">Shader Editor</a></li>
   <li><a href="/zh-TW/docs/Tools/Web_Audio_Editor">Web Audio Editor</a></li>
  </ol>
 </li>
 <li><a href="#">Connecting the devtools</a>
  <ol>
   <li><a href="/zh-TW/docs/Tools/about:debugging">about:debugging</a></li>
   <li><a href="https://developer.mozilla.org/zh-TW/docs/Tools/Remote_Debugging/Debugging_Firefox_for_Android_over_Wifi">Connecting to Firefox for Android</a></li>
   <li><a href="https://developer.mozilla.org/zh-TW/docs/Tools/Working_with_iframes">Connecting to iframes</a></li>
   <li><a href="https://developer.mozilla.org/zh-TW/docs/Tools/Valence">Connecting to other browsers</a></li>
  </ol>
 </li>
 <li><a href="#">Debugging the browser</a>
  <ol>
   <li><a href="/zh-TW/docs/Tools/Browser_Console">Browser Console</a></li>
   <li><a href="/zh-TW/docs/Tools/Browser_Toolbox">Browser Toolbox</a></li>
  </ol>
 </li>
 <li><a href="#">Extending the devtools</a>
  <ol>
   <li><a href="/zh-TW/docs/Tools/Adding_a_panel_to_the_toolbox">Adding a panel to the toolbox</a></li>
   <li><a href="/zh-TW/docs/Tools/Example_add-ons">Example devtools add-ons</a></li>
   <li><a href="https://wiki.mozilla.org/Remote_Debugging_Protocol">Remote Debugging Protocol</a></li>
   <li><a href="https://wiki.mozilla.org/Remote_Debugging_Protocol_Stream_Transport">Stream Transport</a></li>
   <li><a href="/zh-TW/docs/Tools/Editor">Source Editor</a></li>
   <li><a href="/zh-TW/docs/Tools/Debugger-API">The <code>Debugger</code> Interface</a></li>
   <li><a href="/zh-TW/docs/Tools/Web_Console/Custom_output">Web Console custom output</a></li>
  </ol>
 </li>
 <li><a href="/zh-TW/docs/Tools/Settings">Settings</a></li>
 <li><a href="/zh-TW/docs/Tools/Release_notes">Release notes</a></li>
</ol>

