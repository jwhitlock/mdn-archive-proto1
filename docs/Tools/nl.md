---
version: prototype1
revision_id: 941609
locale: nl
slug: Tools
tags: "Tools" "Handleiding" "Webontwikkeling" "Mozilla Ontwikkelaars" "Webontwikkeling hulpmiddelen"
title: Developer Tools
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div class="summary"><span class="seoSummary">Bekijk, bewerk, en debug HTML, CSS, en JavaScript via desktop en mobiel</span></div>

<div class="column-container zone-callout"><a href="https://www.mozilla.org/en-US/firefox/developer/" style="float: right; margin-bottom: 20px; padding: 10px; text-align: center; border-radius: 4px; display: inline-block; background-color: #81BC2E; white-space: nowrap; color: white; text-shadow: 0px 1px 0px rgba(0, 0, 0, 0.25); box-shadow: 0px 1px 0px 0px rgba(0, 0, 0, 0.2), 0px -1px 0px 0px rgba(0, 0, 0, 0.3) inset;">Installeer Firefox Developer Edition</a>

<h3 id="What's_new_in_Aurora.3F" name="What's_new_in_Aurora.3F">Wat is nieuw in Firefox Developer Edition?</h3>

<p><a href="/en-US/Firefox/Developer_Edition">Firefox Developer Edition</a> is een versie van Firefox speciaal voor ontwikkelaars, met de laatste Firefox functies en experimentele developer tools. De huidige Developer Edition heeft de volgende updates in de developer tools:</p>

<ul>
 <li><a href="/en-US/docs/Tools/Web_Console/Console_messages#Server">Server logging in the Web Console</a></li>
 <li><a href="/en-US/docs/Tools/Page_Inspector/How_to/Examine_and_edit_CSS#Overridden_declarations">Quickly find the rule that overrode a CSS declaration</a></li>
 <li><a href="/en-US/docs/Tools/Page_Inspector/How_to/Examine_and_edit_HTML#Element_popup_menu">"Use in Console" context menu item in Inspector</a></li>
 <li><a href="/en-US/docs/Tools/Page_Inspector/How_to/Examine_and_edit_CSS#Strict_search">"Strict" option for filtering in the Rules view</a></li>
 <li><a href="/en-US/docs/Tools/Web_Console/Console_messages#Network">Network entries in the Console now link to the Network Monitor</a></li>
 <li><span class="author-g-1scq3ywqbljc5puc">New sidebar UI for WebIDE</span></li>
</ul>
</div>

<div class="column-container zone-callout"><a href="http://mzl.la/devtools" style="float: right; margin-bottom: 20px; padding: 10px; text-align: center; border-radius: 4px; display: inline-block; background-color: #81BC2E; white-space: nowrap; color: white; text-shadow: 0px 1px 0px rgba(0, 0, 0, 0.25); box-shadow: 0px 1px 0px 0px rgba(0, 0, 0, 0.2), 0px -1px 0px 0px rgba(0, 0, 0, 0.3) inset;">Deel je ideeën</a>

<h3 id="Share_your_ideas" name="Share_your_ideas">Deel je ideeën</h3>

<p>Vraag voor nieuwe functies in de developer tools of stem op ideeën van andere ontwikkelaars.</p>
</div>

<p><img alt="" src="https://mdn.mozillademos.org/files/10529/inspector.png" style="display:block; height:467px; margin-left:auto; margin-right:auto; width:815px" /></p>

<div class="column-container">
<div class="column-half">
<h2 id="Creating" name="Creating">Creëren</h2>

<p>Authoring tools voor websites en web apps.</p>

<dl>
 <dt><a href="/en-US/docs/Tools/Scratchpad">Scratchpad</a></dt>
 <dd>Een text editor ingebouwd in Firefox die jou JavaScript code laat schrijven en executeren.</dd>
 <dt><a href="/en-US/docs/Tools/Style_Editor">Style Editor</a></dt>
 <dd>Bekijk en bewerk CSS styles voor de huidige pagina.</dd>
 <dt><a href="/en-US/docs/Tools/Shader_Editor">Shader Editor</a></dt>
 <dd>Bekijk en bewerk de vertex en fragment shaders gebruikt door <a href="/en-US/docs/Web/WebGL">WebGL</a>.</dd>
 <dt><a href="/en-US/docs/Tools/Web_Audio_Editor">Web Audio Editor</a></dt>
 <dd>Bekijk de grafiek van audio knooppunten in een audio context, en wijzig hun parameters.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Exploring" name="Exploring">Onderzoeken en debuggen</h2>

<p>Bekijk, onderzoek en debug websites en web apps.</p>

<dl>
 <dt><a href="/en-US/docs/Tools/Web_Console">Web Console</a></dt>
 <dd>Zie berichten logboek van een webpagina, en heb directeinteractie met de pagina via JavaScript.</dd>
 <dt><a href="/en-US/docs/Tools/Page_Inspector">Page Inspector</a></dt>
 <dd>Bekijk en wijzig de pagina in HTML and CSS.</dd>
 <dt><a href="/en-US/docs/Tools/Debugger">JavaScript Debugger</a></dt>
 <dd>Stop, stap-voor-stap, onderzoek en wijzig JavaScript code dat draait in een pagina.</dd>
 <dt><a href="/en-US/docs/Tools/Network_Monitor">Network Monitor</a></dt>
 <dd>Zie de netwerkaanvragen wanneer een pagina is geladen.</dd>
 <dt><a href="/en-US/docs/Tools/Storage_Inspector">Storage Inspector</a></dt>
 <dd>Inspecteer cookies, lokale opslag, indexedDB en sessie opslag aanwezig in een pagina.</dd>
 <dt><a href="/en-US/docs/Tools/GCLI">Developer Toolbar</a></dt>
 <dd>Een command-line interface voor de developer tools.</dd>
 <dt><a href="/en-US/docs/Tools/3D_View">3D View</a></dt>
 <dd>3D visualisatie van de pagina.</dd>
 <dt><a href="/en-US/docs/Tools/Eyedropper">Eyedropper</a></dt>
 <dd>Selecteer een kleur van de pagina.</dd>
 <dt><a href="/en-US/docs/Tools/Working_with_iframes">Working with iframes</a></dt>
 <dd><span class="short_text" id="result_box" lang="nl"><span class="hps">Hoe moet je een bepaalde</span> <span class="hps">iframe</span> aanpakken?</span></dd>
</dl>
</div>
</div>

<hr />
<div class="column-container">
<div class="column-half">
<h2 id="Mobile" name="Mobile">Mobiel</h2>

<p>Tools voor mobiele ontwikkelingen.</p>

<dl>
 <dt><a href="/en-US/Firefox_OS/Using_the_App_Manager">App Manager</a></dt>
 <dd>App Manager is vervangen door <a href="/en-US/docs/Tools/WebIDE">WebIDE</a>.</dd>
 <dt><a href="/en-US/docs/Tools/WebIDE">WebIDE</a></dt>
 <dd>De vervanger van App Manager, beschikbaar vanaf Firefox 33.</dd>
 <dt><a href="/en-US/docs/Tools/Firefox_OS_Simulator">Firefox OS Simulator</a></dt>
 <dd>Draai en debug uw Firefox OS app op de desktop zonder een fysiek Firefox OS apparaat.</dd>
 <dt><a href="/en-us/docs/Tools/Responsive_Design_View">Responsive Design View</a></dt>
 <dd>Bekijk hoe uw website of app eruit zal zien op verschillende schermgroottes zonder de grootte van het browservenster te wijzigen.</dd>
 <dt><a href="/en-US/docs/Tools/Remote_Debugging/Firefox_for_Android">Debugging on Firefox for Android</a></dt>
 <dd>Koppel de developer tools op Firefox voor Android.</dd>
 <dt><a href="/en-US/docs/Tools/Remote_Debugging/Debugging_Firefox_for_Android_with_WebIDE">Debugging Firefox for Android with WebIDE</a></dt>
 <dd>Voor Desktop Firefox 36+ / Android Firefox 35+ <span class="short_text" id="result_box" lang="nl"><span class="hps">er is</span> <span class="hps">een eenvoudiger</span> <span class="hps">proces</span><span>.</span></span></dd>
 <dt><a href="/en-US/docs/Tools/Valence">Valence</a></dt>
 <dd>Koppel de developer tools aan Chrome op Android en Safari op iOS</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Performance" name="Performance">Prestaties</h2>

<p>Diagnosticeer en repareer prestatieproblemen.</p>

<dl>
 <dt><a href="/en-US/docs/Tools/Performance">Performance tool</a></dt>
 <dd>Analiseer uw site's algemene <span class="short_text" id="result_box" lang="nl"><span class="hps">responsiviteit</span></span>, JavaScript en lay-out vertoning.</dd>
 <dt><a href="/en-US/docs/Tools/Performance/Frame_rate">Frame rate graph</a></dt>
 <dd>Zie de framesnelheid voor uw site.</dd>
 <dt><a href="/en-US/docs/Tools/Performance/Waterfall">Waterfall</a></dt>
 <dd>Ontdek hoe de browser reageert wanneer uw site draait.</dd>
 <dt><a href="/en-US/docs/Tools/Performance/Call_Tree">Call Tree</a></dt>
 <dd>Ontdek waar uw JavaScript code zijn tijd gebruikt.</dd>
</dl>

<dl>
 <dt><a href="/en-US/docs/Tools/Performance/Flame_Chart">Flame Chart</a></dt>
 <dd>See which functions are on the stack over the course of a performance profile.</dd>
 <dt><a href="/en-US/docs/Tools/Paint_Flashing_Tool">Paint Flashing Tool</a></dt>
 <dd>Highlights the parts of the page that are repainted in response to events.</dd>
 <dt><a href="/en-US/docs/Tools/Web_Console#Reflow_events">Reflow Event Logging</a></dt>
 <dd>See reflow events in the web console.</dd>
 <dt><a href="/en-US/docs/Tools/Network_Monitor#Performance_analysis">Network Performance</a></dt>
 <dd>See how long the parts of your site take to load.</dd>
</dl>
</div>
</div>

<hr />
<p>&nbsp;</p>

<p>&nbsp;</p>

<div class="column-container">
<div class="column-half">
<h2 id="Debugging_the_browser" name="Debugging_the_browser">Debugging the browser</h2>

<p>By default, the developer tools are attached to a web page or web app. But you can also connect them to the browser as a whole. This is useful for browser and add-on development.</p>

<dl>
 <dt><a href="/en-US/docs/Tools/Browser_Console">Browser Console</a></dt>
 <dd>See messages logged by the browser itself and add-ons, and run JavaScript code in the browser's scope.</dd>
 <dt><a href="/en-US/docs/Tools/Browser_Toolbox">Browser Toolbox</a></dt>
 <dd>Attach the Developer Tools to the browser itself.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Extending_the_devtools" name="Extending_the_devtools">Extending the devtools</h2>

<p>The developer tools are designed to be extensible. Firefox add-ons can access the developer tools and the components they use to extend existing tools and add new tools. With the remote debugging protocol you can implement your own debugging clients and servers, enabling you to debug websites using your own tools or to debug different targets using the Firefox tools.</p>

<dl>
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
 <dt><a href="/en-US/docs/Tools/Example_add-ons">Example devtools add-ons</a></dt>
 <dd>Use these examples to understand how to implement a devtools add-on.</dd>
</dl>
</div>
</div>

<hr />
<h2 id="More_resources" name="More_resources">More resources</h2>

<p>This section lists resources which are not currently maintained by Mozilla's developer tools team, but which are widely used by web developers. We've included a few Firefox add-ons in this list, but for the complete list see the <a href="https://addons.mozilla.org/en-US/firefox/extensions/web-development/">“Web Development” category on addons.mozilla.org</a>.</p>

<div class="column-container">
<div class="column-half">
<dl>
 <dt><a href="https://www.getfirebug.com/">Firebug</a></dt>
 <dd>A very popular and powerful web development tool, including a JavaScript debugger, HTML and CSS viewer and editor, and network monitor.</dd>
 <dt><a href="/en-US/docs/Tools/Add-ons/DOM_Inspector">DOM Inspector</a></dt>
 <dd>Inspect, browse, and edit the DOM of web pages or XUL windows.</dd>
 <dt><a href="https://addons.mozilla.org/en-US/firefox/addon/web-developer/">Web Developer</a></dt>
 <dd>Adds a menu and a toolbar to the browser with various web developer tools.</dd>
</dl>
</div>

<div class="column-half">
<dl>
 <dt><a href="https://webmaker.org/en-US/tools/">Webmaker Tools</a></dt>
 <dd>A set of tools developed by Mozilla, aimed at people getting started with Web development.</dd>
 <dt><a href="http://www.w3.org/Status.html">W3C Validators</a></dt>
 <dd>The W3C website hosts a number of tools to check the validity of your website, including its <a href="http://validator.w3.org/" title="http://validator.w3.org/">HTML</a> and <a href="http://jigsaw.w3.org/css-validator/" title="http://jigsaw.w3.org/css-validator/">CSS</a>.</dd>
 <dt><a href="http://www.jshint.com/">JSHint</a></dt>
 <dd>JavaScript code analysis tool.</dd>
</dl>
</div>
</div>

<hr />
<div>{{CommunityBox("Developer tools", "dev-developer-tools", "mozilla.dev.developer-tools", "devtools", "Team info|https://wiki.mozilla.org/DevTools|Dev tools wiki|Designs and plans for the dev tools||Blog|https://hacks.mozilla.org/|Hacks blog|Hacks blog", "FirefoxDevTools", "firefox-developer-tools")}}</div>

<h2 id="Subnav" name="Subnav">Subnav</h2>

<ol>
 <li><a href="#">Creating</a>

  <ol>
   <li><a href="/en-US/docs/Tools/Scratchpad">Scratchpad</a></li>
   <li><a href="/en-US/docs/Tools/Style_Editor">Style Editor</a></li>
   <li><a href="/en-US/docs/Tools/Shader_Editor">Shader Editor</a></li>
   <li><a href="/en-US/docs/Tools/Web_Audio_Editor">Web Audio Editor</a></li>
  </ol>
 </li>
 <li><a href="#">Debugging</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Page_Inspector">Page Inspector</a></li>
   <li><a href="/en-US/docs/Tools/Web_Console">Web Console</a></li>
   <li><a href="/en-US/docs/Tools/Debugger">Debugger</a></li>
   <li><a href="/en-US/docs/Tools/Network_Monitor">Network Monitor</a></li>
   <li><a href="/en-US/docs/Tools/Storage_Inspector">Storage Inspector</a></li>
   <li><a href="/en-US/docs/Tools/GCLI">Developer Toolbar</a></li>
   <li><a href="/en-US/docs/Tools/3D_View">3D View</a></li>
   <li><a href="/en-US/docs/Tools/Eyedropper">Eyedropper</a></li>
   <li><a href="/en-US/docs/tools/Working_with_iframes">Selecting iframes</a></li>
   <li><a href="/en-US/docs/Tools/View_source">View Source</a></li>
  </ol>
 </li>
 <li><a href="#">Mobile</a>
  <ol>
   <li><a href="/en-US/Firefox_OS/Using_the_App_Manager">App Manager</a></li>
   <li><a href="/en-US/docs/Tools/WebIDE">WebIDE</a></li>
   <li><a href="/en-US/docs/Tools/Remote_Debugging/Firefox_for_Android">Firefox for Android</a></li>
   <li><a href="/en-US/docs/Tools/Firefox_OS_Simulator">Firefox OS Simulator</a></li>
   <li><a href="/en-US/docs/Tools/Responsive_Design_View">Responsive Design View</a></li>
  </ol>
 </li>
 <li><a href="/en-US/docs/Tools/Performance">Performance</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Performance/Frame_rate">Frame rate graph</a></li>
   <li><a href="/en-US/docs/Tools/Performance/Waterfall">Waterfall</a></li>
   <li><a href="/en-US/docs/Tools/Performance/Call_Tree">Call Tree</a></li>
   <li><a href="/en-US/docs/Tools/Performance/Flame_Chart">Flame Chart</a></li>
   <li><a href="/en-US/docs/Tools/Paint_Flashing_Tool">Paint Flashing Tool</a></li>
   <li><a href="/en-US/docs/Tools/Web_Console#Reflow_events">Reflow Event Logging</a></li>
   <li><a href="/en-US/docs/Tools/Network_Monitor#Performance_analysis">Network Performance</a></li>
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
 <li><a href="/en-US/docs/Tools_Toolbox#Settings">Settings</a></li>
 <li><a href="/en-US/docs/Tools/Release_notes">Release notes</a></li>
</ol>

