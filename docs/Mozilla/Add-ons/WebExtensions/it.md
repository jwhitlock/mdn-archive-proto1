---
version: prototype1
revision_id: 1214329
locale: it
slug: Mozilla/Add-ons/WebExtensions
tags: 
title: WebExtensions
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: True
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<p>Le WebExtensions sono un metodo cross-browser per sviluppare add-on. In larga parte il metodo è compatibile con le <a class="external-icon external" href="https://developer.chrome.com/extensions">extension API</a> supportate da Google, Chrome e Opera. Le estensioni create per questi browsers funzioneranno con <a href="https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Porting_from_Google_Chrome">poche modifiche</a> su Firefox o <a href="https://developer.microsoft.com/en-us/microsoft-edge/platform/documentation/extensions/">Microsoft Edge</a>. Le API sono anche completamente compatibili con <a href="https://developer.mozilla.org/en-US/Firefox/Multiprocess_Firefox">Firefox multiprocesso</a>.</p>

<p>Vogliamo continuare ad estendere le API per supportare le necessità degli sviluppatori di add-ons, perciò se hai idee, ci piacerebbe sentirle. Contattaci su <a href="https://mail.mozilla.org/listinfo/dev-addons">dev-addons mailing list</a> o <a href="irc://irc.mozilla.org/webextensions">#webextensions</a> su <a href="https://wiki.mozilla.org/IRC">IRC</a>.</p>

<div class="row topicpage-table">
<div class="section">
<h3 id="Iniziare">Iniziare</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/What_are_WebExtensions">Cosa sono le WebExtensions?</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Your_first_WebExtension">La tua prima WebExtension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Your_second_WebExtension">La seconda WebExtension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Anatomy_of_a_WebExtension">Anatomia di una WebExtension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Examples">Esempi di WebExtensions</a></li>
</ul>

<h3 id="Come_fare">Come fare</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Intercept_HTTP_requests">Rilevare richieste HTTP</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Modify_a_web_page">Modificare una pagina web</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Add_a_button_to_the_toolbar">Aggiungere un bottone alla toolbar</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Implement_a_settings_page">Creare una pagina impostazioni</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Interact_with_the_clipboard">Interagire con la clipboard</a></li>
 <li>Manipolare le tabs del browser</li>
 <li>Accedere e modificare bookmarks</li>
 <li>Accedere e modificare&nbsp;cookies</li>
</ul>

<h3 id="Concetti">Concetti</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/API">JavaScript API overview</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/User_interface_components">Componenti UI</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Content_scripts">Scripts contenuto</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Match_patterns">Match di patterns</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Internationalization">Internationazionalizzazione</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Content_Security_Policy">Policy di Sicurezza dei Contenuti</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Native_messaging">Messaging Nativo</a></li>
</ul>

<h3 id="Porting">Porting</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/Porting_from_Google_Chrome">Porting di una estensione Google Chrome</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">Porting di un add-on Firefox</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Embedded_WebExtensions">Embedded WebExtensions</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_the_Add-on_SDK">Comparazione con la Add-on SDK</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_XUL_XPCOM_extensions">Comparazione con le estensioni XUL/XPCOM</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Chrome_incompatibilities">Incompatibilità di Chrome</a></li>
</ul>

<h3 id="Firefox_workflow">Firefox workflow</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/Temporary_Installation_in_Firefox">Installazione</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Debugging">Debugging</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Getting_started_with_web-ext">Iniziare con la web-ext</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/web-ext_command_reference">web-ext reference comandi</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/WebExtensions_and_the_Add-on_ID">WebExtensions e la Add-on ID</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Publishing_your_WebExtension">Pubblicare la tua WebExtension</a></li>
</ul>
</div>

<div class="section">
<h3 id="Riferimenti">Riferimenti</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/API">JavaScript API overview</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">Compatibilità dei Browser con le APIs JavaScript</a></li>
</ul>

<h4 id="JavaScript_APIs">JavaScript APIs</h4>

<div class="twocolumns">{{ ListSubpages ("/en-US/Add-ons/WebExtensions/API") }}</div>

<h4 id="Manifest_keys">Manifest keys</h4>

<div class="twocolumns">{{ ListSubpages ("/en-US/Add-ons/WebExtensions/manifest.json") }}</div>
</div>
</div>

