---
version: prototype1
revision_id: 1335778
locale: ru
slug: Tools
tags: "Tools" "TopicStub" "l10n:priority" "инструменты" "Веб-разработка" "Developing Mozilla" "Разработка Mozilla" "веб-разработка:инструменты"
title: Инструменты разработчика Firefox
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: True
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<p>Исследуйте, редактируйте и отлаживайте HTML, CSS и JavaScript на компьютерах и мобильных устройствах. Для получения последних обновлений для инструментов разработки <a href="https://www.mozilla.org/ru/firefox/developer/">скачайте Firefox Developer Edition</a>.</p>

<p>{{ SauceLabsPromo("a") }}</p>

<h2 id="Основные_инструменты">Основные инструменты</h2>

<hr />
<div class="column-container">
<div class="column-half">
<h3 id="Инспектор_страницы">Инспектор страницы</h3>

<p><a href="/en-US/docs/Tools/Page_Inspector"><img alt="" src="https://mdn.mozillademos.org/files/14532/inspector.png" style="display:block; height:257px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>Инструмент для просмотра и редактирования содержимого и макета страницы. Позволяет рассмотреть страницу с разных точек зрения, включая блочную модель, анимацию и grid компоновку.</p>
</div>

<div class="column-half">
<h3 id="Web_консоль">Web консоль</h3>

<p><a href="/en-US/docs/Tools/Web_Console"><img alt="" src="https://mdn.mozillademos.org/files/14528/console.png" style="display:block; height:257px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>Позволяет просматривать отладочные сообщения страницы и взаимодействовать с ней посредством JavaScript.</p>
</div>
</div>

<hr />
<div class="column-container">
<div class="column-half">
<h3 id="Отладчик_JavaScript">Отладчик JavaScript</h3>

<p><a href="/en-US/docs/Tools/Debugger"><img alt="" src="https://mdn.mozillademos.org/files/14542/debugger.png" style="display:block; height:1026px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>Позволяет остановить, выполнять по шагам, исследовать и изменять JavaScript код выполняемый на странице.</p>
</div>

<div class="column-half">
<h3 id="Монитор_сетевой_активности">Монитор сетевой активности</h3>

<p><a href="/en-US/docs/Tools/Network_Monitor"><img alt="" src="https://mdn.mozillademos.org/files/14534/network-monitor.png" style="display:block; height:257px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>Показывает сетевые запросы возникающие в процессе загрузки страницы.</p>
</div>
</div>

<hr />
<div class="column-container">
<div class="column-half">
<h3 id="Performance_Tools">Performance Tools</h3>

<p><a href="/en-US/docs/Tools/Performance"><img alt="" src="https://mdn.mozillademos.org/files/14536/performance.png" style="display:block; height:1026px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>Позволяет провести общий анализ отзывчивости вашего сайта, а также производительности JavaScript кода и макета.</p>
</div>

<div class="column-half">
<h3 id="Режим_адаптивного_дизайна">Режим адаптивного дизайна</h3>

<p><a href="/en-US/docs/Tools/Responsive_Design_Mode"><img alt="" src="https://mdn.mozillademos.org/files/14538/rdm.png" style="display:block; height:1542px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>Позволяет увидеть, как будут выглядеть и работать ваши сайты или приложения на различных устройствах или типах сетей.</p>
</div>
</div>

<hr />
<h2 id="Больше_инструментов">Больше инструментов</h2>

<p>Эти инструменты разработчика также встроены в Firefox. В отличие от «Core Tools»&nbsp; описанных выше, могут не использоватся в повседневной работе.</p>

<div class="twocolumns">
<dl>
 <dt><a href="/en-US/docs/Tools/Memory">Memory</a></dt>
 <dd>Figure out which objects are keeping memory in use.</dd>
 <dt><a href="/en-US/docs/Tools/Storage_Inspector">Storage Inspector</a></dt>
 <dd>Inspect cookies, local storage, indexedDB, and session storage present in a page.</dd>
 <dt><a href="/en-US/docs/Tools/DOM_Property_Viewer">DOM Property Viewer</a></dt>
 <dd>Inspect the page's DOM properties, functions, etc.</dd>
 <dt><a href="/en-US/docs/Tools/GCLI">Developer Toolbar</a></dt>
 <dd>A command-line interface for the developer tools.</dd>
 <dt><a href="/en-US/docs/Tools/Eyedropper">Eyedropper</a></dt>
 <dd>Select a color from the page.</dd>
 <dt><a href="/en-US/docs/Tools/Scratchpad">Scratchpad</a></dt>
 <dd>A text editor built into Firefox that lets you write and execute JavaScript.</dd>
 <dt><a href="/en-US/docs/Tools/Style_Editor">Редактор стилей</a></dt>
 <dd>Просмотр и редактирование стилей CSS для текущей страницы.</dd>
 <dt><a href="/en-US/docs/Tools/Shader_Editor">Shader Editor</a></dt>
 <dd>View and edit the vertex and fragment shaders used by <a href="/en-US/docs/Web/WebGL">WebGL</a>.</dd>
 <dt><a href="/en-US/docs/Tools/Web_Audio_Editor">Web Audio Editor</a></dt>
 <dd>Examine the graph of audio nodes in an audio context, and modify their parameters.</dd>
 <dt><a href="/en-US/docs/Tools/Screenshot_tool">Taking screenshots</a></dt>
 <dd>Take a screenshot of the entire page or of a single element.</dd>
</dl>
</div>

<hr />
<h2 id="Connecting_the_Developer_Tools">Connecting the Developer Tools</h2>

<p>If you open the developer tools using <a href="/en-US/docs/Tools/Keyboard_shortcuts#Opening_and_closing_tools">keyboard shortcuts</a> or the equivalent menu items, they'll target the document hosted by the currently active tab. But you can attach the tools to a variety of other targets, too, both within the current browser and in different browsers or even different devices.</p>

<div class="twocolumns">
<dl>
 <dt><a href="/en-US/docs/Tools/about:debugging">about:debugging</a></dt>
 <dd>Debug add-ons, content tabs, and workers running in the browser.</dd>
 <dt><a href="/en-US/docs/Tools/Remote_Debugging/Debugging_Firefox_for_Android_over_Wifi">Connecting to Firefox for Android</a></dt>
 <dd>Connect the developer tools to an instance of Firefox running on an Android device.</dd>
 <dt><a href="/en-US/docs/Tools/Working_with_iframes">Connecting to iframes</a></dt>
 <dd>Connect the developer tools to a specific iframe in the current page.</dd>
 <dt><a href="/en-US/docs/Tools/Valence">Connecting to other browsers</a></dt>
 <dd>Connect the developer tools to Chrome on Android and Safari on iOS.</dd>
</dl>
</div>

<hr />
<h2 id="Debugging_the_browser">Debugging the browser</h2>

<p>By default, the developer tools are attached to a web page or web app. But you can also connect them to the browser as a whole. This is useful for browser and add-on development.</p>

<div class="twocolumns">
<dl>
 <dt><a href="/en-US/docs/Tools/Browser_Console">Browser Console</a></dt>
 <dd>See messages logged by the browser itself and by add-ons, and run JavaScript code in the browser's scope.</dd>
 <dt><a href="/en-US/docs/Tools/Browser_Toolbox">Browser Toolbox</a></dt>
 <dd>Attach the Developer Tools to the browser itself.</dd>
</dl>
</div>

<hr />
<h2 id="Extending_the_devtools">Extending the devtools</h2>

<p>The developer tools are designed to be extensible. Firefox add-ons can access the developer tools and the components they use to extend existing tools and add new tools. With the remote debugging protocol, you can implement your own debugging clients and servers, enabling you to debug websites using your own tools or to debug different targets using the Firefox tools.</p>

<div class="twocolumns">
<dl>
 <dt><a href="/en-US/docs/Tools/Example_add-ons">Example devtools add-ons</a></dt>
 <dd>Use these examples to understand how to implement a devtools add-on.</dd>
 <dt><a href="/en-US/docs/Tools/Adding_a_panel_to_the_toolbox">Add a new panel to the devtools</a></dt>
 <dd>Write an add-on that adds a new panel to the Toolbox.</dd>
 <dt><a href="https://wiki.mozilla.org/Remote_Debugging_Protocol">Remote Debugging Protocol</a></dt>
 <dd>The protocol used to connect the Firefox Developer Tools to a debugging target like an instance of Firefox or a Firefox OS device.</dd>
 <dt><a href="/en-US/docs/Tools/Editor">Source Editor</a></dt>
 <dd>A code editor built into Firefox that can be embedded in your add-on.</dd>
 <dt><a href="/en-US/docs/Tools/Debugger-API">The <code>Debugger</code> Interface</a></dt>
 <dd>An API that lets JavaScript code observe the execution of other JavaScript code. The Firefox Developer Tools use this API to implement the JavaScript debugger.</dd>
 <dt><a href="/en-US/docs/Tools/Web_Console/Custom_output">Web Console custom output</a></dt>
 <dd>How to extend and customize the output of the <a href="/en-US/docs/Tools/Web_Console">Web Console</a> and the <a href="/en-US/docs/Tools/Browser_Console">Browser Console</a>.</dd>
</dl>
</div>

<hr />
<h2 id="Contribute">Contribute</h2>

<p>If you want to help to improve the developer tools, these resources will get you started.</p>

<div class="twocolumns">
<dl>
 <dt><a href="https://devtools-html.github.io/#getting-in-touch">Get Involved</a></dt>
 <dd>Mozilla wiki page explaining how to get involved.</dd>
 <dt><a href="http://firefox-dev.tools/">firefox-dev.tools</a></dt>
 <dd>A tool helping to find bugs to work on.</dd>
</dl>
</div>

<hr />
<div>{{CommunityBox("Developer tools", "dev-developer-tools", "mozilla.dev.developer-tools", "devtools", "Team info|https://wiki.mozilla.org/DevTools|Dev tools wiki|Designs and plans for the dev tools||Blog|https://hacks.mozilla.org/|Hacks blog|Hacks blog", "FirefoxDevTools", "firefox-developer-tools")}}</div>

<h2 id="Subnav">Subnav</h2>

<ol>
 <li><a href="#">Основные иструменты</a>

  <ol>
   <li><a href="/en-US/docs/Tools/Page_Inspector">Инспектор страницы</a></li>
   <li><a href="/en-US/docs/Tools/Web_Console">Web консоль</a></li>
   <li><a href="/en-US/docs/Tools/Debugger">Отладчик JavaScript</a></li>
   <li><a href="/en-US/docs/Tools/Network_Monitor">Монитор сетевой активности</a></li>
   <li><a href="/en-US/docs/Tools/Performance">Performance</a></li>
   <li><a href="/en-US/docs/Tools/Responsive_Design_Mode">Режим адаптивного дизайна</a></li>
   <li><a href="/en-US/docs/Tools/Tips">Советы</a></li>
  </ol>
 </li>
 <li><a href="#">Больше инструментов</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Memory">Memory</a></li>
   <li><a href="/en-US/docs/Tools/Storage_Inspector">Storage Inspector</a></li>
   <li><a href="/en-US/docs/Tools/DOM_Property_Viewer">DOM Property Viewer</a></li>
   <li><a href="/en-US/docs/Tools/GCLI">Developer Toolbar</a></li>
   <li><a href="/en-US/docs/Tools/Eyedropper">Eyedropper</a></li>
   <li><a href="/en-US/docs/Tools/Taking_screenshots">Screenshot</a></li>
   <li><a href="/en-US/docs/Tools/Scratchpad">Scratchpad</a></li>
   <li><a href="/en-US/docs/Tools/Style_Editor">Редактор стилей</a></li>
   <li><a href="/en-US/docs/Tools/Shader_Editor">Shader Editor</a></li>
   <li><a href="/en-US/docs/Tools/Web_Audio_Editor">Web Audio Editor</a></li>
  </ol>
 </li>
 <li><a href="#">Connecting the devtools</a>
  <ol>
   <li><a href="/en-US/docs/Tools/about:debugging">about:debugging</a></li>
   <li><a href="https://developer.mozilla.org/en-US/docs/Tools/Remote_Debugging/Debugging_Firefox_for_Android_over_Wifi">Connecting to Firefox for Android</a></li>
   <li><a href="https://developer.mozilla.org/en-US/docs/Tools/Working_with_iframes">Connecting to iframes</a></li>
   <li><a href="https://developer.mozilla.org/en-US/docs/Tools/Valence">Connecting to other browsers</a></li>
  </ol>
 </li>
 <li><a href="#">Debugging the browser</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Browser_Console">Browser Console</a></li>
   <li><a href="/en-US/docs/Tools/Browser_Toolbox">Browser Toolbox</a></li>
  </ol>
 </li>
 <li><a href="#">Extending the devtools</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Adding_a_panel_to_the_toolbox">Adding a panel to the toolbox</a></li>
   <li><a href="/en-US/docs/Tools/Example_add-ons">Example devtools add-ons</a></li>
   <li><a href="https://wiki.mozilla.org/Remote_Debugging_Protocol">Remote Debugging Protocol</a></li>
   <li><a href="https://wiki.mozilla.org/Remote_Debugging_Protocol_Stream_Transport">Stream Transport</a></li>
   <li><a href="/en-US/docs/Tools/Editor">Source Editor</a></li>
   <li><a href="/en-US/docs/Tools/Debugger-API">The <code>Debugger</code> Interface</a></li>
   <li><a href="/en-US/docs/Tools/Web_Console/Custom_output">Web Console custom output</a></li>
  </ol>
 </li>
 <li><a href="/en-US/docs/Tools/Settings">Settings</a></li>
 <li><a href="/en-US/docs/Tools/Release_notes">Release notes</a></li>
</ol>

