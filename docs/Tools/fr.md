---
version: prototype1
revision_id: 1228895
locale: fr
slug: Outils
tags: "Guide" "Outils" "Firefox" "Développement Web" "Développement Web:Outils"
title: Outils de développement
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>Examinez, modifiez, et déboguez du HTML, du CSS, et du JavaScript sur ordinateur, et sur mobile. Pour avoir la dernière version des outils de développement, téléchargez <a href="https://www.mozilla.org/fr/firefox/developer/">Firefox Developer Edition</a>.</p>

<p>{{ SauceLabsPromo("a") }}</p>

<h2 id="Outils_principaux">Outils principaux</h2>

<hr />
<div class="column-container">
<div class="column-half">
<h3 id="Inspecteur">Inspecteur</h3>

<p><a href="/fr/docs/Tools/Page_Inspector"><img alt="" src="https://mdn.mozillademos.org/files/14532/inspector.png" style="display:block; height:257px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>Permet de voir et modifier une page en HTML et en CSS. Permet de visualiser différents aspects de la page y compris les animations, l'agencement de la grille.</p>
</div>

<div class="column-half">
<h3 id="Console_Web">Console Web</h3>

<p><a href="/fr/docs/Tools/Web_Console"><img alt="" src="https://mdn.mozillademos.org/files/14528/console.png" style="display:block; height:257px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>Affiche les messages émis par la page web. Permet également d'interagir avec la page via JavaScript.</p>
</div>
</div>

<hr />
<div class="column-container">
<div class="column-half">
<h3 id="Débogueur_Javascript">Débogueur Javascript</h3>

<p><a href="/fr/docs/Tools/Debugger"><img alt="" src="https://mdn.mozillademos.org/files/14542/debugger.png" style="display:block; height:1026px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>Permet de parcourir, stopper, examiner et modifier le code JavaScript s’exécutant dans une page</p>
</div>

<div class="column-half">
<h3 id="Réseau">Réseau</h3>

<p><a href="/fr/docs/Tools/Network_Monitor"><img alt="" src="https://mdn.mozillademos.org/files/14534/network-monitor.png" style="display:block; height:257px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>Permet d'inspecter les requêtes réseau lors du chargement de la page.</p>
</div>
</div>

<hr />
<div class="column-container">
<div class="column-half">
<h3 id="Performances">Performances</h3>

<p><a href="/fr/docs/Tools/Performance"><img alt="" src="https://mdn.mozillademos.org/files/14536/performance.png" style="display:block; height:1026px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>Permet d'analyser les performances de la réactivité globale, du JavaScript et, de l'agencement des sites.</p>
</div>

<div class="column-half">
<h3 id="Vue_Adaptative">Vue Adaptative</h3>

<p><a href="/fr/docs/Tools/Responsive_Design_Mode"><img alt="" src="https://mdn.mozillademos.org/files/14538/rdm.png" style="display:block; height:1542px; margin-left:auto; margin-right:auto; width:425px" /></a></p>

<p>Permet de voir comment un site web ou une application se comporte sur différents types d'appareils et de connexions.</p>
</div>
</div>

<hr />
<h2 id="Outils_supplémentaires">Outils supplémentaires</h2>

<p>Ces outils sont également inclus dans Firefox. Cependant il est possible qu'ils soient utilisés moins régulièrement.</p>

<div class="twocolumns">
<dl>
 <dt><a href="/fr/docs/Tools/Memory">Mémoire</a></dt>
 <dd>Déterminer quels objets prennent de la place en mémoire.</dd>
 <dt><a href="/fr/docs/Tools/Storage_Inspector">Inspecteur de Stockage</a></dt>
 <dd>Inspecter les cookies, le stockage local, l'indexedDB, et le stockage de session présent dans une page.</dd>
 <dt><a href="/fr/docs/Tools/DOM_Property_Viewer">DOM Property Viewer</a></dt>
 <dd>Inspecter les propriétés DOM d'une page (fonctions, etc...)</dd>
 <dt><a href="/fr/docs/Tools/GCLI">Barre de développement</a></dt>
 <dd>Une interface en ligne de commande pour les outils de développement.</dd>
 <dt><a href="/fr/docs/Tools/Eyedropper">Pipette</a></dt>
 <dd>Sélectionner une couleur de la page.</dd>
 <dt><a href="/fr/docs/Tools/Scratchpad">Ardoise JavaScript</a></dt>
 <dd>Un éditeur de texte intégré à Firefox qui permet d'écrire et d'exécuter du JavaScript..</dd>
 <dt><a href="/fr/docs/Outils/Style_Editor">Éditeur de Style</a></dt>
 <dd>Voir et modifier les styles CSS de la page affichée.</dd>
 <dt><a href="/fr/docs/Outils/Shader_Editor">Éditeur de Shaders</a></dt>
 <dd>Voir et éditer les <em>vertex shaders</em> et les <em>fragment shaders</em> utilisés par <a href="/fr/docs/WebGL">WebGL</a>.</dd>
 <dt><a href="/fr/docs/Outils/Web_Audio_Editor">Éditeur Web Audio</a></dt>
 <dd>Examiner les nœuds audio dans un contexte audio, et modifier leurs paramètres.</dd>
 <dt><a href="/fr/docs/Tools/Screenshot_tool">Capture d'écran</a></dt>
 <dd>Prendre une capture d'écran de la page entière ou d'un seul élément</dd>
</dl>
</div>

<hr />
<h2 id="Connecter_les_outils_de_développement">Connecter les outils de développement</h2>

<p>Les outils de développement ciblent la page actuelle par défaut. Il est cependant possible d'attacher ces outils à une variété de cibles différentes. Cela inclut des cibles dans le navigateur, dans d'autres navigateurs et même dans d'autres appareils.</p>

<div class="twocolumns">
<dl>
 <dt><a href="/fr/docs/Tools/about:debugging">about:debugging</a></dt>
 <dd>Un tableau de bord pour déboguer les modules complémentaires et les workers</dd>
 <dt><a href="/fr/docs/Tools/Remote_Debugging/Debugging_Firefox_for_Android_over_Wifi">Connexion à Firefox pour Android</a></dt>
 <dd>Connecter les outils de développement à une instance de Firefox s'exécutant sur un appareil Android.</dd>
 <dt><a href="/fr/docs/Tools/Working_with_iframes">Travailler avec des iframes</a></dt>
 <dd>Comment travailler avec un iframe particulier.</dd>
 <dt><a href="/fr/docs/Tools/Valence">Valence</a></dt>
 <dd>Connecter les outils de développement à Chrome pour Android et Safari pour IOS.</dd>
</dl>
</div>

<hr />
<h2 id="Deboguer_le_navigateur">Deboguer le navigateur</h2>

<p>Par défaut, les outils de développement sont attachés à une page web. Il est cependant possible de les connecter au navigateur en lui même. C'est utile lors de développements portant sur le navigateur ou sur un module complémentaire.</p>

<div class="twocolumns">
<dl>
 <dt><a href="/fr/docs/Tools/Browser_Console">Console du navigateur</a></dt>
 <dd>Lire les messages du navigateur lui-même et des modules. Exécuter du JavaScript dans le contexte de la fenêtre du navigateur.</dd>
 <dt><a href="/fr/docs/Outils/Browser_Toolbox">Boîte à outils du navigateur</a></dt>
 <dd>Attache les outils de développement au navigateur lui-même.</dd>
</dl>
</div>

<hr />
<h2 id="Étendre_les_outils_de_développement">Étendre les outils de développement</h2>

<p>Ces outils sont pensés pour être extensibles. Les modules complémentaires de Firefox peuvent accéder aux outils de développement ainsi qu'aux composants qu'ils utilisent. Avec le protocole de débogage distant, il est possible d'implémenter son propre débogage de clients et serveur. Cela peut permettre de déboguer des sites web en utilisant des outils personnels ou bien de déboguer des cibles différentes en utilisant les outils de Firefox.</p>

<div class="twocolumns">
<dl>
 <dt><a href="/fr/docs/Tools/Example_add-ons">Examples de modules complémentaires d'outils de développement.</a></dt>
 <dd>Ces exemples servent à faciliter la compréhension sur comment implémenter un module complémentaire d'outils de développement.</dd>
 <dt><a href="/fr/docs/Tools/Adding_a_panel_to_the_toolbox">Ajouter un nouveau panneau aux outils de développement</a></dt>
 <dd>Écrire un module complémentaire qui ajoute un nouveau panneau à la boite à outils.</dd>
 <dt><a class="external external-icon" href="https://wiki.mozilla.org/Remote_Debugging_Protocol" title="Remote Debugging Protocol">Protocole de débogage à distance</a></dt>
 <dd>Le protocole utilisé pour connecter les outils de développement de Firefox à une cible à déboguer, telle qu’une instance de Firefox ou un terminal Firefox OS.</dd>
 <dt><a href="/fr/docs/Tools/Editor" title="Source Editor">Éditeur de source</a></dt>
 <dd>Un éditeur de code intégré à Firefox pouvant être embarqué dans votre module.</dd>
 <dt><a href="/fr/docs/Tools/Debugger-API">L’interface <code>Debugger</code></a></dt>
 <dd>Une API permettant à du code JavaScript d’observer l’exécution d’un autre code JavaScript. Les outils de développement de Firefox utilisent cette API pour implémenter le débogueur JavaScript.</dd>
 <dt><a href="/fr/docs/Tools/Web_Console/Custom_output">Sortie personnalisée de la Console Web</a></dt>
 <dd>Comment étendre et personnaliser la sortie de la <a href="/fr/docs/Tools/Web_Console">Console Web</a> et de la <a href="/fr/docs/Tools/Browser_Console">Console Javascript</a>.</dd>
</dl>
</div>

<hr />
<h2 id="Contribuer">Contribuer</h2>

<p>Si vous voulez aider à améliorer les outils de développement, voici les ressources qui vous mettront le pied à l'étrier :</p>

<div class="twocolumns">
<dl>
 <dt><a href="https://wiki.mozilla.org/DevTools/GetInvolved">Get Involved</a></dt>
 <dd>La page du wiki de Mozilla expliquant comment s'impliquer.</dd>
 <dt><a href="http://firefox-dev.tools/">firefox-dev.tools</a></dt>
 <dd>Un outil pour aider à trouver des bugs sur lesquels travailler.</dd>
</dl>
</div>

<hr />
<div>{{CommunityBox("Developer tools", "dev-developer-tools", "mozilla.dev.developer-tools", "devtools", "Team info|https://wiki.mozilla.org/DevTools|Dev tools wiki|Designs and plans for the dev tools||Blog|https://hacks.mozilla.org/|Hacks blog|Hacks blog", "FirefoxDevTools", "firefox-developer-tools")}}</div>

<h2 id="Subnav">Subnav</h2>

<ol>
 <li><a href="#">Outils principaux</a>

  <ol>
   <li><a href="/fr/docs/Tools/Page_Inspector">Inspecteur</a></li>
   <li><a href="/fr/docs/Outils/Web_Console">Console web</a></li>
   <li><a href="/fr/docs/Outils/Debugger">Débogueur JavaScript</a></li>
   <li><a href="/fr/docs/Tools/Network_Monitor">Moniteur réseau</a></li>
   <li><a href="/fr/docs/Tools/Performance">Performances</a></li>
   <li><a href="/fr/docs/Outils/Vue_adaptative">Vue adaptative</a></li>
   <li><a href="/fr/docs/Tools/Tips">Astuces</a></li>
  </ol>
 </li>
 <li><a href="#">More Tools</a>
  <ol>
   <li><a href="/fr/docs/Tools/Memory">Mémoire</a></li>
   <li><a href="/fr/docs/Tools/Storage_Inspector">Inspecteur de stockage</a></li>
   <li><a href="/fr/docs/Tools/DOM_Property_Viewer">DOM Property Viewer</a></li>
   <li><a href="/fr/docs/Tools/GCLI">Barre de développement</a></li>
   <li><a href="/fr/docs/Tools/Eyedropper">Pipette</a></li>
   <li><a href="/fr/docs/Tools/Taking_screenshots">Capture d'écran</a></li>
   <li><a href="/fr/docs/Tools/Scratchpad">Ardoise JavaScript</a></li>
   <li><a href="/fr/docs/Tools/Style_Editor">Éditeur de style</a></li>
   <li><a href="/fr/docs/Tools/Shader_Editor">Éditeur de shader</a></li>
   <li><a href="/fr/docs/Tools/Web_Audio_Editor">Éditeur Web Audio</a></li>
  </ol>
 </li>
 <li><a href="#">Connecting the devtools</a>
  <ol>
   <li><a href="/fr/docs/Tools/about:debugging">about:debugging</a></li>
   <li><a href="/fr/docs/Tools/Remote_Debugging/Debugging_Firefox_for_Android_over_Wifi">Connexion à Firefox pour Android</a></li>
   <li><a href="/fr/docs/Tools/Working_with_iframes">Connexion aux iframes</a></li>
   <li><a href="/fr/docs/Tools/Valence">Connexion à d'autres navigateurs</a></li>
  </ol>
 </li>
 <li><a href="#">Debugging the browser</a>
  <ol>
   <li><a href="/fr/docs/Tools/Browser_Console">Console du navigateur</a></li>
   <li><a href="/fr/docs/Tools/Browser_Toolbox">Boite à outils du navigateur</a></li>
  </ol>
 </li>
 <li><a href="#">xtending the devtools</a>
  <ol>
   <li><a href="/fr/docs/Tools/Adding_a_panel_to_the_toolbox">Ajout d'un panneau à la boîte à outils</a></li>
   <li><a href="/fr/docs/Tools/Example_add-ons">Exemples d'extensions aux outils de développement</a></li>
   <li><a href="https://wiki.mozilla.org/Remote_Debugging_Protocol">Protocole de déboguage à distance</a></li>
   <li><a href="https://wiki.mozilla.org/Remote_Debugging_Protocol_Stream_Transport">Stream Transport</a></li>
   <li><a href="/fr/docs/Tools/Editor">Éditeur de source</a></li>
   <li><a href="/fr/docs/Tools/Debugger-API">L’interface <code>Debugger</code></a></li>
   <li><a href="/fr/docs/Tools/Web_Console/Custom_output">Sortie personnalisée dans la console web</a></li>
  </ol>
 </li>
 <li><a href="/fr/docs/Tools/Settings">Paramètres</a></li>
 <li><a href="/fr/docs/Tools/Release_notes">Notes de version</a></li>
</ol>

