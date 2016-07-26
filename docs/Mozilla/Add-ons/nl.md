---
version: prototype1
revision_id: 1091307
locale: nl
slug: Mozilla/Add-ons
tags: "Add-ons" "Landing" "Mozilla" "Extension" "Extensions"
title: Add-ons
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<p><span class="seoSummary">Via add-ons kunnen ontwikkelaars de functionaliteit van Firefox uitbreiden en aanpasssen.</span> Add-ons worden geschreven door gebruikmaking van standaard webtechnologieën – JavaScript, HTML en CSS – plus enkele toepassingsspecifieke JavaScript-API’s. Naast andere dingen kan een add-on het volgende doen:</p>

<ul>
 <li>De vormgeving of inhoud van bepaalde websites wijzigen</li>
 <li>De gebruikersinterface van Firefox aanpassen</li>
 <li>Nieuwe functies aan Firefox toevoegen</li>
</ul>

<h2 id="Developing_add-ons">Add-ons ontwikkelen</h2>

<p>Momenteel bestaan er enkele toolsets voor het ontwikkelen van Firefox-add-ons, maar <a href="/Add-ons/WebExtensions">WebExtensions</a> zullen eind 2017 de standaard worden. Van de rest wordt verwacht dat ze rond dezelfde tijdsperiode zijn <a href="/Add-ons/Overlay_Extensions">afgeschaft</a>.</p>

<p>Hier vindt u informatie over beschikbare opties voor het ontwikkelen van add-ons, zodat u kunt beslissen wat op dit moment en in de toekomst het beste voor u is.</p>

<h3 id="Create_a_New_Add-on">Een nieuwe add-on maken</h3>

<p>Als u een nieuwe add-on schrijft, wordt aanbevolen een van de volgende methoden te kiezen. Totdat de overgang naar WebExtensions is voltooid, zijn er voor- en nadelen bij elke methode. Lees verder wat de opties inhouden om te beslissen wat het beste voor u werkt.</p>

<ul class="card-grid">
 <li style="position: relative; max-width: 400px;">
  <div style="margin-bottom: 70px;">
  <h4 id="WebExtensions"><a href="/Add-ons/WebExtensions">WebExtensions</a></h4>

  <p>WebExtensions zijn de toekomst van add-ons voor Firefox. Als u de WebExtensions-API kunt gebruiken, is dit de beste keuze. U kunt WebExtensions nu meteen ontwikkelen en publiceren, maar ze verkeren nog in een vroeg stadium.<br />
   <br />
   De meeste WebExtension-API’s zijn ook beschikbaar in <a href="/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">Firefox voor Android</a>.</p>

  <p>We zijn bezig met de voorbereiding van een eerste volledige versie voor <a href="https://wiki.mozilla.org/RapidRelease/Calendar">Firefox 48</a>.</p>
  </div>
  <a class="card-grid-button" href="/Add-ons/WebExtensions">Meer info</a></li>
 <li style="position: relative; max-width: 400px;">
  <div style="margin-bottom: 70px;">
  <h4 id="Add-on_SDK"><a href="/Add-ons/SDK">Add-on-SDK</a></h4>

  <p>De Add-on-SDK biedt API’s voor het ontwikkelen van add-ons voor Firefox, en een hulpmiddel voor het ontwikkelen, testen en verpakken ervan.</p>

  <p>U kunt ook <a href="/Add-ons/SDK/Tutorials/Mobile_development">Add-on-SDK-extensies in Firefox voor Android</a> uitvoeren.</p>

  <p>Het gebruik van alleen <a href="/Add-ons/SDK/High-Level_APIs">‘high-level-API’s’</a> wordt aangemoedigd, omdat dit gaandeweg makkelijker is om naar WebExtensions te migreren.</p>
  </div>
  <a class="card-grid-button" href="/Add-ons/SDK">Meer info</a></li>
</ul>

<h3 id="Migrate_an_Existing_Add-on">Een bestaande add-on migreren</h3>

<p>Er zijn in het komende jaar wijzigingen aan Firefox in aantocht die het browsen betrouwbaarder maken voor gebruikers, en het maken van add-ons makkelijker voor ontwikkelaars. Mogelijk dient uw add-on te worden bijgewerkt om compatibiliteit te behouden, maar als dit eenmaal is gebeurd en de vertaling is voltooid, is uw add-on meer compatibel, veiliger en toekomstbestendiger dan ooit.</p>

<p>We hebben <a href="https://wiki.mozilla.org/Add-ons/developer/communication">hulpbronnen, migratiepaden, kantoortijden en meer</a> aangemaakt om te verzekeren dat u de nodige ondersteuning hebt om de overgang te maken.</p>

<p>Gebruik om te beginnen de <a href="https://compatibility-lookup.services.mozilla.com/">add-on-compatibiliteitscontrole</a> om te zien of dit op uw add-on van toepassing is.</p>

<h2 id="Publishing_add-ons">Add-ons publiceren</h2>

<p><a href="https://addons.mozilla.org">Addons.mozilla.org</a>, doorgaans bekend als ‘AMO’, is Mozilla’s officiële website voor ontwikkelaars om add-ons te vermelden, en voor gebruikers om deze te vinden. Door uw add-on naar AMO te uploaden, kunt u deelnemen aan onze gemeenschap van gebruikers en makers, en een publiek vinden voor uw add-on.</p>

<p>U bent niet verplicht om uw add-on op AMO te vermelden, maar vanaf Firefox 40 moet uw code door Mozilla zijn ondertekend, anders kunnen gebruikers deze niet installeren.</p>

<p>Voor een overzicht van het proces van het publiceren van uw add-on, zie <a href="https://developer.mozilla.org/Add-ons/Distribution">Uw add-ons ondertekenen en distribueren</a>.</p>

<h2 id="Other_types_of_add-ons">Andere typen add-ons</h2>

<p>Doorgaans refereren mensen aan extensies als ze over add-ons spreken, maar er zijn enkele andere typen add-ons waarmee gebruikers Firefox kunnen aanpassen. Deze add-ons omvatten:</p>

<ul>
 <li><a href="https://developer.mozilla.org/Add-ons/Themes/Background">Lichtgewicht thema’s</a> zijn een eenvoudige manier om beperkte aanpassing van Firefox te bieden.</li>
 <li><a href="/Add-ons/Firefox_for_Android">Add-ons voor Mobiel</a> zijn add-ons voor Firefox voor Android. Houd er echter rekening mee dat we een deel van de onderliggende technologie in deze API’s willen afschaffen. In de toekomst zullen WebExtensions volledig compatibel zijn in Firefox voor Android.</li>
 <li><a href="/nl/docs/Creating_OpenSearch_plugins_for_Firefox">Zoekmachineplug-ins</a> voegen nieuwe zoekmachines toe aan de zoekbalk van de browser.</li>
 <li><a href="/docs/Mozilla/Creating_a_spell_check_dictionary_add-on">Gebruikerswoordenlijsten</a> zijn add-ons waarmee u in verschillende talen spelling kunt controleren.</li>
 <li><a href="https://support.mozilla.org/kb/use-firefox-interface-other-languages-language-pack">Taalpakketten</a> zijn add-ons waarmee u meerdere beschikbare talen voor de gebruikersinterface van Firefox kunt hebben.</li>
</ul>

<hr />
<h2 id="Contact_us">Contact</h2>

<p>U kunt de onderstaande koppelingen gebruiken om hulp te verkrijgen, up-to-date over add-ons te blijven en ons feedback te geven.</p>

<h3 id="Add-ons_forum">Add-onsforum</h3>

<p>Gebruik het <a href="https://discourse.mozilla-community.org/c/add-ons">Add-ons Discourse-forum</a> om alle aspecten van add-on-ontwikkeling te bespreken en hulp te verkrijgen.</p>

<h3 id="Mailing_lists">Mailinglijsten</h3>

<p>Gebruik de lijst <strong>dev-addons</strong> om ontwikkeling van het add-ons-ecosysteem te bespreken, waaronder de ontwikkeling van het WebExtensions-systeem en van AMO:</p>

<ul>
 <li><a href="https://mail.mozilla.org/listinfo/dev-addons">dev-addons-lijstinfo</a></li>
 <li><a href="https://mail.mozilla.org/pipermail/dev-addons/">dev-addons-archieven</a></li>
</ul>

<h3 id="IRC">IRC</h3>

<p>Als u een fan bent van IRC, kunt u ons bereiken via:</p>

<ul>
 <li><a href="irc://irc.mozilla.org/addons">#addons</a> (discussie over het add-ons-ecosysteem)</li>
 <li><a href="irc://irc.mozilla.org/extdev">#extdev</a> (algemene discussie over add-on-ontwikkeling)</li>
 <li><a href="irc://irc.mozilla.org/webextensions">#webextensions</a> (discussie over WebExtensions in het bijzonder)</li>
</ul>

