---
version: prototype1
revision_id: 1326637
locale: sv-SE
slug: Web/HTML
tags: "Vad är HTML" "Referenser" "HTML-handledning" "HTML-programmering"
title: HTML
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<div>{{HTMLSidebar}}</div>

<p class="summary"><span class="seoSummary"><strong>HTML</strong> (HyperText Markup Language) är webbens mest grundläggande byggsten.&nbsp;Det beskriver och definierar <em>innehållet</em>&nbsp;på en webbsida.&nbsp;Andra tekniker utöver HTML används vanligen för att beskriva en webbsidas utseende&nbsp;(<a href="/en-US/docs/Web/CSS">CSS</a>) eller&nbsp;funktionalitet (<a href="/en-US/docs/Web/JavaScript">JavaScript</a>).</span></p>

<p>"HyperText" refererar till länkar som binder samman&nbsp;webbsidor med varandra, antingen inom en enskild webbsajt eller mellan olika webbsajter. Länkar är en grundläggande aspekt av webben. Genom att ladda upp innehåll på internet och länka det till sidor som skapats av andra människor blir du en aktiv deltagare i World Wide Web.</p>

<p>HTML använder sig av "uppmärkning" vid&nbsp;annotering av text, bilder och annat innehåll&nbsp;för visning i en webbläsare.&nbsp;HTML märkspråk inkluderar speciella "element" såsom&nbsp;{{HTMLElement("head")}}, {{HTMLElement("title")}}, {{HTMLElement("body")}}, {{HTMLElement("header")}}, {{HTMLElement("footer")}}, {{HTMLElement("article")}}, {{HTMLElement("section")}}, {{HTMLElement("p")}}, {{HTMLElement("div")}}, {{HTMLElement("span")}}, {{HTMLElement("img")}}, och många andra.</p>

<p>Artiklarna nedan hjälper dig att lära dig mer om HTML.</p>

<section class="cleared" id="sect1">
<ul class="card-grid">
 <li><span>HTML-introduktion</span>

  <p>Om du är ny inom webbutveckling, se till att läsa vår artikel <a href="/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics">Grunderna i HTML</a>&nbsp;för att lära dig vad HTML är och hur du använder det.</p>
 </li>
 <li><span>HTML-handledning</span>
  <p>För artiklar&nbsp;om hur du använder HTML, handledning/tutorials och fullständiga exempel, så kan du utforska vår&nbsp;<a href="/en-US/docs/Learn/HTML">HTML Learning Area</a>.</p>
 </li>
 <li><span>HTML-referenser</span>
  <p>I vår omfattande <a href="/en-US/docs/Web/HTML/Reference">HTML-referenser</a>-sektion hittar du detaljerad information om alla element och attribut i HTML.</p>
 </li>
</ul>

<div class="row topicpage-table">
<div class="section">
<h2 class="Tools" id="Tools" name="Tools">Nybörjarhandledning</h2>

<p>Vår&nbsp;<a href="/en-US/docs/Learn/HTML">HTML Learning Area</a>&nbsp;innehåller ett flertal moduler som lär ut HTML från grunden&nbsp;— inga förkunskaper krävs.</p>

<dl>
 <dt><a href="/en-US/docs/Learn/HTML/Introduction_to_HTML">Introduktion till&nbsp;HTML</a></dt>
 <dd>Denna modul lägger grunden, och introducerar&nbsp;viktiga koncept och&nbsp;syntax, såsom att&nbsp;applicera HTML till&nbsp;text, skapa&nbsp;hyperlänkar och att använda&nbsp;HTML för att strukturera en webbsida.</dd>
 <dt><a href="/en-US/docs/Learn/HTML/Multimedia_and_embedding">Multimedia och inbäddning</a></dt>
 <dd>Denna modul utforskar hur du kan använda HTML för att inkludera multimedia i dina webbsidor, och även de olika sätt som bilder kan inkluderas, samt hur du bäddar in video, audio, och även kompletta hemsidor.</dd>
 <dt><a href="/en-US/docs/Learn/HTML/Tables">HTML-tabeller</a></dt>
 <dd>Att representera tabulär data på en webbsida på ett förståeligt och tillgängligt sätt kan vara en utmaning. Denna modul innefattar grundläggande tabell-uppmärkning, såväl som mer komplexa funktioner såsom tillämpning av tabellrubriker och sammanfattningar.</dd>
 <dt><a href="/en-US/docs/Learn/HTML/Forms">HTML-formulär</a></dt>
 <dd>Formulär&nbsp;är en väldigt viktig del av webben — de bidrar med mycket av den funktionaliteten som du behöver för att kunna interagera med webbsajter, t.ex. registrera&nbsp;och logga in, skicka feedback, köpa produkter och mycket mer.&nbsp;Med denna modul kan du komma igång med att skapa de delar av formulär som hör till klient-sidan.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Howto">Använda&nbsp;HTML för att lösa vanliga problem</a></dt>
 <dd>Erbjuder länkar till sektioner av innehåll som förklarar hur man använder HTML för att lösa mycket vanliga problem som uppstår när man skapar en webbsida: hantera titlar, lägga till bilder eller videos, betona innehåll, skapa ett enkelt formulär, etc.</dd>
</dl>

<h2 id="Avancerade_ämnen">Avancerade ämnen</h2>

<dl>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/CORS_enabled_image">CORS enabled image</a></dt>
 <dd class="landingPageList">The&nbsp;<code><a href="/en-US/docs/Web/HTML/Element/img#attr-crossorigin">crossorigin</a></code> attribute, in combination with an appropriate <a class="glossaryLink" href="/en-US/docs/Glossary/CORS">CORS</a> header, allows images defined by the {{HTMLElement("img")}} element to be loaded from foreign origins and used in a {{HTMLElement("canvas")}} element as if they were being loaded from the current origin.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/CORS_settings_attributes">CORS settings attributes</a></dt>
 <dd class="landingPageList">Some HTML elements that provide support for <a href="/en-US/docs/HTTP/Access_control_CORS">CORS</a>, such as {{HTMLElement("img")}} or {{HTMLElement("video")}}, have a <code>crossorigin</code> attribute (<code>crossOrigin</code> property), which lets you configure the CORS requests for the element's fetched data.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Focus_management_in_HTML">Focus management in HTML</a></dt>
 <dd class="landingPageList">The <code><a href="/en-US/docs/Web/API/Document/activeElement">activeElement</a></code> DOM attribute and the <code><a href="/en-US/docs/Web/API/Document/hasFocus">hasFocus()</a></code> DOM method help you track and control a user's interactions with elements on a web page.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Using_the_application_cache">Using the application cache</a></dt>
 <dd class="landingPageList">Application caching&nbsp;lets web-based applications run offline. You can use the <strong>Application Cache</strong> (<em>AppCache</em>) interface to specify resources that the browser should cache and make available to offline users. Applications that are cached load and work correctly even if users click the refresh button when they are offline.</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Preloading_content">Preloading content with rel="preload"</a></dt>
 <dd class="landingPageList">The <code>preload</code> value of the {{htmlelement("link")}} element's {{htmlattrxref("rel", "link")}} attribute allows you to write declarative fetch requests in your HTML {{htmlelement("head")}}, specifying resources that your pages will need very soon after loading, which you therefore want to start preloading early in the lifecycle of a page load, before the browser's main rendering machinery kicks in. This ensures that they are made available earlier and are less likely to block the page's first render, leading to performance improvements. This article provides a basic guide to how <code>preload</code> works.</dd>
</dl>
</div>

<div class="section">
<h2 class="Documentation" id="Referenser">Referenser</h2>

<dl>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Reference">HTML-referenser</a></dt>
 <dd class="landingPageList">HTML består av&nbsp;<strong>element</strong>, som vart och ett kan modifieras med ett visst&nbsp;antal&nbsp;<strong>attribut</strong>. HTML-dokument&nbsp;är sammanbundna med varandra med hjälp av <a href="/en-US/docs/Web/HTML/Link_types">länkar</a>.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Element">HTML-elementreferenser</a></dt>
 <dd class="landingPageList">Bläddra igenom en lista på alla <a class="glossaryLink" href="/en-US/docs/Glossary/HTML">HTML</a>-<a class="glossaryLink" href="/en-US/docs/Glossary/Element">element</a>.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Attributes">HTML-attributreferenser</a></dt>
 <dd class="landingPageList">Element&nbsp;i&nbsp;HTML har&nbsp;olika&nbsp;<strong>attribut</strong>. Dessa är kompletterande värden som konfigurerar elementen eller justerar deras beteenden på olika sätt.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Global_attributes">Globala attribut</a></dt>
 <dd class="landingPageList">Globala attribut&nbsp;kan specifieras för alla <a href="/en-US/docs/Web/HTML/Element">HTML element</a>, <em>även de som inte är specifierade i standarden</em>. Detta betyder att alla&nbsp;icke-standardelement ändå måste tillåta dessa attribut, även om de&nbsp;gör dokumentet icke-kompatibelt med HTML5.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Inline_elements">Inline-element</a>&nbsp;och&nbsp;<a href="/en-US/docs/Web/HTML/Block-level_elements">block-level-element</a></dt>
 <dd class="landingPageList">HTML-element är vanligtvis "textnivå"- ("inline") eller&nbsp;"blocknivå"-element ("block level"). Ett textnivåelement tar inte upp mer plats än vad som ryms mellan de taggar som definierar det. Ett blocknivåelement tar upp hela sitt föräldraelements (containers) yta, och skapar på så sätt ett "block".</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Link_types">Länktyper</a></dt>
 <dd class="landingPageList">I&nbsp;HTML kan flera länktyper användas för att etablera och definiera förhållandet mellan två dokument.&nbsp;Länkelement som&nbsp;länktyper kan användas på inkluderar <a href="/en-US/docs/Web/HTML/Element/a"><code>&lt;a&gt;</code></a>, <a href="/en-US/docs/Web/HTML/Element/area"><code>&lt;area&gt;</code></a>, och&nbsp;<a href="/en-US/docs/Web/HTML/Element/link"><code>&lt;link&gt;</code></a>.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Supported_media_formats">Mediaformat&nbsp;som stöds av HTML-audio- och videoelement</a></dt>
 <dd class="landingPageList">Elementen&nbsp;<a href="/en-US/docs/Web/HTML/Element/audio"><code>&lt;audio&gt;</code></a>&nbsp;och&nbsp;<a href="/en-US/docs/Web/HTML/Element/video"><code>&lt;video&gt;</code></a>&nbsp;låter dig spela upp ljud&nbsp;och video. Dessa element&nbsp;erbjuder ett webbläsarnativt alternativ till liknande funktioner i Adobe Flash och andra plug-ins.</dd>
 <dt class="landingPageList"><a href="/en-US/docs/Web/HTML/Kinds_of_HTML_content">Olika typer av HTML-innehåll</a>&nbsp;(Avancerat)</dt>
 <dd class="landingPageList">HTML består av flera typer av innehåll, som vart och ett är tillåtet att använda i viss kontext och förbjudet i andra. På samma sätt har alla dessa typer&nbsp;varsin&nbsp;uppsättning av andra innehållskategorier som de kan innehålla och element som kan eller inte&nbsp;kan användas i dem. Detta är en guide till dessa kategorier.</dd>
</dl>

<h2 class="landingPageList" id="Relaterade_ämnen">Relaterade&nbsp;ämnen</h2>

<dl>
 <dt><a href="/en-US/docs/Web/HTML/Applying_color">Applicera färg på&nbsp;HTML-element&nbsp;med CSS</a></dt>
 <dd>Denna artikel tar upp de flesta sätt som du kan använda CSS för att addera färg till HTML-innehåll. Den listar vilka delar av HTML-dokument som kan färgas och vilka CSS-egenskaper som används då. Den inkluderar exempel, länkar till palettbyggarverktyg, m.m.</dd>
</dl>
</div>
</div>
<span class="alllinks"><a href="/en-US/docs/tag/HTML">View All...</a></span>

<p>{{CommunityBox("Web layout", "dev-tech-layout", "mozilla.dev.tech.layout", "", "Stack Overflow|http://stackoverflow.com/questions/tagged/html|HTML topics|Visit Stack Overflow, a collaboratively built and maintained Q&amp;A site. See if you can find an answer; if not, you can ask your question there.")}}</p>
</section>

