---
version: prototype1
revision_id: 489369
locale: cs
slug: Tools
tags: "Tools" "TopicStub" "NeedsMarkupWork" "Web Development" "NeedsTranslation" "Developing Mozilla" "Web Development:Tools" "NeedsTechnicalReview"
title: Firefox Developer Tools
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: 6fc2e2910d0b2514fe7144ca40b00c5d740d7412
---
<div class="summary">
 Examine, edit, and debug HTML, CSS, and JavaScript on the desktop and on mobile</div>
<div class="column-container zone-callout">
 <h3 id="What's_new_in_Aurora.3F"><a href="https://hacks.mozilla.org/2013/11/firefox-developer-tools-episode-27-edit-as-html-codemirror-more/" title="Aurora Hacks post">What's new in Aurora?</a></h3>
 The <a href="http://www.mozilla.org/en-US/firefox/aurora/" title="http://www.mozilla.org/en-US/firefox/aurora/">current Firefox Aurora release</a> is Firefox 27, and includes these updates to the developer tools:
 <ul>
  <li>Instruct the debugger to <a href="/en-US/docs/Tools/Debugger#Break_on_a_DOM_event">break on DOM events</a> to which you're listening</li>
  <li><a href="/en-US/docs/Tools/Page_Inspector#Editing_HTML">Edit HTML in the Inspector</a></li>
  <li>See color swatches and background images in the Inspector's <a href="/en-US/docs/Tools/Page_Inspector#Rules_view">Rules view</a></li>
  <li>The Web Console now <a href="/en-US/docs/Tools/Web_Console#Reflow_events">logs reflow events</a></li>
  <li>CodeMirror is now used as the source editor in many tools</li>
 </ul>
</div>
<div class="column-container">
 <p><img alt="" src="https://mdn.mozillademos.org/files/6111/debugger-800.png" style="width: 800px; height: 360px; display: block; margin-left: auto; margin-right: auto;" />You can use the developer tools to <a href="/en-US/docs/Tools/Page_Inspector" title="/en-US/docs/Tools/Page_Inspector">examine and edit HTML and CSS</a>, to <a href="/en-US/docs/Tools/Debugger" title="/en-US/docs/Tools/Debugger">debug JavaScript</a>, and to <a href="/en-US/docs/Tools/Web_Console#The_command_line_interpreter" title="/en-US/docs/Tools/Web_Console#The_command_line_interpreter">run JavaScript in the page</a>. You can use them to <a href="/en-US/docs/Tools/Network_Monitor" title="/en-US/docs/Tools/Network_Monitor">see network requests</a> that your browser makes as well as any <a href="/en-US/docs/Tools/Web_Console" title="/en-US/docs/Tools/Web_Console">JavaScript and CSS warnings and errors</a> that it encounters when loading a page. You can use them to <a href="/en-US/docs/Tools/Profiler" title="/en-US/docs/Tools/Profiler">debug performance problems with your site</a>.</p>
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
  <h2 id="Standalone_Tools">Standalone Tools</h2>
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
    Also known as "Tilt", this provides a 3D visualisation of the current page.</dd>
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
<div class="overheadIndicator communitybox">
 <div class="column-container">
  <div class="column-half">
   <h2 id="Join_the_Community">Join the Community</h2>
   <h3 id="Developer_Tools_forum">Developer Tools forum</h3>
   <ul class="communitymailinglist">
    <li><a href="https://lists.mozilla.org/listinfo/dev-developer-tools">As a mailing list</a></li>
    <li><a href="news://news.mozilla.org/mozilla.dev.developer-tools">As a newsgroup</a></li>
    <li><a href="https://groups.google.com/forum/#!forum/mozilla.dev.developer-tools">As a Google Group</a></li>
   </ul>
  </div>
  <div class="column-half">
   <ul class="communitycontact">
    <li><strong>IRC: </strong><a href="http://mibbit.com/?channel=%23devtools&amp;server=irc.mozilla.org">#devtools</a> on <a href="http://irc.mozilla.org/">irc.mozilla.org</a></li>
    <li><strong>Wiki: </strong><a href="https://wiki.mozilla.org/DevTools">https://wiki.mozilla.org/DevTools</a></li>
   </ul>
  </div>
 </div>
</div>
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
   <li><a href="/en-US/docs/Tools/Debugging_Firefox_JS_Code" title="Debugging Firefox JS code">Debugging Firefox JS Code</a></li>
  </ol>
 </li>
</ol>
<p>&nbsp;</p>
<p>&nbsp;</p>
