---
version: prototype1
revision_id: 1269333
locale: de
slug: Mozilla/Add-ons/WebExtensions
tags: 
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

<p>WebExtensions sind ein Cross-Browser-System zur Entwicklung von Browser-Add-ons. Das System ist in weiten Teilen kompatibel mit der <a class="external-icon external" href="https://developer.chrome.com/extensions">extension API</a>, welche von Google Chrome und Opera unterstützt wird. Erweiterungen, welche für diese Browser geschrieben wurden, werden in den meisten Fällen mit <a href="https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Porting_from_Google_Chrome">nur wenigen Anpassungen</a> auch in Firefox oder <a href="https://developer.microsoft.com/en-us/microsoft-edge/platform/documentation/extensions/">Microsoft Edge</a> lauffähig sein. Die API ist außerdem vollständig kompatibel mit <a href="https://developer.mozilla.org/en-US/Firefox/Multiprocess_Firefox">Multiprozess-Firefox</a>.</p>

<p>Wir beabsichtigen auch, die APIs zu erweitern, um die Unterstützung für Add-on-Entwickler zu verbessern. Sollten Sie Vorschläge dazu haben, würden wir uns über Ihre Mitteilung freuen. Sie erreichen uns über die englischsprachige <a href="https://mail.mozilla.org/listinfo/dev-addons">Mailingliste für Add-on-Entwickler</a> oder auf <a href="irc://irc.mozilla.org/webextensions">#webextensions</a> im <a href="https://wiki.mozilla.org/IRC">IRC</a>.</p>

<div class="row topicpage-table">
<div class="section">
<h3 id="Getting_started">Getting started</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/What_are_WebExtensions_">What are WebExtensions?</a></li>
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
 <li>Manipulate browser tabs</li>
 <li>Access and modify bookmarks</li>
 <li>Access and modify cookies</li>
</ul>

<h3 id="Concepts">Concepts</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Using_the_JavaScript_APIs">Using the JavaScript APIs</a></li>
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

