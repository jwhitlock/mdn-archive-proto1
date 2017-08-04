---
version: prototype1
revision_id: 1283455
locale: en-US
slug: Mozilla/Add-ons/WebExtensions
tags: "add-on" "Landing" "Extensions" "WebExtensions"
title: Browser extensions
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<p>Extensions can extend and modify the capability of a browser. Extensions for Firefox are built using WebExtension APIs, a cross-browser system for developing extensions. To a large extent the system is compatible with the <a class="external-icon external" href="https://developer.chrome.com/extensions">extension API</a> supported by Google Chrome and Opera and the <a href="https://browserext.github.io/browserext/">W3C Draft Community Group</a>. Extensions written for these browsers will in most cases run in Firefox or <a href="https://developer.microsoft.com/en-us/microsoft-edge/platform/documentation/extensions/">Microsoft Edge</a> with <a href="https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Porting_from_Google_Chrome">just a few changes</a>. The API is also fully compatible with <a href="https://developer.mozilla.org/en-US/Firefox/Multiprocess_Firefox">multiprocess Firefox</a>.</p>

<p>If you have ideas or questions, or need help migrating a legacy add-on to use WebExtension APIs, you can reach us on the <a href="https://mail.mozilla.org/listinfo/dev-addons">dev-addons mailing list</a> or <a href="irc://irc.mozilla.org/extdev">#extdev</a> on <a href="https://wiki.mozilla.org/IRC">IRC</a>.</p>

<div class="row topicpage-table">
<div class="section">
<h2 id="Getting_started">Getting started</h2>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/What_are_WebExtensions">What are extensions?</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Your_first_WebExtension">Your first extension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Your_second_WebExtension">Your second extension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Anatomy_of_a_WebExtension">Anatomy of an extension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Examples">Example extensions</a></li>
</ul>

<h2 id="How_to">How to</h2>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Intercept_HTTP_requests">Intercept HTTP requests</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Modify_a_web_page">Modify a web page</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Add_a_button_to_the_toolbar">Add a button to the toolbar</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Implement_a_settings_page">Implement a settings page</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Interact_with_the_clipboard">Interact with the clipboard</a></li>
</ul>

<h2 id="User_interface">User interface</h2>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface">Introduction</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Browser_action">Browser toolbar button</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Popups">Browser toolbar button with a popup</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Page_actions">Address bar button</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Popups">Address bar button with a popup</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Context_menu_items">Context menu items</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Sidebars">Sidebars</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Options_pages">Options page</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Bundled_web_pages">Bundled web pages</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Notifications">Notifications</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Omnibox">Address bar suggestions</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/devtools_panels">Developer tools panels</a></li>
</ul>

<h2 id="Concepts">Concepts</h2>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/API">JavaScript API overview</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Content_scripts">Content scripts</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Match_patterns">Match patterns</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Working_with_files">Working with files</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Internationalization">Internationalization</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Content_Security_Policy">Content Security Policy</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Native_messaging">Native messaging</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Using_the_devtools_APIs">Using the devtools APIs</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/User_experience_best_practices">User experience best practices</a></li>
</ul>

<h2 id="Porting">Porting</h2>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/Porting_from_Google_Chrome">Porting a Google Chrome extension</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">Porting a legacy Firefox extension</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Embedded_WebExtensions">Embedded WebExtensions</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_the_Add-on_SDK">Comparison with the Add-on SDK</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_XUL_XPCOM_extensions">Comparison with XUL/XPCOM extensions</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Chrome_incompatibilities">Chrome incompatibilities</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Differences_between_desktop_and_Android">Differences between desktop and Android</a></li>
</ul>

<h2 id="Firefox_workflow">Firefox workflow</h2>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/Temporary_Installation_in_Firefox">Installation</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Debugging">Debugging</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Developing_WebExtensions_for_Firefox_for_Android">Developing for Firefox for Android</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Getting_started_with_web-ext">Getting started with web-ext</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/web-ext_command_reference">web-ext command reference</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/WebExtensions_and_the_Add-on_ID">Extensions and the Add-on ID</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Alternative_distribution_options">Alternative distribution options</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Publishing_your_WebExtension">Publishing your extension</a></li>
</ul>
</div>

<div class="section">
<h2 id="Reference">Reference</h2>

<h3 id="JavaScript_APIs">JavaScript APIs</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/API">JavaScript API overview</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">Browser compatibility tables for JavaScript APIs</a></li>
</ul>

<div class="twocolumns">{{ ListSubpages ("/en-US/Add-ons/WebExtensions/API") }}</div>

<h3 id="Manifest_keys">Manifest keys</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json">manifest.json overview</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Browser_compatibility_for_manifest.json">Browser compatibility for manifest.json</a></li>
</ul>

<div class="twocolumns">{{ ListSubpages ("/en-US/Add-ons/WebExtensions/manifest.json") }}</div>
</div>
</div>

