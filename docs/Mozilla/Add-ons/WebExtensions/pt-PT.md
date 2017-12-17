---
version: prototype1
revision_id: 1337807
locale: pt-PT
slug: Mozilla/Add-ons/WebExtensions
tags: "Extras" "Landing" "Extensões" "Extensões da Web"
title: Extensões de Navegador
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<div class="m2">
<div class="mrg">
<div class="client" id="baseBody" style="BOTTOM: -67px">
<div id="textContainer" style="DISPLAY: block">
<div id="FtxtWnd" style="BOTTOM: 0px">
<div class="targetTxt">
<div class="txtDiv border3d" id="targetTxt" style="FONT-FAMILY: Tahoma !important; DIRECTION: ltr; TEXT-ALIGN: left">
<p>As extensões podem ampliar e modificar a capacidade de um navegador. As extensões para Firefox são criadas utilizando a API de WebExtensions, um sistema de navegador cruzado para desenvolver extensões. Em grande medida, o sistema é compatível com a <a class="external-icon external" href="https://developer.chrome.com/extensions">API de extensão</a> suportada pelo Google Chrome, Opera e <a href="https://browserext.github.io/browserext/">W3C Draft Community Group</a>. As extensões escritas para estes navegadores irão na maioria dos casos ser executadas no Firefox ou <a href="https://docs.microsoft.com/pt-pt/microsoft-edge/extensions">Microsoft Edge</a> com <a href="/pt-PT/Add-ons/WebExtensions/Trasnsferir_extensao_Google_Chrome">apenas algumas alterações</a>. A API também é totalmente compatível com <a href="/pt-PT/Firefox/Multiprocess_Firefox">os multiprocessos do Firefox</a>.</p>

<p>Se tiver ideias ou questões, ou precisar de ajuda para migrar um extra legado para utilizar as APIs de WebExtensions, pode contactar-nos em <a href="https://mail.mozilla.org/listinfo/dev-addons">lista de discussões dev-addons</a> ou <a href="irc://irc.mozilla.org/webextensions">#webextensions</a> no <a href="https://wiki.mozilla.org/IRC">IRC</a></p>

<div class="row topicpage-table">
<div class="section">
<h2 id="Iniciação">Iniciação</h2>

<ul>
 <li><a href="/pt-PT/Add-ons/WebExtensions/O_que_sao_WebExtensions">O que são WebExtensions?</a></li>
 <li><a href="/pt-PT/Add-ons/WebExtensions/A_sua_primeira_extensao">A sua primeir Extensão da Web</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Your_second_WebExtension">Your second WebExtension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Anatomy_of_a_WebExtension">Anatomy of a WebExtension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Examples">Example WebExtensions</a></li>
</ul>

<h2 id="Como...">Como...</h2>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Intercept_HTTP_requests">Intercept HTTP requests</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Modify_a_web_page">Modify a web page</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Add_a_button_to_the_toolbar">Add a button to the toolbar</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Implement_a_settings_page">Implement a settings page</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Interact_with_the_clipboard">Interact with the clipboard</a></li>
</ul>

<h2 id="Interface_do_utilizador">Interface do utilizador</h2>

<ul>
 <li><a href="/pt-PT/Add-ons/WebExtensions/interface_do_utilizador">Introdução</a></li>
 <li><a href="/pt-PT/Add-ons/WebExtensions/interface_do_utilizador/Ação_navegador">Botão da barra de ferramentas do navegador</a></li>
 <li><a href="/pt-PT/Add-ons/WebExtensions/interface_do_utilizador/Popups">Botão da barra de ferramentas do navegador com uma janela (<em>popup</em>)</a></li>
 <li><a href="/pt-PT/Add-ons/WebExtensions/interface_do_utilizador/Acoes_pagina">Botão da barra de endereço</a></li>
 <li><a href="/pt-PT/Add-ons/WebExtensions/interface_do_utilizador/Popups">Botão da barra de endereço com uma janela (<em>popup</em>)</a></li>
 <li><a href="/pt-PT/Add-ons/WebExtensions/interface_do_utilizador/Itens_do_menu_de_contexto">Itens do meno de contexto</a></li>
 <li><a href="/pt-PT/Add-ons/WebExtensions/interface_do_utilizador/Barras_laterais">Barras laterais</a></li>
 <li><a href="/pt-PT/Add-ons/WebExtensions/interface_do_utilizador/Options_pages">Página de opções</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Bundled_web_pages">Bundled web pages</a></li>
 <li><a href="/pt-PT/Add-ons/WebExtensions/interface_do_utilizador/Notificacoes">Notificações</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Omnibox">Address bar suggestions</a></li>
 <li><a href="/pt-PT/Add-ons/WebExtensions/interface_do_utilizador/devtools_panels">Painés das ferramentas de desenvolvimento</a></li>
</ul>

<h2 id="Conceitos">Conceitos</h2>

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

<h2 id="Transferência">Transferência</h2>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/Porting_from_Google_Chrome">Porting a Google Chrome extension</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">Porting a legacy Firefox extension</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Developing_WebExtensions_for_Firefox_for_Android">Developing for Firefox for Android</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Embedded_WebExtensions">Embedded WebExtensions</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_the_Add-on_SDK">Comparison with the Add-on SDK</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_XUL_XPCOM_extensions">Comparison with XUL/XPCOM extensions</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Chrome_incompatibilities">Chrome incompatibilities</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Differences_between_desktop_and_Android">Differences between desktop and Android</a></li>
</ul>

<h2 id="Fluxo_de_trabalho_do_Firefox">Fluxo de trabalho do Firefox</h2>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/User_experience_best_practices">User experience</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Temporary_Installation_in_Firefox">Installation</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Debugging">Debugging</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Getting_started_with_web-ext">Getting started with web-ext</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/web-ext_command_reference">web-ext command reference</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/WebExtensions_and_the_Add-on_ID">Extensions and the Add-on ID</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Alternative_distribution_options">Alternative distribution options</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Publishing_your_WebExtension">Publishing your extension</a></li>
</ul>
</div>

<div class="section">
<h2 id="Referência">Referência</h2>

<h3 id="APIS_de_JavaScript">APIS de JavaScript</h3>

<ul>
 <li><a href="/pt-PT/Add-ons/WebExtensions/API">Sinopse de API de JavaScript API</a></li>
 <li><a href="/pt-PT/Add-ons/WebExtensions/Suporte_navegador_APIs_JavaScript">Tabelas de compatibilidade de navegador para as APIs de JavaScript</a></li>
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
</div>
</div>
</div>
</div>
</div>
</div>
</div>

