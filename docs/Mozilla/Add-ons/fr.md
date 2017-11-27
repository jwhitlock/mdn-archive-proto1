---
version: prototype1
revision_id: 1330845
locale: fr
slug: Mozilla/Add-ons
tags: "Add-ons" "Landing" "Modules" "Mozilla" "Extensions"
title: Modules
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<p><span class="seoSummary">Les modules complémentaires (<em>add-ons</em>) permettent aux développeurs d'ajouter et de modifier les fonctionnalités de Firefox.</span> Les modules sont écrits à l'aide de technologies web standard : JavaScript, HTML, et CSS - et d'API JavaScript spécifiques à ces modules. Un module complémentaire peut, par exemple, être utilisé pour :</p>

<ul>
 <li>Modifier l'apparence ou le contenu de certains sites web</li>
 <li>Modifier l'interface utilisateur de Firefox</li>
 <li>Ajouter de nouvelles fonctionnalités à Firefox</li>
</ul>

<h2 id="Développer_des_modules_complémentaires">Développer des modules complémentaires</h2>

<p>Actuellement, il existe différents outils et formats pour développer des modules complémentaires pour Firefox. Cependant, d'ici à fin 2017, <a href="/fr/Add-ons/WebExtensions">WebExtensions</a> deviendra le format standard. Les autres outils (le SDK Add-On par exemple) seront alors dépréciés.</p>

<p><a href="/fr/Add-ons/WebExtensions" style="margin-left: auto; margin-right: auto; margin-bottom: 20px; padding: 10px; text-align: center; border-radius: 4px; display: block; width: 30%; background-color: #81BC2E; color: white; text-shadow: 0px 1px 0px rgba(0, 0, 0, 0.25); box-shadow: 0px 1px 0px 0px rgba(0, 0, 0, 0.2), 0px -1px 0px 0px rgba(0, 0, 0, 0.3) inset;">En savoir plus à propos des WebExtensions</a></p>

<p>Si vous développez un nouveau module complémentaire, nous vous recommandons d'utiliser WebExtension.</p>

<p>Les extensions WebExtensions sont conçues afin de pouvoir être utilisées sur différents navigateurs. Les extensions WebExtensions écrites pour Firefox fonctionneront pour la plupart dans Chrome, Edge et Opera et nécessiteront au pire peu de changement pour obtenir cette compatibilité. Elles sont également compatibles avec le mode multi-processus de Firefox.<br />
 <br />
 <a href="/fr/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">Voici la liste des API actuellement prises en charge par Firefox et les autres navigateurs</a>. Nous continuons à concevoir et à implémenter de nouvelles API afin de répondre aux besoins des développeurs.<br />
 <br />
 La plupart des API utilisées pour WebExtension sont également disponibles pour Firefox pour Android.</p>

<h3 id="Migrer_un_module_existant">Migrer un module existant</h3>

<p>Si vous maintenez un module complémentaire historique utilisant XUL ou le SDK Add-on, nous vous recommandons de le porter vers une extension WebExtensions. <a href="/fr/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">Voici quelques ressources MDN à propos du portage d'extension</a>.</p>

<p>Nous avons rassemblé <a href="https://wiki.mozilla.org/Add-ons/developer/communication">un ensemble de ressources</a> sur un page wiki afin d'aider les développeurs pendant cette phase de transition. Pour commencer, vous pouvez utiliser l'outil <a href="https://compatibility-lookup.services.mozilla.com/">Lookup </a>afin de détecter si votre module complémentaire est impacté.</p>

<h2 id="Publier_des_modules">Publier des modules</h2>

<p><a href="https://addons.mozilla.org">addons.mozilla.org</a>, aussi appelé AMO, est le site officiel de Mozilla sur lequel sont publiés les modules complémentaires et que les utilisateurs peuvent parcourir pour découvrir de nouveaux modules. Publier un module complémentaire sur AMO permet d'entretenir la communauté d'utilisateurs et de créateurs de modules. C'est également une ressource essentielle pour qu'un module puisse être découvert.</p>

<p>Il n'est pas nécessaire que votre module soit publié sur AMO. En revanche, votre module doit être signé par Mozilla afin que les utilisateurs puissent l'installer.</p>

<p><a href="/fr/Add-ons/Distribution">Dans cet article</a>, vous trouverez différentes informations relatives au processus de publication.</p>

<h2 id="Les_autres_types_de_modules">Les autres types de modules</h2>

<p>Généralement, lorsqu'on évoque les modules complémentaires, on parle des extensions. Ceci étant dit, il existe d'autres types de modules qui permettent aux utilisateurs de personnaliser Firefox. Ces modules peuvent être :</p>

<ul>
 <li><a href="/fr/Add-ons/Thèmes/Fond">Des thèmes légers</a> : un outil simple qui permet de personnaliser Firefox de façon limitée</li>
 <li><a href="/fr/docs/Extensions/Mobile">Les modules mobiles</a> : des modules complémentaires destinés à Firefox pour Android. Attention, certaines des API utilisées pour ces modules sont dépréciées (ou le seront dans un avenir proche). Par la suite, Firefox pour Android prendra pleinement en charge le format WebExtension</li>
 <li><a href="/fr/Add-ons/Creating_OpenSearch_plugins_for_Firefox">Des plugins pour les moteurs de recherche</a> qui permettent d'ajouter de nouveaux moteurs de recherche à la barre de recherche du navigateur</li>
 <li><a href="/fr/docs/Mozilla/Creating_a_spell_check_dictionary_add-on">Des dictionnaires utilisateur</a> qui permettent d'utiliser la vérification orthographique dans différentes langues</li>
 <li><a href="https://support.mozilla.org/kb/use-firefox-interface-other-languages-language-pack">Des packs de langues</a> qui permettent de traduire l'interface de Firefox dans plus de langues.</li>
</ul>

<hr />
<h2 id="Nous_contacter">Nous contacter</h2>

<p>Vous pouvez utiliser les liens qui suivent pour demander de l'aide, être tenu-e informé-e des actualités concernant les modules complémentaires et nous fournir vos retours.</p>

<h3 id="Forum">Forum</h3>

<p><a href="https://discourse.mozilla-community.org/c/add-ons">Le forum Discourse dédié aux modules complémentaires</a> est un lieu où discuter du développement de modules complémentaires et où demander de l'aide.</p>

<h3 id="Liste_de_diffusion">Liste de diffusion</h3>

<p>La liste de diffusion <strong>dev-addons</strong> (anglophone) est utilisée afin de discuter du développement des modules complémentaires et de leur environnement. Les thèmes abordés incluent le format WebExtensions et AMO (<a href="https://addons.mozilla.org">https://addons.mozilla.org</a>) :</p>

<ul>
 <li><a href="https://mail.mozilla.org/pipermail/dev-addons/">Informations sur la liste dev-addons</a></li>
 <li><a href="https://mail.mozilla.org/pipermail/dev-addons/">Archives de la liste dev-addons</a></li>
</ul>

<h3 id="IRC">IRC</h3>

<p>Si vous utilisez IRC, vous pouvez utiliser ces canaux (anglophones) :</p>

<ul>
 <li><a href="irc://irc.mozilla.org/addons">#addons</a> (discussions sur l'écosystème des modules complémentaires)</li>
 <li><a href="irc://irc.mozilla.org/extdev">#extdev</a> (discussions sur le développement des modules complémentaires)</li>
 <li><a href="irc://irc.mozilla.org/webextensions">#webextensions</a> (discussion sur les modules de type WebExtensions)</li>
</ul>

