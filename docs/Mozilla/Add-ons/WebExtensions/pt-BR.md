---
version: prototype1
revision_id: 1341628
locale: pt-BR
slug: Mozilla/Add-ons/WebExtensions
tags: "Passo a passo" "WebExtension"
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

<p>Extensões são capazes de extender e modificar a capacidade de um navegador. As extensões para Firefox são feitas usando WebExtensions APIs, um sistema de cross-browser para desenvolvimento de extensões. Para uma maior amplitude o API é compatível com <a class="external-icon external" href="https://developer.chrome.com/extensions">extension API</a> suportado pelo Google Chrome e Opera. Extensões escritas para esses navegadores vão, em muitos casos, rodar no Firefox e Microsoft Edge <a href="https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Porting_from_Google_Chrome">com poucas mudanças</a>. O API é também totalmente compatível com o <a href="https://developer.mozilla.org/en-US/Firefox/Multiprocess_Firefox">multiprocess Firefox</a>.</p>

<p>Se você tem dúvidas ou sugestões, ou precisa de ajuda para migrar um add-on antigo para o WebExtensions APIs, você pode entrar em contato conosco pela <a class="external external-icon" href="https://mail.mozilla.org/listinfo/dev-addons">newsletter de dev-addons </a>ou <a href="irc://irc.mozilla.org/extdev">#extdev</a> no <a class="external-icon external" href="https://wiki.mozilla.org/IRC">IRC</a>.</p>

<div class="row topicpage-table">
<div class="section">
<h3 id="Começando">Começando</h3>

<ul>
 <li><a href="https://developer.mozilla.org/pt-BR/Add-ons/WebExtensions/What_are_WebExtensions">O que é uma extensão </a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Your_first_WebExtension">Sua primeira extensão</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Your_second_WebExtension">Sua segunda extensão</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Anatomy_of_a_WebExtension">Anatomia de uma extensão</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Examples">Exemplos de extensões</a></li>
</ul>

<h3 id="Como">Como</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Intercept_HTTP_requests">Interceptar solicitações de HTTP</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Modify_a_web_page">Modificar uma página de Web</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Add_a_button_to_the_toolbar">Adicionar um botão na barra de ferramenta</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Implement_a_settings_page">Implementar uma página de configurações</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Interact_with_the_clipboard">Interagir com a área de transferência</a></li>
</ul>

<h3 id="User_interface">User interface</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface">Introdução</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Browser_action">Botão na Barra de Ferramenta</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Popups">Botão na Barra de Ferramenta com um popup</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Page_actions">Botão na Barra de Endereço</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Popups">Botão na Barra de Endereço com um popup</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Context_menu_items">Itens de Menu de contexto</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Sidebars">Sidebars</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Options_pages">Página de Opções</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Bundled_web_pages">Páginas web incluídas</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Notifications">Notificação</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/Omnibox">Sugestões na Barra de Endereço</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface/devtools_panels">Developer tools panels</a></li>
</ul>

<h3 id="Conceitos">Conceitos</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/API">Visão geral de JavaScript API</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Content_scripts">Content scripts</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Match_patterns">Match patterns</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Internationalization">Internacionalização</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Content_Security_Policy">Política de Segurança</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Native_messaging">Mensagem Nativa</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Using_the_devtools_APIs">Usando o devtools APIs</a></li>
</ul>

<h3 id="Portabilidade">Portabilidade</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">Portandouma extensão de Google Chrome</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">Portando uma extensão antiga de Firefox </a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Embedded_WebExtensions">Embedded WebExtensions</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_the_Add-on_SDK">Comparação com Add-on SDK</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_XUL_XPCOM_extensions">Comparação com extensão XUL/XPCOM extensions</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Chrome_incompatibilities">Imcompatibilidades Chrome</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Differences_between_desktop_and_Android">Diferenças entre desktop e Android</a></li>
</ul>

<h3 id="Fluxo_de_trabalho_do_Firefox">Fluxo de trabalho do Firefox</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/Temporary_Installation_in_Firefox">Instalando</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Debugging">Debugging</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Developing_WebExtensions_for_Firefox_for_Android">Desenvolvendo para Firefox Android</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Getting_started_with_web-ext">Começando com web-ext</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/web-ext_command_reference">Referência de web-ext command</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/WebExtensions_and_the_Add-on_ID">Extensão e o Add-on ID</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Publishing_your_WebExtension">Publicando uma extesãoPublishing your extension</a></li>
</ul>
</div>

<div class="section">
<h3 id="Reference">Reference</h3>

<h4 id="JavaScript_APIs">JavaScript APIs</h4>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/API">Visão geral de JavaScript API </a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">Browser compatibility tables for JavaScript APIs</a></li>
</ul>

<div class="twocolumns">{{ ListSubpages ("/en-US/Add-ons/WebExtensions/API") }}</div>

<h4 id="Manifest_keys">Manifest keys</h4>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json">manifest.json overview</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Browser_compatibility_for_manifest.json">Browser compatibility for manifest.json</a></li>
</ul>

<div class="twocolumns">{{ ListSubpages ("/en-US/Add-ons/WebExtensions/manifest.json") }}</div>
</div>
</div>

