---
version: prototype1
revision_id: 1320753
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
<h3 id="Getting_started">Erste Schritte</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/What_are_WebExtensions_">Was sind WebExtensions?</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Your_first_WebExtension">Deine erste WebExtension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Your_second_WebExtension">Deine zweite WebExtension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Anatomy_of_a_WebExtension">Anatomie einer WebExtension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Examples">Beispiel-WebExtensions</a></li>
</ul>

<h3 id="How_to">Kurzanleitungen</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Intercept_HTTP_requests">Abfangen von HTTP-Anfragen</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Modify_a_web_page">Eine Web-Seite verändern</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Add_a_button_to_the_toolbar">Eine Schaltfläche zu einer Werkzeugleiste hinzufügen</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Implement_a_settings_page">Eine Einstellungen-Seite erstellen</a></li>
 <li>Browser-Tabs beeinflussen</li>
 <li>Zugreifen auf und verändern von Lesezeichen</li>
 <li>Zugreifen auf und verändern von Cookies</li>
</ul>

<h3 id="Concepts">Konzepte</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Using_the_JavaScript_APIs">Verwendung der JavaScript-APIs</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Content_scripts">Content scripts</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Match_patterns">Match patterns</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Internationalization">Internationalisierung</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Content_Security_Policy">Content Security Policy</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Native_messaging">Native messaging</a></li>
</ul>

<h3 id="Porting">Portieren</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/Porting_from_Google_Chrome">Portieren einer Google Chrome-Erweiterung</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">Portieren eines veralteten Firefox Add-ons</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Embedded_WebExtensions">Eingebettete WebExtensions</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_the_Add-on_SDK">Vergleich mit dem Add-on SDK</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_XUL_XPCOM_extensions">Vergleich mit XUL/XPCOM-Erweiterungen</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Chrome_incompatibilities">Inkompatibilitäten mit Chrome</a></li>
</ul>

<h3 id="Firefox_workflow">Firefox workflow</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/Temporary_Installation_in_Firefox">Installation</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Debugging">Debugging</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Getting_started_with_web-ext">Einstieg in Web-Ext</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/web-ext_command_reference">Web-Ext Befehlsreferenz</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/WebExtensions_and_the_Add-on_ID">WebExtensions und die Add-On-ID</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Publishing_your_WebExtension">Veröffentlichen deiner WebExtension</a></li>
</ul>
</div>

<div class="section">
<h3 id="Reference">Referenz</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/API">JavaScript-API-Überblick</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">Tabellen zur Browser-Kompatibilität zu JavaScript-APIs</a></li>
</ul>

<h4 id="JavaScript_APIs">JavaScript APIs</h4>

<div class="twocolumns">{{ ListSubpages ("/en-US/Add-ons/WebExtensions/API") }}</div>

<h4 id="Manifest_keys">Manifest keys</h4>

<div class="twocolumns">{{ ListSubpages ("/en-US/Add-ons/WebExtensions/manifest.json") }}</div>
</div>
</div>

