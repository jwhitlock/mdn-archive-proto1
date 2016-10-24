---
version: prototype1
revision_id: 1133887
locale: en-US
slug: Mozilla/Add-ons/WebExtensions
tags: "add-on" "Landing" "Extensions" "WebExtensions"
title: WebExtensions
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<p>WebExtensions are a cross-browser system for developing browser add-ons. To a large extent the system is compatible with the <a class="external-icon external" href="https://developer.chrome.com/extensions">extension API</a> supported by Google Chrome and Opera. Extensions written for these browsers will in most cases run in Firefox or <a href="https://developer.microsoft.com/en-us/microsoft-edge/platform/documentation/extensions/">Microsoft Edge</a> with <a href="https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Porting_from_Google_Chrome">just a few changes</a>. The API is also fully compatible with <a href="https://developer.mozilla.org/en-US/Firefox/Multiprocess_Firefox">multiprocess Firefox</a>.</p>

<p>We're also intending to extend the APIs to support the needs of add-on developers, so if you have ideas, we'd love to hear them. You can reach us on the <a href="https://mail.mozilla.org/listinfo/dev-addons">dev-addons mailing list</a> or <a href="irc://irc.mozilla.org/webextensions">#webextensions</a> on <a href="https://wiki.mozilla.org/IRC">IRC</a>.</p>

<div class="row topicpage-table">
<div class="section">
<h3 id="Getting_started">Getting started</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/What_are_WebExtensions">What are WebExtensions?</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Your_first_WebExtension">Your first WebExtension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Your_second_WebExtension">Your second WebExtension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Anatomy_of_a_WebExtension">Anatomy of a WebExtension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Examples">Example WebExtensions</a></li>
</ul>

<h3 id="How_to">How to</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Intercept_HTTP_requests">Intercept HTTP requests</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Modify_a_web_page">Modify a web page</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Add_a_button_to_the_toolbar">Add a button to the toolbar</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Implement_a_settings_page">Implement a settings page</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Interact_with_the_clipboard">Interact with the clipboard</a></li>
 <li>Manipulate browser tabs</li>
 <li>Access and modify bookmarks</li>
 <li>Access and modify cookies</li>
</ul>

<h3 id="Concepts">Concepts</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Using_the_JavaScript_APIs">Using the JavaScript APIs</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/User_interface_components">User interface components</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Content_scripts">Content scripts</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Match_patterns">Match patterns</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Internationalization">Internationalization</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Content_Security_Policy">Content Security Policy</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Native_messaging">Native messaging</a></li>
</ul>

<h3 id="Porting">Porting</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/Porting_from_Google_Chrome">Porting a Google Chrome extension</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">Porting a legacy Firefox add-on</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Embedded_WebExtensions">Embedded WebExtensions</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_the_Add-on_SDK">Comparison with the Add-on SDK</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_XUL_XPCOM_extensions">Comparison with XUL/XPCOM extensions</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Chrome_incompatibilities">Chrome incompatibilities</a></li>
</ul>

<h3 id="Firefox_workflow">Firefox workflow</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/Temporary_Installation_in_Firefox">Installation</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Debugging">Debugging</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Getting_started_with_web-ext">Getting started with web-ext</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/web-ext_command_reference">web-ext command reference</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/WebExtensions_and_the_Add-on_ID">WebExtensions and the Add-on ID</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Publishing_your_WebExtension">Publishing your WebExtension</a></li>
</ul>
</div>

<div class="section">
<h3 id="Reference">Reference</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/API">JavaScript API overview</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">Browser compatibility tables for JavaScript APIs</a></li>
</ul>

<h4 id="JavaScript_APIs">JavaScript APIs</h4>

<div class="twocolumns">{{ ListSubpages ("/en-US/Add-ons/WebExtensions/API") }}</div>

<h4 id="Manifest_keys">Manifest keys</h4>

<div class="twocolumns">{{ ListSubpages ("/en-US/Add-ons/WebExtensions/manifest.json") }}</div>
</div>
</div>

