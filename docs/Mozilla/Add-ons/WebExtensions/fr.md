---
version: prototype1
revision_id: 1344039
locale: fr
slug: Mozilla/Add-ons/WebExtensions
tags: "Landing" "Extensions" "WebExtensions"
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

<p>Les WebExtensions constituent le système permettant de développer des extensions multinavigateurs. De manière générale, ce système est compatible avec l'<a href="https://developer.chrome.com/extensions">API d'extensions</a> supportée par Google Chrome, Opera et le <a href="https://browserext.github.io/browserext/">W3C Draft Community Group</a>. Les extensions écrites pour ces navigateurs fonctionneront dans la plupart des cas sous Firefox ou Microsoft Edge, après <a href="/fr/Add-ons/WebExtensions/Porting_a_Google_Chrome_extension">seulement quelques petits changements</a>. L'API est aussi totalement compatible avec <a href="/fr/Firefox/Multiprocessus_Firefox">le multiprocessus de Firefox</a>.</p>

<p>Nous avons l'intention d'étendre les API en fonction des besoins des développeurs d'extensions. Si vous avez des idées ou des questions, n'hésitez pas à nous en faire part. Si vous avez besoin d'aide pour migrer une extension obsolète, vous pouvez aussi nous joindre sur la <a href="https://mail.mozilla.org/listinfo/dev-addons">dev-addons mailing list</a> ou le canal <a href="irc://irc.mozilla.org/webextensions">#webextensions</a> sur <a href="https://wiki.mozilla.org/IRC">IRC</a>.</p>

<div class="row topicpage-table">
<div class="section">
<h2 id="Démarrage">Démarrage</h2>

<ul>
 <li><a href="/fr/Add-ons/WebExtensions/What_are_WebExtensions">Que sont les WebExtensions ?</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Your_first_WebExtension">Votre première WebExtension</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Your_second_WebExtension">Votre seconde WebExtension</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Anatomy_of_a_WebExtension">Anatomie d'une WebExtension</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Examples">Exemples de WebExtensions</a></li>
</ul>

<h2 id="Mode_d'emploi">Mode d'emploi</h2>

<ul>
 <li><a href="/fr/Add-ons/WebExtensions/Intercepter_requêtes_HTTP">Intercepter les requêtes HTTP</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Modify_a_web_page">Modifier une page web</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Ajouter_un_bouton_a_la_barre_d_outils">Ajouter un bouton à la barre d'outils</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Ajouter_une_page_de_paramètres">Mettre en place une page de paramètres</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/interagir_avec_le_presse_papier">Interagir avec le presse-papier</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Travailler_avec_l_API_Tabs">Travailler avec l'API Tabs</a></li>
</ul>

<h2 id="Interface_utilisateur">Interface utilisateur</h2>

<ul>
 <li><a href="/fr/docs/Mozilla/Add-ons/WebExtensions/user_interface">Introduction</a></li>
 <li><a href="/fr/docs/Mozilla/Add-ons/WebExtensions/user_interface/Browser_action">Bouton de la barre d'outils</a></li>
 <li><a href="/fr/docs/Mozilla/Add-ons/WebExtensions/user_interface/Popups">Bouton de la barre d'outils avec un popup</a></li>
 <li><a href="/fr/docs/Mozilla/Add-ons/WebExtensions/user_interface/Page_actions">Bouton de la barre d'adresse</a></li>
 <li><a href="/fr/docs/Mozilla/Add-ons/WebExtensions/user_interface/Popups">Bouton de la barre d'adresse avec un popup</a></li>
 <li><a href="/fr/docs/Mozilla/Add-ons/WebExtensions/user_interface/elements_menu_contextuel">Elements du menu contextuel</a></li>
 <li><a href="/fr/docs/Mozilla/Add-ons/WebExtensions/user_interface/barres_laterales">Barres laterales</a></li>
 <li><a href="/fr/docs/Mozilla/Add-ons/WebExtensions/user_interface/Options_pages">Options page</a></li>
 <li><a href="/fr/docs/Mozilla/Add-ons/WebExtensions/user_interface/extension_pages">Extension pages</a></li>
 <li><a href="/fr/docs/Mozilla/Add-ons/WebExtensions/user_interface/Notifications">Notifications</a></li>
 <li><a href="/fr/docs/Mozilla/Add-ons/WebExtensions/user_interface/Omnibox">Suggestions de la barre d'adresse</a></li>
 <li><a href="/fr/docs/Mozilla/Add-ons/WebExtensions/user_interface/panneaux_devtools">Panneaux devtools de développement</a></li>
</ul>

<h2 id="Concepts">Concepts</h2>

<ul>
 <li><a href="/fr/Add-ons/WebExtensions/API">Utilisation des API JavaScript</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Content_scripts">Scripts de contenu</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Match_patterns">Motifs (Match patterns)</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Working_with_files">Travailler avec les fichiers</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Internationalization">Internationalisation</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Content_Security_Policy">Politique de sécurité du contenu</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Native_messaging">Messages natifs</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/extension_des_outils_de_developpement">Utilisation des API devtools</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/User_experience_best_practices">Bonne pratiques expérience utilisateur</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/manifests_native">Manifests Natif</a></li>
</ul>

<h2 id="Portage">Portage</h2>

<ul>
 <li><a href="/fr/Add-ons/WebExtensions/Porting_a_Google_Chrome_extension">Porter une extension Google Chrome</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Portage_d_une_extension_Firefox_heritee">Porter une ancienne extension Firefox</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Embedded_WebExtensions">WebExtensions intégrées</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Developing_WebExtensions_for_Firefox_for_Android">Développer pour Firefox pour Android</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Comparaison_avec_le_SDK_Add-on">Comparaison avec le Add-on SDK</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Comparison_with_XUL_XPCOM_extensions">Comparaison avec les extensions XUL/XPCOM</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Chrome_incompatibilities">Incompatibilités avec Chrome</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Differences_between_desktop_and_Android">Différence entre le bureau et l'Android</a></li>
</ul>

<h2 id="Déroulement_avec_Firefox">Déroulement avec Firefox</h2>

<ul>
 <li><a href="/fr/Add-ons/WebExtensions/installation_temporaire_dans_Firefox">Installation</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Debugging">Débogage</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Getting_started_with_web-ext">Démarrer avec web-ext</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/web-ext_command_reference">Détail de la commande web-ext</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/WebExtensions_and_the_Add-on_ID">Les WebExtensions et l'ID Add-on</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Alternative_distribution_options">Options de distribution Alternatives</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Publishing_your_WebExtension">Publier votre WebExtension</a></li>
</ul>
</div>

<div class="section">
<h2 id="Références">Références</h2>

<h3 id="Les_APIs_JavaScript">Les APIs JavaScript</h3>

<ul>
 <li><a href="/fr/docs/Mozilla/Add-ons/WebExtensions/API">Aperçu de l'API JavaScript</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">Tableau des compatibilités de navigateur pour les API JavaScript</a></li>
</ul>

<div class="twocolumns">{{ ListSubpages ("/fr/Add-ons/WebExtensions/API") }}</div>

<h3 id="Clés_de_Manifest">Clés de Manifest</h3>

<ul>
 <li><a href="/fr/Add-ons/WebExtensions/manifest.json">Présentation de manifest.json</a></li>
 <li><a href="/fr/Add-ons/WebExtensions/Browser_compatibility_for_manifest.json">Compatibilité du navigateur pour manifest.json</a></li>
</ul>

<div class="twocolumns">{{ ListSubpages ("/fr/Add-ons/WebExtensions/manifest.json") }}</div>
</div>
</div>

