---
version: prototype1
revision_id: 514469
locale: en-US
slug: Tools
tags: "Guide" "Tools" "l10n:priority" "Web Development" "Developing Mozilla" "Web Development:Tools"
title: Firefox Developer Tools
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div class="summary">
 Examine, edit, and debug HTML, CSS, and JavaScript on the desktop and on mobile</div>
<div class="column-container zone-callout">
 <h3 id="What's_new_in_Aurora.3F"><a href="https://hacks.mozilla.org/2013/12/split-console-pretty-print-minified-js-and-more-firefox-developer-tools-episode-28/" title="Aurora Hacks post">What's new in Aurora?</a></h3>
 <p>The <a href="http://www.mozilla.org/en-US/firefox/aurora/" title="http://www.mozilla.org/en-US/firefox/aurora/">current Firefox Aurora release</a> is Firefox 28. These are the main updates to the developer tools:</p>
 <ul>
  <li>The App Manager has an integrated <a href="/en-US/Firefox_OS/Using_the_App_Manager#Manifest_editor">manifest editor</a></li>
  <li>The <a href="/en-US/docs/Tools/Web_Console#The_split_console">Split Console</a> feature enables you to use the Web Console and another developer tool side by side</li>
  <li><a href="/en-US/docs/Tools/Debugger#Pretty-print_a_minified_file">Pretty-print minified JavaScript</a> in the Debugger</li>
  <li><a href="/en-US/docs/Tools/Page_Inspector#Rules_view">Color picker tooltip</a> in the Inspector</li>
  <li><a href="/en-US/docs/Tools/Browser_Toolbox">Browser Toolbox</a> for debugging platform or add-on code</li>
 </ul>
</div>
<div class="column-container">
 <p><img alt="" src="https://mdn.mozillademos.org/files/6111/debugger-800.png" style="width: 800px; height: 360px; display: block; margin-left: auto; margin-right: auto;" /><span class="seoSummary">You can use the Firefox developer tools to <a href="/en-US/docs/Tools/Page_Inspector" title="/en-US/docs/Tools/Page_Inspector">examine and edit HTML and CSS</a>, to <a href="/en-US/docs/Tools/Debugger" title="/en-US/docs/Tools/Debugger">debug JavaScript</a>, and to <a href="/en-US/docs/Tools/Web_Console#The_command_line_interpreter" title="/en-US/docs/Tools/Web_Console#The_command_line_interpreter">run JavaScript in the page</a>.</span> You can use them to <a href="/en-US/docs/Tools/Network_Monitor" title="/en-US/docs/Tools/Network_Monitor">see network requests</a> that your browser makes as well as any <a href="/en-US/docs/Tools/Web_Console" title="/en-US/docs/Tools/Web_Console">JavaScript and CSS warnings and errors</a> that it encounters when loading a page. You can use them to <a href="/en-US/docs/Tools/Profiler" title="/en-US/docs/Tools/Profiler">debug performance problems with your site</a>.</p>
 <p>You can use the developer tools to <a href="/en-US/docs/Tools/Remote_Debugging" title="/en-US/docs/Tools/Remote_Debugging">debug code running Firefox for Android</a>, and soon, Firefox OS. We've also provided tools that target mobile development: the <a href="/en-US/docs/Tools/Responsive_Design_View" title="/en-US/docs/Tools/Responsive_Design_View">Responsive Design View</a> is a quick way to see how a site will look on a small screen, and the <a href="/en-US/docs/Tools/Firefox_OS_Simulator" title="/en-US/docs/https://developer.mozilla.org/en-US/docs/Tools/Firefox_OS_Simulator">Firefox OS Simulator</a> lets you run and debug a Firefox OS app on the desktop without needing to use a real Firefox OS device.</p>
 <p>Firefox add-ons can access the debugger API, so you can build your own developer tools that extend and enhance the built-in tools. With the <a href="https://wiki.mozilla.org/Remote_Debugging_Protocol" title="https://wiki.mozilla.org/Remote_Debugging_Protocol">remote debugging protocol</a> you can implement your own debugging clients and servers, enabling you to debug websites using your own tools or to debug different targets using the Firefox tools.</p>
</div>
<hr />
<div class="column-container">
 <div class="column-third">
  <h2 id="Tools" name="Tools">Toolbox</h2>
  <p>The <a href="/en-US/docs/Tools/Toolbox" title="/en-US/docs/Tools/Toolbox">Toolbox</a> provides a single home for most of the developer tools that are built into Firefox.</p>
  <dl>
   <dt>
    <a href="/en-US/docs/Tools/Page_Inspector" title="Tools/Page_Inspector">Page Inspector</a></dt>
   <dd>
    View and modify the HTML and CSS for the selected element.</dd>
   <dt>
    <a href="/en-US/docs/Tools/Web_Console" title="Tools/Web_Console">Web Console </a></dt>
   <dd>
    See informational, warning and error messages emitted by the browser loading a web page, and examine and manipulate the page using JavaScript.</dd>
   <dt>
    <a href="/en-US/docs/Tools/Style_Editor" title="Tools/Style_Editor">Style Editor</a></dt>
   <dd>
    View and edit CSS styles for the current page.</dd>
   <dt>
    <a href="/en-US/docs/Tools/Debugger" title="Tools/Debugger">JavaScript Debugger</a></dt>
   <dd>
    Step through JavaScript code that is running in the browser and watch variables to help track down bugs.</dd>
   <dt>
    <a href="/en-US/docs/Tools/Profiler" title="Tools/Profiler">JavaScript Profiler</a></dt>
   <dd>
    Use the profiler to figure out where your JavaScript code is spending its time.</dd>
   <dt>
    <a href="/en-US/docs/Tools/Network_Monitor" title="Tools/Network_Monitor">Network Monitor</a></dt>
   <dd>
    Inspect all the network requests that are made when a page is loaded, and how long they take to execute.</dd>
   <dt>
    <a href="/en-US/docs/Tools/Shader_Editor">Shader Editor</a></dt>
   <dd>
    View and edit the vertex and fragment shaders used by <a href="https://developer.mozilla.org/en-US/docs/Web/WebGL">WebGL</a>.</dd>
  </dl>
 </div>
 <div class="column-third">
  <h2 id="Mobile">Mobile</h2>
  <p>Of course, mobile web developers are web developers too, so most of the web development tools will be interesting to mobile web developers as well. But we've also created some tools specifically aimed at mobile development.</p>
  <dl>
   <dt>
    <a href="/en-US/docs/Tools/Remote_Debugging" title="Tools/Remote_Debugging">Remote Debugging</a></dt>
   <dd>
    Use the developer tools to debug your Android device over USB.</dd>
   <dt>
    <a href="/en-US/docs/Tools/Firefox_OS_Simulator" title="Tools/Firefox_OS_Simulator">Firefox OS Simulator</a></dt>
   <dd>
    Run and debug your Firefox OS app on the desktop, without needing to use a real Firefox OS device.</dd>
   <dt>
    <a href="/en-us/docs/Tools/Responsive_Design_View" title="/en-us/docs/Tools/Responsive_Design_View">Responsive Design View</a></dt>
   <dd>
    See how your website or app will look on different screen sizes without changing the size of your browser window.</dd>
  </dl>
 </div>
 <div class="column-third">
  <h2 id="Standalone_tools">Standalone tools</h2>
  <p>These tools ship inside Firefox as well, but their user interfaces aren't integrated into the Toolbox.</p>
  <dl>
   <dt>
    <a href="/en-US/docs/Tools/Scratchpad" title="Tools/Scratchpad">Scratchpad</a></dt>
   <dd>
    A text editor built into Firefox that lets you write and execute JavaScript.</dd>
   <dt>
    <a href="/en-us/docs/Tools/Browser_Console" title="/en-us/docs/Tools/Responsive_Design_View">Browser Console</a></dt>
   <dd>
    See messages from all JavaScript code running in the browser including content, chrome, and add-ons. Execute JavaScript code in the chrome window's context.</dd>
   <dt>
    <a href="https://developer.mozilla.org/en-US/docs/Tools/GCLI" title="en/Tools/GCLI">Developer Toolbar</a></dt>
   <dd>
    A command-line interface to manipulate and work with the developer tools in Firefox, and buttons for quick access to the most commonly used tools.</dd>
   <dt>
    <a href="/en-US/docs/Tools/3D_View" title="Tools/3D_View">3D View</a></dt>
   <dd>
    Also known as "Tilt", this provides a 3D visualization of the current page.</dd>
   <dt>
    <a href="/en-US/docs/Tools/Paint_Flashing_Tool" title="Tools/Paint_Flashing_Tool">Paint Flashing Tool</a></dt>
   <dd>
    The paint flashing tool highlights the part of the browser window that are repainted in response to events, helping to diagnose potential performance problems with your site.</dd>
  </dl>
 </div>
</div>
<hr />
<h2 id="More_resources">More resources</h2>
<p>This section lists resources which aren't maintained by Mozilla's developer tools team, but which are widely used by web developers. We've included a few Firefox add-ons in this list, but for the complete list see the <a href="https://addons.mozilla.org/en-US/firefox/extensions/web-development/" title="https://addons.mozilla.org/en-US/firefox/extensions/web-development/">"Web Development" category on addons.mozilla.org</a>.</p>
<dl>
 <dt>
  <a href="https://www.getfirebug.com/" title="Firebug">Firebug</a></dt>
 <dd>
  A very popular and powerful web development tool, including a JavaScript debugger, HTML and CSS viewer and editor, and network monitor.</dd>
 <dt>
  <a href="https://developer.mozilla.org/en-US/docs/DOM_Inspector" title="DOM_Inspector">DOM Inspector</a></dt>
 <dd>
  Inspect, browse, and edit the DOM of web pages or XUL windows.</dd>
 <dt>
  <a href="https://addons.mozilla.org/en-US/firefox/addon/web-developer/" title="Web-Developer">Web Developer</a></dt>
 <dd>
  Adds a menu and a toolbar to the browser with various web developer tools.</dd>
 <dt>
  <a href="https://webmaker.org/en-US/tools/" title="https://webmaker.org/en-US/tools/">Webmaker Tools</a></dt>
 <dd>
  A set of tools developed by Mozilla, aimed at people getting started with Web development.</dd>
 <dt>
  <a href="http://www.w3.org/Status.html" title="W3C">W3C Validators</a></dt>
 <dd>
  The W3C website hosts a number of tools to check the validity of your website, including its <a href="http://validator.w3.org/" title="http://validator.w3.org/">HTML</a> and <a href="http://jigsaw.w3.org/css-validator/" title="http://jigsaw.w3.org/css-validator/">CSS</a>.</dd>
 <dt>
  <a href="http://www.jshint.com/" title="JSHint">JSHint</a></dt>
 <dd>
  JavaScript code analysis tool.</dd>
</dl>
<hr />
<p>{{CommunityBox("Developer tools", "dev-developer-tools", "mozilla.dev.developer-tools", "devtools", "Other links|https://wiki.mozilla.org/DevTools|Dev tools wiki|Designs and plans for the dev tools")}}</p>
<h2 id="Subnav">Subnav</h2>
<ol>
 <li><a href="/en-US/docs/Tools/Toolbox">Toolbox</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Page_Inspector" title="Tools/Page_Inspector">Page Inspector</a></li>
   <li><a href="/en-US/docs/Tools/Web_Console" title="Web Console">Web Console</a></li>
   <li><a href="/en-US/docs/Tools/Style_Editor" title="Style Editor">Style Editor</a></li>
   <li><a href="/en-US/docs/Tools/Debugger" title="Debugger">Debugger</a></li>
   <li><a href="/en-US/docs/Tools/Profiler" title="Profiler">Profiler</a></li>
   <li><a href="/en-US/docs/Tools/Network_Monitor" title="Network Monitor">Network Monitor</a></li>
   <li><a href="/en-US/docs/Tools/Shader_Editor">Shader Editor</a></li>
  </ol>
 </li>
 <li><a href="#">Mobile</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Remote_Debugging" title="Remote Debugging">Remote Debugging</a></li>
   <li><a href="/en-US/docs/Tools/Firefox_OS_Simulator" title="Firefox OS Simulator">Firefox OS Simulator</a></li>
   <li><a href="/en-US/docs/Tools/Responsive_Design_View" title="Responsive Design View">Responsive Design View</a></li>
  </ol>
 </li>
 <li><a href="#">Standalone tools</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Scratchpad" title="Scratchpad">Scratchpad</a></li>
   <li><a href="/en-US/docs/Tools/Browser_Console" title="Browser Console">Browser Console</a></li>
   <li><a href="/en-US/docs/Tools/GCLI" title="GCLI">Developer Toolbar</a></li>
   <li><a href="/en-US/docs/Tools/3D_View" title="3D View">3D View</a></li>
   <li><a href="/en-US/docs/Tools/Paint_Flashing_Tool" title="Paint Flashing Tool">Paint Flashing Tool</a></li>
   <li><a href="/en-US/docs/Tools/Browser_Toolbox" title="Browser Toolbox">Browser Toolbox</a></li>
  </ol>
 </li>
</ol>
<p>&nbsp;</p>
<p>&nbsp;</p>

