---
version: prototype1
revision_id: 1322350
locale: ca
slug: Web/HTML
tags: "HTML" "HTML5" "Web" "HTML Lesson" "What is HTML" "Landing" "HTML Tutorials" "Hyper text" "Hypertext" "Reference" "HTML Programming" "l10n:priority"
title: HTML (HyperText Markup Language)
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<div>{{HTMLSidebar}}</div>

<p class="summary">HTML (llenguatge de marcatge hipertextual - HyperText Markup Language) és el bloc de construcció més bàsic de la web. Descriu i defineix el contingut d'una pàgina web. Altres tecnologies a més de HTML s'utilitzen generalment per descriure l'aparença/presentació (<a href="https://developer.mozilla.org/en-US/docs/Web/CSS">CSS</a>) o la funcionalitat (<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript">JavaScript</a>) d'una pàgina web.</p>

<p>"HyperText" fa referència als enllaços que connecten pàgines web entre si, ja sigui dins d'un únic lloc web o entre llocs web. Els enllaços són un aspecte fonamental de la web. En penjar contingut a Internet i enllaçar-lo a pàgines creades per altres persones, us convertiu en un participant actiu a la World Wide Web.</p>

<p>HTML utilitza "marcat" per anotar text, imatges i altres continguts per mostrar-ho en un navegador web. El marcat HTML inclou "elements" especials com {{HTMLElement("head")}}, {{HTMLElement("title")}}, {{HTMLElement("body")}}, {{HTMLElement("header")}}, {{HTMLElement("footer")}}, {{HTMLElement("article")}}, {{HTMLElement("section")}}, {{HTMLElement("p")}}, {{HTMLElement("div")}}, {{HTMLElement("span")}}, {{HTMLElement("img")}} i molts altres.</p>

<p>Els següents articles us ajudaran a aprendre més sobre HTML.</p>

<section class="cleared" id="sect1">
<ul class="card-grid">
 <li><span>Introducció a HTML</span>

  <p>Si sou nou en el desenvolupament web, assegureu-vos de llegir l'article <a href="/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics">HTML Bàsics</a> per aprendre què és HTML i com utilitzar-lo.</p>
 </li>
 <li><span>Tutorials HTML</span>
  <p>Per articles sobre com utilitzar HTML, així com tutorials i exemples complets, consulteu el nostre <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML">àrea d'aprenentatge HTML</a>.</p>
 </li>
 <li><span>Referència HTML</span>
  <p>A la nostra àmplia secció de <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Reference">referència HTML</a>, trobareu els detalls sobre cada element i atribut en HTML.</p>
 </li>
</ul>

<div class="row topicpage-table">
<div class="section">
<h2 class="Tools" id="Tools" name="Tools">Tutorials per principiants</h2>

<p>La nostra <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML">àrea d'aprenentatge HTML</a> ofereix múltiples mòduls que ensenyen HTML des del principi, sense necessitat d'un coneixement previ.</p>

<dl>
 <dt><a href="/en-US/docs/Learn/HTML/Introduction_to_HTML">Introducció a HTML</a></dt>
 <dd>Aquest mòdul estableix l'escenari, perquè us aneu acostumant a conceptes i sintaxis importants, com aplicar HTML al text, com crear hipervincles i com usar HTML per estructurar una pàgina web.</dd>
 <dt><a href="/en-US/docs/Learn/HTML/Multimedia_and_embedding">Multimèdia i incrustació</a></dt>
 <dd>Aquest mòdul explora com utilitzar HTML per incloure multimèdia a les vostres pàgines web, incloent les diferents maneres en què es poden incloure les imatges i com incrustar vídeo, àudio i fins i tot pàgines web senceres.</dd>
 <dt><a href="/en-US/docs/Learn/HTML/Tables">Taules HTML</a></dt>
 <dd>Representar dades tabulars en una pàgina web d'una manera comprensible i accessible pot ser un repte. Aquest mòdul inclou el marcat bàsic de la taula, juntament amb característiques més complexes, com ara la implementació de subtítols i resums.</dd>
 <dt><a href="/en-US/docs/Learn/HTML/Forms">Formularis HTML</a></dt>
 <dd>Els formularis són una part molt important de la Web: proporcionen gran part de la funcionalitat que necessiteu per interactuar amb els llocs web, p. ex. registrar i iniciar sessió, enviar comentaris, comprar productes i molt més. Aquest mòdul us permet començar a crear les parts del costat del client dels formularis.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Howto">Utilitzar HTML per resoldre problemes comuns</a></dt>
 <dd>Proporciona enllaços a seccions de contingut que expliquen com utilitzar HTML per resoldre problemes molt comuns a l'hora de crear una pàgina web: tractar els títols, afegir imatges o vídeos, fer èmfasi en el contingut, crear un formulari bàsic, etc.</dd>
</dl>

<h2 id="Temes_avançats">Temes avançats</h2>

<dl>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/CORS_enabled_image">Imatge CORS habilitada</a></dt>
 <dd class="landingPageList">L'atribut <code><a href="/en-US/docs/Web/HTML/Element/img#attr-crossorigin">crossorigin</a></code> en combinació amb un encapçalament <a class="glossaryLink" href="/en-US/docs/Glossary/CORS">CORS</a> adequat, permet que les imatges definides per l'element {{HTMLElement("img")}} es carreguin des d'origens estrangers i s'utilitzin en un element {{HTMLElement("canvas")}} com si s'estiguessin carregant des de l'origen actual.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/CORS_settings_attributes">Atributs de configuració de CORS</a></dt>
 <dd class="landingPageList">Alguns elements HTML que proporcionen suport per <a href="/en-US/docs/HTTP/Access_control_CORS">CORS</a>, com ara {{HTMLElement("img")}} o {{HTMLElement("video")}}, tenen un atribut <code>crossorigin</code> (propietat <code>crossOrigin</code>), que us permet configurar les sol·licituds CORS per les dades&nbsp; recuperades de l'element.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Focus_management_in_HTML">Gestió de focus en HTML</a></dt>
 <dd class="landingPageList">L'atribut DOM <code><a href="/en-US/docs/Web/API/Document/activeElement">activeElement</a></code> i el mètode DOM <code><a href="/en-US/docs/Web/API/Document/hasFocus">hasFocus()</a></code> ajudan a rastrejar i controlar les interaccions d'un usuari amb elements d'una pàgina web.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Using_the_application_cache">Ús de la memòria cau de l'aplicació</a></dt>
 <dd class="landingPageList">L'emmagatzematge en memòria cau d'aplicacions, permet que les aplicacions basades en web s'executin sense connexió. Podeu utilitzar la interfície <strong>Application Cache</strong> (<em>AppCache</em>) per especificar els recursos que el navegador hauria d'emmagatzemar en memòria cau i posar-la a disposició dels usuaris fora de línia. Les aplicacions que es carreguen a la memòria cau i funcionen correctament encara que els usuaris facin clic al botó d'actualització quan no estiguin connectats.</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Preloading_content">Precàrrega de contingut amb rel="preload"</a></dt>
 <dd class="landingPageList">El valor <code>preload</code> de l'atribut {{htmlattrxref("rel", "link")}} de l'element {{htmlelement("link")}} permet escriure sol·licituds de cerca declaratives en el seu {{htmlelement("head")}} HTML , especificant els recursos que les vostres pàgines necessitaran, ràpidament després de la càrrega, per la qual cosa necessita començar la precàrrega abans del cicle de vida d'una càrrega de pàgina, abans que la maquinària de representació principal, del navegador, entri en acció . Això garanteix que estiguin disponibles abans i sigui menys probable que bloquegi el primer renderitzat de la pàgina, la qual cosa comporta millores en el rendiment. Aquest article proporciona una guia bàsica sobre com funciona el <code>preload</code>.</dd>
</dl>
</div>

<div class="section">
<h2 class="Documentation" id="Referències">Referències</h2>

<dl>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Reference">Referència HTML</a></dt>
 <dd class="landingPageList">HTML consisteix en <strong>elements</strong>, cadascun dels quals pot ser modificat per un cert nombre d'<strong>atributs</strong>. Els documents HTML es connecten entre si per <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Link_types">enllaços</a>.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Element">Referència de l'element HTML</a></dt>
 <dd class="landingPageList">Navegareu per una llista de tots els <a class="glossaryLink" href="/en-US/docs/Glossary/Element">elements HTML</a>.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Attributes">Referència de l'atribut HTML</a></dt>
 <dd class="landingPageList">Els elements en HTML tenen <strong>atributs</strong>. Són valors addicionals que configuren els elements o ajusten el seu comportament de diverses maneres.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Global_attributes">Atributs Globals</a></dt>
 <dd class="landingPageList">Els atributs globals es poden especificar en tots els <a href="/en-US/docs/Web/HTML/Element">elements HTML</a>, <em>fins i tot aquells no especificats en l'estàndard</em>. Això significa que qualsevol element no estàndard ha de permetre aquests atributs, encara que aquests elements facin que el document HTML5 no sigui compatible.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Inline_elements">Elements en línia</a> i <a href="/en-US/docs/Web/HTML/Block-level_elements">elements a nivell de bloc</a></dt>
 <dd class="landingPageList">Els elements HTML solen ser elements "en línia" o "a nivell de bloc". Un element inline ocupa només l'espai delimitat per les etiquetes que el defineixen. Un element a nivell de bloc ocupa tot l'espai del seu element pare (contenidor), creant així un "bloc".</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Link_types">Tipus d'enllaços</a></dt>
 <dd class="landingPageList">En HTML, es poden utilitzar diversos tipus d'enllaços per establir i definir la relació entre dos documents. Els elements d'enllaç que els tipus es poden configurar, inclouen <a href="/en-US/docs/Web/HTML/Element/a"><code>&lt;a&gt;</code></a>, <a href="/en-US/docs/Web/HTML/Element/area"><code>&lt;area&gt;</code></a> i <a href="/en-US/docs/Web/HTML/Element/link"><code>&lt;link&gt;</code></a>.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Supported_media_formats">Formats de medis compatibles amb elements d'àudio u vídeo HTML</a></dt>
 <dd class="landingPageList">Els elements <a href="/en-US/docs/Web/HTML/Element/audio"><code>&lt;audio&gt;</code></a> i <a href="/en-US/docs/Web/HTML/Element/video"><code>&lt;video&gt;</code></a> permeten reproduir medis d'àudio i de vídeo. Aquests elements proporcionen una alternativa nativa del navegador a funcions similars que es troben en Adobe Flash i altres connectors (plug-ins).</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Kinds_of_HTML_content">Tipus de contingut HTML</a> (Avançat)</dt>
 <dd class="landingPageList">HTML es compon de diversos tipus de contingut, cadascun dels quals es permet utilitzar en determinats contextos i està prohibit en uns altres. De la mateixa manera, cadascun d'ells té un conjunt d'altres categories de contingut que poden contenir i elements que poden o no ser utilitzats en ells. Aquesta és una guia per a aquestes categories.</dd>
</dl>

<h2 class="landingPageList" id="Temes_relacionats">Temes relacionats</h2>

<dl>
 <dt><a href="/en-US/docs/Web/HTML/Applying_color">Aplicació de colors a elements HTML usant CSS</a></dt>
 <dd>Aquest article abasta la majoria de les maneres d'utilitzar CSS per afegir color a contingut HTML, enumerant quines parts dels documents HTML es poden acolorir i quines propietats CSS s'utilitzaran en fer-ho. Inclou exemples, enllaços a eines de construcció de paleta, i molt més.</dd>
</dl>
</div>
</div>
<span class="alllinks"><a href="/en-US/docs/tag/HTML">Veure Tot...</a></span>

<p>{{CommunityBox("Web layout", "dev-tech-layout", "mozilla.dev.tech.layout", "", "Stack Overflow|http://stackoverflow.com/questions/tagged/html|HTML topics|Visit Stack Overflow, a collaboratively built and maintained Q&amp;A site. See if you can find an answer; if not, you can ask your question there.")}}</p>
</section>

