---
version: prototype1
revision_id: 1142193
locale: fr
slug: HTTP
tags: "HTTP" "Web" "TopicStub" "Référence(2)"
title: HTTP
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{ HTTPSidebar }}</div>

<p class="summary"><strong><dfn>Hypertext Transfer Protocol (HTTP)</dfn></strong> est un protocole de&nbsp; <a class="external" href="https://fr.wikipedia.org/wiki/Couche_application">la couche application</a> servant à transmettre des documents hypermedia, comme HTML. Il a été conçu pour communiquer entre les navigateurs web et les serveurs web, bien qu'il puisse être utilisé à d'autres fins. Il suit le modèle classique <a class="external" href="https://fr.wikipedia.org/wiki/Client-serveur">client-serveur</a>, avec un client qui ouvre une <strong>connexion</strong>, faire une requête et attends jusqu'à recevoir une réponse. C'est aussi un <a class="external" href="https://fr.wikipedia.org/wiki/Serveur_sans_%C3%A9tat">protocole sans état</a>, ce qui signifie que le serveur ne converse aucune données (état) entre deux requêtes. Bien que généralement basé sur une couche TCP/IP, il peut aussi être utilisé sur toute <a class="external" href="https://fr.wikipedia.org/wiki/Couche_transport">couche de transport</a> fiable,qui est un protocole qui ne perd pas de messages silencieusement.</p>

<div class="column-container">
<div class="column-half">
<h2 id="Tutoriels">Tutoriels</h2>

<p>Apprenez comment utiliser HTTP avec des guides et des tutoriels.</p>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Overview">Aperçu du protocole&nbsp;HTTP</a></dt>
 <dd>Présentation des fonctionnalités basiques du protocole client-serveur : <span id="result_box" lang="fr"><span>ce qu'il peut faire</span> <span>et pour quels </span><span>utilisations il est prévue.</span></span></dd>
 <dt><a href="/en-US/docs/Web/HTTP/Basics_of_HTTP/Evolution_of_HTTP">Evolution du protocole HTTP</a></dt>
 <dd>Description&nbsp;rapide des changements entre HTTP dans ses premières versions et le moderne HTTP/2.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Messages">Les différents messages HTTP</a></dt>
 <dd>Description du type et de la structure des différentes sortes de messages de HTTP/1.x et HTTP/2.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Session">Démonstration de session HTTP</a></dt>
 <dd>Démonstration et explication du déroulement classique d'une session HTTP.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Connection_management_in_HTTP_1.x">Gestion des connexions&nbsp;HTTP/1.x</a></dt>
 <dd>Description des forces et faiblesse des trois modèles de management de connexion disponible dans&nbsp; HTTP/1.x.</dd>
 <dt><a href="/en-US/docs/Mozilla/HTTP_cache">Le cache HTTP</a></dt>
 <dd>Le cache est l'un des outils majeurs pour de bonnes performances sur les sites Web. Cet article présente les différents type de cache et comment utiliser les entêtes HTTP pour configurer et utiliser le cache.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Cookies">Les cookies et HTTP</a></dt>
 <dd>La façon donc les cookies fonctionnent sont définie par la&nbsp; <a class="external" href="http://tools.ietf.org/html/rfc6265">RFC 6265</a>. Lors de la réception d'une requête HTTP, un serveur peut envoyer un entête <code>Set-Cookie</code> avec la réponse. En suite le client renvoie la valeur du cookie, dans la forme d'un en-tête HTTP &nbsp;<code>Cookie,</code> avec chaque requête vers le même serveur.&nbsp; Un délai d'expiration peut être spécifié. Un coookie peut aussi être restreint à un domaine spécifique et un chemin (path).</dd>
 <dt><a href="/fr/docs/HTTP/Access_control_CORS">Contrôle d'accès HTTP (CORS)</a></dt>
 <dd><strong>Les requêtes HTTP de type Cross-site</strong> sont des requêtes HTTP pour des ressources depuis un <strong>domaine différent</strong> que&nbsp;<span id="result_box" lang="fr"><span>le domaine</span> <span>de la ressource</span> <span>qui fait la demande</span><span>.</span></span> Par exemple, une ressources chargée depuis un domaine A (<code>http://domaina.example/</code>), comme une page HTML, fait une requête pour une ressource sur un domaine B (http://domainb.foo/), comme une image, en utilisant la balise <code>img</code> (<code>http://domainb.foo/image.jpg</code>). Ceci est très courant sur le web de nos jours — les pages chargent de nombreuses ressources en utilsant les requêtes cross-site, notamment des feuilles de style CSS, des images, des scripts et d'autres ressources.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Controlling_DNS_prefetching">Pré-chargement DNS (prefetching</a>)</dt>
 <dd>Firefox et la majorité des autres naviateurs moderne utilisent le <strong>DNS prefetching</strong>. Cela signifie que les navigateurs réalisent de façon pro-active la résolution de nom de domaine sur un lien que l'utilisateur pourrait choisir de suivre et sur les références des ressouces comme les images, CSS et JavaScript. Ce pré-chargement est réalisé en arrière-plan ainsi, la recherche DNS est déjà résolu au moment où cette élément est demandé. Cela réduit la latence lorsque, par exemple l'utilisateur clique sur un lien.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Références">Références</h2>

<p>Naviguez dans la documentation détaillée de HTTP.</p>

<dl>
 <dt><a href="/fr/docs/HTTP/Headers">En-tête HTTP</a></dt>
 <dd>Les messages d'en-tête HTTP sont utilisés pour décrire précisement la ressource&nbsp;ou le comportement du client ou du serveur. Un en-tête propriétaire sur mesure peut être ajouté en utilsant le préfix 'X-' ; d'autres sont disponible dans le <a class="external" href="http://www.iana.org/assignments/message-headers/perm-headers.html">registe de l'IANA</a>, dont le contenu original a été défini dans la <a class="external" href="http://tools.ietf.org/html/rfc4229">RFC 4229</a>. L'IANA maintient aussi un <a class="external" href="http://www.iana.org/assignments/message-headers/prov-headers.html">registre des nouveaux messages d'en-tête HTTP</a>.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Methods">Les méthodes de requête HTTP</a></dt>
 <dd>Différentes opérations peuvent être fait avec HTTP : {{HTTPMethod("GET")}}, {{HTTPMethod("POST")}}, mais aussi moins couramment des requêtes comme&nbsp; {{HTTPMethod("OPTIONS")}}, {{HTTPMethod("DELETE")}} ou {{HTTPMethod("TRACE")}}.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Response_codes">Les codes de réponse HTTP</a></dt>
 <dd>Les codes de réponse&nbsp;HTTP indiquent si une requête HTTP a été <span class="short_text" id="result_box" lang="fr"><span>complétée&nbsp;avec succès. Les réponses sont regroupées en cinq classes : les réponses informationnelles, les réponses de succès, les redirections, les erreurs client et les erreurs serveur</span></span>.</dd>
</dl>

<h2 id="Outils_ressources">Outils &amp; ressources</h2>

<p>Outils utiles pour utiliser et debbugger vos connextions HTTP.</p>

<dl>
 <dt><a href="/en-US/docs/Tools">Firefox Developer Tools</a></dt>
 <dd><a href="/en-US/docs/Tools/Network_Monitor">Network monitor</a></dd>
 <dt><a href="https://redbot.org/">RedBot</a></dt>
 <dd>Un outil pour vérifier vos en-têtes relatifs aux caches</dd>
</dl>
</div>
</div>

