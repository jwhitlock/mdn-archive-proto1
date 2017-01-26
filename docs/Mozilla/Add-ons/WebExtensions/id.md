---
version: prototype1
revision_id: 1176407
locale: id
slug: Mozilla/Add-ons/WebExtensions
tags: "TopicStub" "NeedsTranslation"
title: WebExtensions
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<p><span id="result_box" lang="id"><span title="WebExtensions are a cross-browser system for developing browser add-ons.">WebExtensions adalah sistem cross-browser untuk mengembangkan browser add-ons. </span><span title="To a large extent the API is compatible with the extension API supported by Google Chrome and Opera.">Untuk sebagian besar API tersebut kompatibel dengan</span></span> <a class="external-icon external" href="https://developer.chrome.com/extensions">extension API</a> <span id="result_box" lang="id"><span title="To a large extent the API is compatible with the extension API supported by Google Chrome and Opera.">yang didukung oleh Google Chrome dan Opera</span></span>. <span id="result_box" lang="id"><span title="Extensions written for these browsers will in most cases run in Firefox or Microsoft Edge with just a few changes.">Ekstensi ditulis untuk browser ini dalam banyak kasus akan berjalan di Firefox atau </span></span><a href="https://developer.microsoft.com/en-us/microsoft-edge/platform/documentation/extensions/">Microsoft Edge</a><span lang="id"><span title="Extensions written for these browsers will in most cases run in Firefox or Microsoft Edge with just a few changes."> hanya</span></span> dengan <a href="https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Porting_from_Google_Chrome">beberapa erubahan</a>. <span id="result_box" lang="id"><span title="The API is also fully compatible with multiprocess Firefox.

">API ini juga sepenuhnya kompatibel dengan</span></span> <a href="https://developer.mozilla.org/en-US/Firefox/Multiprocess_Firefox">multiprocess Firefox</a>.</p>

<p><span id="result_box" lang="id"><span title="We're also intending to extend the APIs to support the needs of add-on developers, so if you have ideas, we'd love to hear them.">Kami juga berniat untuk memperpanjang API untuk mendukung kebutuhan para pengembang, jadi jika Anda memiliki ide, kami akan senang mendengar mereka. </span><span title="You can reach us on the dev-addons mailing list or #webextensions on IRC.

">Anda dapat menghubungi kami</span></span> <a href="https://mail.mozilla.org/listinfo/dev-addons">dev-addons mailing list</a> atau <a href="irc://irc.mozilla.org/webextensions">#webextensions</a> di <a href="https://wiki.mozilla.org/IRC">IRC</a>.</p>

<div class="row topicpage-table">
<div class="section">
<h3 id="Getting_started">Memulai</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/What_are_WebExtensions">Apa Itu WebExtensions?</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Your_first_WebExtension">WebExtension Pertama Anda</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Your_second_WebExtension">WebExtension Kedua Anda</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Anatomy_of_a_WebExtension">Anatomi dari WebExtension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Examples">Contoh WebExtensions</a></li>
</ul>

<h3 id="How_to">Bagaimana</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Intercept_HTTP_requests">Menangkap HTTP requests</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Modify_a_web_page">Merubah halaman web</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Add_a_button_to_the_toolbar">Menambah button ke toolbar</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Implement_a_settings_page">Implementasi pengaturan halaman</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Interact_with_the_clipboard">Interaksi dengan clipboard</a></li>
 <li>Memanipulasi tab browser</li>
 <li>Akses dan modifikasi bookmarks</li>
 <li>Akses dan modifikasi cookies</li>
</ul>

<h3 id="Concepts">Konsep</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/API">Meninjau JavaScript API</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/User_interface_components">Komponen User interface</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Content_scripts">Content scripts</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Match_patterns">Match patterns</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Internationalization">Internasionalisasi</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Content_Security_Policy">Content Security Policy</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Native_messaging">Native messaging</a></li>
</ul>

<h3 id="Porting">Porting</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/Porting_from_Google_Chrome">Porting&nbsp; ekstensi Google Chrome</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">Porting legacy Firefox add-on</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Embedded_WebExtensions">Embedded WebExtensions</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_the_Add-on_SDK">Perbandingan dengan the Add-on SDK</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_XUL_XPCOM_extensions">Perbandingan dengan XUL/XPCOM extensions</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Chrome_incompatibilities">Chrome incompatibilities</a></li>
</ul>

<h3 id="Firefox_workflow">Alur Kerja Firefox</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/Temporary_Installation_in_Firefox">Pemasangan</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Debugging">Debugging</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Getting_started_with_web-ext">Memulai dengan web-ext</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/web-ext_command_reference">Referensi perintah web-ext</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/WebExtensions_and_the_Add-on_ID">WebExtensions dan Add-on ID</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Publishing_your_WebExtension">Penerbitan WebExtension anda</a></li>
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

