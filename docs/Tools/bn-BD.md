---
version: prototype1
revision_id: 800975
locale: bn-BD
slug: Tools
tags: "NeedsReview"
title: ফায়ারফক্স ডেভেলপার টুল
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div class="summary"><span class="seoSummary">ডেস্কটপ এবং মোবাইলে HTML, CSS এবং জাভাস্ক্রিপ্ট পরীক্ষা, সম্পাদন এবং ডিবাগ করুন</span></div>

<div class="column-container zone-callout"><a href="https://www.mozilla.org/firefox/channel/#aurora" style="float: right; margin-bottom: 20px; padding: 10px; text-align: center; border-radius: 4px; display: inline-block; background-color: #81BC2E; white-space: nowrap; color: white; text-shadow: 0px 1px 0px rgba(0, 0, 0, 0.25); box-shadow: 0px 1px 0px 0px rgba(0, 0, 0, 0.2), 0px -1px 0px 0px rgba(0, 0, 0, 0.3) inset;" target="_">ফায়ারফক্স অরোরা ইন্সটল করুন</a>

<h3 id="What's_new_in_Aurora.3F" name="What's_new_in_Aurora.3F">অরোরাতে নতুন কি আছে?</h3>

<p>অরোরা হচ্ছে ফায়ারফক্সের প্রিভিউ বিল্ড, যেখানে আপনি যেকোনো নতুন ফিচার সর্বসাধারণের জন্য উন্মুক্ত করার আগেই ব্যবহারের সুযোগ পাবেন। বর্তমান অরোরাতে ডেভেলপার টুলসে নিচের আপডেট সমূহ রয়েছে:</p>

<ul>
 <li><a href="/en-US/docs/Tools/Storage_Inspector">স্টোরেজ ইনস্পেক্টর: একটি নতুন টূল, যেটা আপনাকে ওয়েব পেজ সমূহের স্টোর করা ডাটা সমূহ দেখতে সহায়তা করবে</a></li>
 <li><a href="/en-US/docs/Tools/Performance">পারফরম্যান্স টূল: উন্নত প্রফাইলার ইউজার ইন্টারফেস এবং ফ্রেমরেট টাইমলাইন</a></li>
 <li><a href="/en-US/docs/tools/Working_with_iframes">ফ্রেম সুইচিং: পেজের মধ্যে একটি নির্দিষ্ট iframe এ ডেভেলপার টুলসকে কেন্দ্রীভূত করতে পারবেন</a></li>
 <li><a href="/en-US/docs/Web/API/Console.table">console.table সমর্থন</a></li>
 <li><a href="/en-US/docs/Tools/Page_Inspector#Examining_event_listeners">পেজ ইনস্পেক্টরের মধ্যে এখন jQuery ইভেন্ট দেখা যায়</a></li>
 <li><a href="/en-US/docs/Tools/Adding_a_panel_to_the_toolbox">টুলবক্সে নতুন প্যানেল যুক্ত করার জন্য এক্সটেনশন এপিআই।</a></li>
</ul>
</div>

<div class="column-container zone-callout"><a href="http://mzl.la/devtools" style="float: right; margin-bottom: 20px; padding: 10px; text-align: center; border-radius: 4px; display: inline-block; background-color: #81BC2E; white-space: nowrap; color: white; text-shadow: 0px 1px 0px rgba(0, 0, 0, 0.25); box-shadow: 0px 1px 0px 0px rgba(0, 0, 0, 0.2), 0px -1px 0px 0px rgba(0, 0, 0, 0.3) inset;" target="_">আপনার আইডিয়া শেয়ার করুন</a>

<h3 id="Share_your_ideas" name="Share_your_ideas">আপনার আইডিয়া শেয়ার করুন</h3>

<p>ডেভেলপার টুলসে নতুন ফিচারের জন্য অনুরোধ করুন অথবা অন্যান্য ডেভেলপারের আবেদন করা আইডিয়ার জন্য ভোট করুন।</p>
</div>

<p><img alt="" src="https://mdn.mozillademos.org/files/7307/inspector.png" style="display:block; height:467px; margin-left:auto; margin-right:auto; width:815px" /></p>

<div class="column-container">
<div class="column-half">
<h2 id="Creating" name="Creating">তৈরি করা</h2>

<p>ওয়েবসাইট এবং ওয়েব অ্যাপ এর জন্য অথরিং টুলস।</p>

<dl>
 <dt><a href="/en-US/docs/Tools/Scratchpad">স্ক্র্যাচপ্যাড</a></dt>
 <dd>ফায়ারফক্স এর ভেতরে একটি টেক্সট এডিটর দেয়া আছে যা আপনাকে জাভাস্ক্রিপ্ট লিখতে এবং এক্সিকিউট করতে দেয়।</dd>
 <dt><a href="/en-US/docs/Tools/Style_Editor">স্টাইল এডিটর</a></dt>
 <dd>বর্তমান পেজ এর CSS স্টাইল দেখুন এবং এডিট করুন।</dd>
 <dt><a href="/en-US/docs/Tools/Shader_Editor">শেডার এডিটর</a></dt>
 <dd>WebGL এর ব্যবহার করা ফ্র্যাগমেন্ট শেডার সহ সবকিছু দেখুন এবং সম্পাদনা করুন</dd>
 <dt><a href="/en-US/docs/Tools/Web_Audio_Editor">ওয়েব অডিও এডিটর</a></dt>
 <dd>একটি অডিও কনটেক্সটে অডিও নোডের গ্রাফ পরীক্ষা করুন এবং তাদের প্যারামিটার পরিবর্তন করুন।</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Exploring" name="Exploring">Exploring and debugging</h2>

<p>Examine, explore, and debug websites and web apps.</p>

<dl>
 <dt><a href="/en-US/docs/Tools/Web_Console">Web Console</a></dt>
 <dd>See messages logged a web page, and interact with the page using JavaScript.</dd>
 <dt><a href="/en-US/docs/Tools/Page_Inspector">Page Inspector</a></dt>
 <dd>View and modify the page HTML and CSS.</dd>
 <dt><a href="/en-US/docs/Tools/Debugger">JavaScript Debugger</a></dt>
 <dd>Stop, step through, examine and modify the JavaScript running in a page.</dd>
 <dt><a href="/en-US/docs/Tools/Network_Monitor">Network Monitor</a></dt>
 <dd>See the network requests made when a page is loaded.</dd>
 <dt><a href="/en-US/docs/Tools/Storage_Inspector">Storage Inspector</a></dt>
 <dd>Inspect cookies, local storage, indexedDB and session storage present in a page.</dd>
 <dt><a href="/en-US/docs/Tools/GCLI">Developer Toolbar</a></dt>
 <dd>A command-line interface for the developer tools.</dd>
 <dt><a href="/en-US/docs/Tools/3D_View">3D View</a></dt>
 <dd>3D visualization of the page.</dd>
 <dt><a href="/en-US/docs/Tools/Eyedropper">Eyedropper</a></dt>
 <dd>Select a color from the page.</dd>
 <dt><a href="/en-US/docs/Tools/Working_with_iframes">Working with iframes</a></dt>
 <dd>How to target a particular iframe.</dd>
</dl>
</div>
</div>

<hr />
<div class="column-container">
<div class="column-half">
<h2 id="Mobile" name="Mobile">মোবাইল</h2>

<p>মোবাইল ডেভেলপ করার টুলস সমূহ.</p>

<dl>
 <dt>অ্যাপ ম্যানেজার</dt>
 <dd>ফায়ারফক্স ওএস অ্যাপ ডিজাইন এবং ডেভেলপ।</dd>
 <dt><a href="/en-US/docs/Tools/WebIDE">WebIDE</a></dt>
 <dd>অ্যাাপ ম্যানেজারের প্রতিস্তাপক যা ফায়ারফক্স ৩৩ ভার্সন থেকে শুরু হয়েছে।</dd>
 <dt><a href="/en-US/docs/Tools/Firefox_OS_Simulator">Firefox OS Simulator</a></dt>
 <dd>Run and debug your Firefox OS app on the desktop, without needing a real Firefox OS device.</dd>
 <dt><a href="/en-us/docs/Tools/Responsive_Design_View">Responsive Design View</a></dt>
 <dd>See how your website or app will look on different screen sizes without changing the size of your browser window.</dd>
 <dt><a href="/en-US/docs/Tools/Remote_Debugging/Firefox_for_Android">Debugging on Firefox for Android</a></dt>
 <dd>Connect the developer tools to Firefox for Android.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Performance" name="Performance">Performance</h2>

<p>Diagnose and fix performance problems.</p>

<dl>
 <dt><a href="/en-US/docs/Tools/Performance">Performance tool</a></dt>
 <dd>Revamped JS profiler and frame rate timeline.</dd>
</dl>

<dl>
 <dt><a href="/en-US/docs/Tools/Profiler">JavaScript Profiler</a></dt>
 <dd>Figure out where your JavaScript code is spending its time.</dd>
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
</div>

<hr />
<h2 id="More_resources" name="More_resources">More resources</h2>

<p>This section lists resources which aren't maintained by Mozilla's developer tools team, but which are widely used by web developers. We've included a few Firefox add-ons in this list, but for the complete list see the <a href="https://addons.mozilla.org/en-US/firefox/extensions/web-development/">“Web Development” category on addons.mozilla.org</a>.</p>

<div class="column-container">
<div class="column-half">
<dl>
 <dt><a href="https://www.getfirebug.com/">Firebug</a></dt>
 <dd>A very popular and powerful web development tool, including a JavaScript debugger, HTML and CSS viewer and editor, and network monitor.</dd>
 <dt><a href="/en-US/docs/DOM_Inspector">DOM Inspector</a></dt>
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
<div>{{CommunityBox("Developer tools", "dev-developer-tools", "mozilla.dev.developer-tools", "devtools", "Team info|https://wiki.mozilla.org/DevTools|Dev tools wiki|Designs and plans for the dev tools||Blog|https://hacks.mozilla.org/|Hacks blog|Hacks blog")}}</div>

<h2 id="Subnav" name="Subnav">Subnav</h2>

<ol>
 <li><a href="#">তৈরি করা</a>

  <ol>
   <li><a href="/en-US/docs/Tools/Scratchpad">স্ক্র্যাচ প্যাড</a></li>
   <li><a href="/en-US/docs/Tools/Style_Editor">স্টাইল এডিটর</a></li>
   <li><a href="/en-US/docs/Tools/Shader_Editor">শেডার এডিটর</a></li>
   <li><a href="/en-US/docs/Tools/Web_Audio_Editor">ওয়েব অডিও এডিটর</a></li>
  </ol>
 </li>
 <li><a href="#">ডিবাগ করা</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Page_Inspector">পেজ ইন্সপেক্টর</a></li>
   <li><a href="/en-US/docs/Tools/Web_Console">ওয়েব কনসোল</a></li>
   <li><a href="/en-US/docs/Tools/Debugger">ডিবাগার</a></li>
   <li><a href="/en-US/docs/Tools/Network_Monitor">নেটওয়ার্ক মনিটর</a></li>
   <li><a href="/en-US/docs/Tools/Storage_Inspector">স্টোরেজ ইন্সপেক্টর</a></li>
   <li><a href="/en-US/docs/Tools/GCLI">ডেভেলপার টুলবার</a></li>
   <li><a href="/en-US/docs/Tools/3D_View">3D ভিউ</a></li>
   <li><a href="/en-US/docs/Tools/Eyedropper">আইড্রপার</a></li>
   <li><a href="/en-US/docs/tools/Working_with_iframes">iframe নির্বাচন করা</a></li>
  </ol>
 </li>
 <li><a href="#">মোবাইল</a>
  <ol>
   <li><a href="/en-US/Firefox_OS/Using_the_App_Manager">অ্যাপ ম্যানেজার</a></li>
   <li><a href="/en-US/docs/Tools/WebIDE">WebIDE</a></li>
   <li><a href="/en-US/docs/Tools/Remote_Debugging/Firefox_for_Android">Firefox for Android</a></li>
   <li><a href="/en-US/docs/Tools/Firefox_OS_Simulator">Firefox OS সিমুলেটর</a></li>
   <li><a href="/en-US/docs/Tools/Responsive_Design_View">রেসপন্সিভ ডিজাইন ভিউ</a></li>
  </ol>
 </li>
 <li><a href="#">Performance</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Performance">Performance</a></li>
   <li><a href="/en-US/docs/Tools/Profiler">Profiler</a></li>
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
<style type="text/css">::-moz-selection { color: #000; background: none repeat scroll 100% 0% transparent;text-shadow: 0px 0px 2px #0048FF;} a::selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 2px 2px 2px #0048FF;} ::selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 2px 0px 2px #0048FF;}  input::selection { color: #3356C6; background: none repeat scroll 0% 0% transparent;} a::selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 2px 0px 2px #0048FF;} ::-webkit-selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 0px 0px 2px #0048FF;} a::selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 2px 2px 2px #0048FF;} ::-ms-selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 0px 0px 2px #0048FF;} a::selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 2px 2px 2px #0048FF;} ::-o-selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 0px 0px 2px #0048FF;} a::selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 2px 2px 2px #0048FF;}
</style>
<style type="text/css">::-moz-selection { color: #000; background: none repeat scroll 100% 0% transparent;text-shadow: 0px 0px 2px #0048FF;} a::selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 2px 2px 2px #0048FF;} ::selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 2px 0px 2px #0048FF;}  input::selection { color: #3356C6; background: none repeat scroll 0% 0% transparent;} a::selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 2px 0px 2px #0048FF;} ::-webkit-selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 0px 0px 2px #0048FF;} a::selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 2px 2px 2px #0048FF;} ::-ms-selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 0px 0px 2px #0048FF;} a::selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 2px 2px 2px #0048FF;} ::-o-selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 0px 0px 2px #0048FF;} a::selection { color: #000; background: none repeat scroll 0% 0% transparent;text-shadow: 2px 2px 2px #0048FF;}
</style>

