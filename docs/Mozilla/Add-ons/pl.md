---
version: prototype1
revision_id: 1329384
locale: pl
slug: Mozilla/Add-ons
tags: "Add-ons" "TopicStub" "NeedsTranslation"
title: Dodatki
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<div class="summary">Modyfikacje i rozszerzenia programu Mozilla</div>

<p><span class="seoSummary">Dodatki dodają nowych funkcji do aplikacji bazujących na Gecko takich jak Firefox, SeaMonkey i Thunderbird.</span><strong> </strong>Istnieją dwa główne typy dodatków : Rozszerzenia, które dodają nowych właściwości do programu, oraz motywy które zmieniają wygląd programu</p>

<p>Dla obu rodzajów rozszerzeń, Mozilla wprowadziła specjalną stronę <a href="https://addons.mozilla.org/">addons.mozilla.org</a>, znaną również jako "AMO" . <a href="/en-US/Add-ons/Submitting_an_add-on_to_AMO">submit add-ons to AMO</a> they are reviewed, and after passing review they are made available to users. You don't have to submit add-ons to AMO, but if you do, users can take confidence in the fact that they have been reviewed, and you can benefit from AMO's visibility as a source for useful add-ons.</p>

<p>Add-ons can greatly affect the behaviour of the application that hosts them. We've developed a <a href="/en-US/docs/Mozilla/Add-ons/Add-on_guidelines">set of guidelines</a> to help ensure that they provide a good experience to users. These guidelines apply for all sorts of add-ons, whether they are hosted at <a href="https://addons.mozilla.org/">addons.mozilla.org</a> or not.</p>

<hr />
<h2 id="Rozszerzenia"><a name="Extensions">Rozszerzenia</a></h2>

<p>Rozszerzenia dodają nową funkcjonalność do aplikacji Mozilla takich jak Firefox czy Thunderbird. Mogą dodawać nowe funkcje do przeglądarki, na przykład inny sposób zarządzania zakładkami. Mogą także modyfikować zawartość witryn, by ulepszyć użytkowanie i bezpieczeństwo określonych stron.</p>

<p>Istnieją trzy różne techniki, których możesz użyć, by stworzyć rozszerzenie: rozszerzenia bazujące na dodatkach SDK, rozszerzenia niewymagające restartu (bootstrap) oraz rozszerzenia legacy.</p>

<ul class="card-grid">
 <li><span><a href="https://developer.mozilla.org/en-US/Add-ons/SDK">Rozszerzenia bazujące na dodatkach SDK</a></span><br />
  Rozszerzenia tworzone z użyciem wysokopoziomowych JavaScript APIs, które nie potrzebują ponownego uruchamiania przeglądarki do zainstalowania.</li>
 <li><span><a href="/en-US/Add-ons/Bootstrapped_extensions">Rozszerzenia niewymagające restartu</a></span><br />
  Rozszerzenia, które nie potrzebują ponownego uruchamiania przeglądarki do zainstalowania.</li>
 <li><a href="/en-US/Add-ons/Overlay_Extensions"><span>Rozszerzenia legacy</span></a><br />
  Rozszerzenia wymagające ponowne uruchamianie przeglądarki do zainstalowania; głównie z użyciem <a href="https://developer.mozilla.org/en-US/docs/Mozilla/Tech/XUL/Overlays">XUL overlays</a>.</li>
</ul>

<p>If you can, it's advisable to use the Add-on SDK, which uses the restartless extension mechanism but simplifies certain tasks and cleans up after itself. If the Add-on SDK isn't sufficient for your needs, implement a manual restartless extension instead. Overlay extensions are mostly obsolete now, although there are still many of them in the wild.</p>

<p>For more information on choosing which technique to use, read this <a href="/en-US/Add-ons/Comparing_Extension_Toolchains">comparison</a>.</p>

<div class="column-container">
<div class="column-half">
<h3 id="Good_practices">Good practices</h3>

<p>No matter how you develop an extension, there are some guidelines you can follow to help ensure your extension provides as good a user experience as possible.</p>

<dl>
 <dt><a href="/en-US/Add-ons/Performance_best_practices_in_extensions">Performance</a></dt>
 <dd>Ensuring your extension is fast, responsive and memory-efficient.</dd>
 <dt><a href="/en-US/Add-ons/Security_best_practices_in_extensions">Security</a></dt>
 <dd>Ensuring your extension doesn't expose the user to malicious websites.</dd>
 <dt><a href="/en-US/Add-ons/Extension_etiquette">Etiquette</a></dt>
 <dd>Ensuring your extension plays nicely with other extensions.</dd>
</dl>
</div>

<div class="column-half">
<h3 id="Application-specific">Application-specific</h3>

<p>Most of the documentation assumes you're developing for Firefox Desktop. If you're developing for some other Gecko-based application, there are major differences you need to know about.</p>

<dl>
 <dt><a href="/en-US/Add-ons/Thunderbird">Thunderbird</a></dt>
 <dd>Developing extensions for the Thunderbird mail client.</dd>
 <dt><a href="/en-US/Add-ons/Firefox_for_Android">Firefox for Android</a></dt>
 <dd>Developing extensions for Firefox for Android.</dd>
 <dt><a href="/en-US/Add-ons/SeaMonkey_2">SeaMonkey</a></dt>
 <dd>Developing extensions for the <a href="http://www.seamonkey-project.org/">SeaMonkey</a> software suite.</dd>
</dl>
</div>
</div>

<hr />
<h2 id="Themes_2"><a name="Themes">Motywy</a></h2>

<p>Motywy to dodatki modyfikujące interfejs użytkownika. Istnieją dwa rodzaje motywów: lekkie&nbsp; i kompletne motywy.</p>

<div class="column-container">
<div class="column-half">
<p><a href="https://addons.mozilla.org/en-US/developers/docs/themes">Lekkie motywy</a> są prostsze w implementacji od kompletnych motywów, ale są też bardzo ograniczone.<br />
 <br />
 Z&nbsp; <a href="/en-US/docs/Themes">kompletnymi motywami</a> możesz dokonywać głębszych modyfikacji w UI. Dokumentacja tych motywów jest nieaktualna, ale jest tutaj podlinkowana zaktualizowana wersja.</p>
</div>
</div>

<hr />
<h2 id="Other_types_of_add-ons">Inne rodzaje dodatków</h2>

<p><a href="/en-US/docs/Creating_OpenSearch_plugins_for_Firefox">Search engine plugins</a> are a simple and very specific type of add-on: they add new search engines to the browser's search bar.</p>

<p><a href="/en-US/docs/Plugins">Plugins</a> help the application understand content that it does not natively support. We're in the process of deprecating support for these plugins, as they have a history of causing stability, performance, and security problems.</p>

<hr />
<p>{{CommunityBox("extension development", "dev-extensions", "mozilla.dev.extensions", "extdev","Add-ons forums|https://forums.mozilla.org/addons/viewforum.php?f=3|discussion and support|Visit the add-ons forums||AMO|https://addons.mozilla.org/en-US/firefox/|addons.mozilla.org|Visit addons.mozilla.org")}}</p>

<h2 id="Subnav">Subnav</h2>

<ol>
 <li><a href="/en-US/User:wbamberg/Add-ons/Overlay_Extensions" title="Overlay extensions">Overlay extensions</a></li>
 <li><a href="/en-US/docs/Extensions/Bootstrapped_extensions" title="Restartless extensions">Restartless extensions</a></li>
 <li><a href="https://addons.mozilla.org/en-US/developers/docs/sdk/latest/dev-guide/index.html">Add-on SDK</a>{{AddonSDKSubnav}}</li>
 <li><a href="#">Extension good practices</a>
  <ol>
   <li><a href="/en-US/Add-ons/Performance_best_practices_in_extensions" title="Performance">Performance</a></li>
   <li><a href="/en-US/Add-ons/Security_best_practices_in_extensions" title="Security">Security</a></li>
   <li><a href="/en-US/Add-ons/Extension_etiquette" title="Etiquette">Etiquette</a></li>
  </ol>
 </li>
 <li><a href="#">Themes</a>
  <ol>
   <li><a href="https://addons.mozilla.org/en-US/developers/docs/themes" title="Lightweight themes">Lightweight themes</a></li>
   <li><a href="/en-US/docs/Themes" title="Complete themes">Complete themes</a></li>
  </ol>
 </li>
 <li><a href="#">Publishing add-ons</a>
  <ol>
   <li><a href="https://addons.mozilla.org/" title="addons.mozilla.org">addons.mozilla.org</a></li>
   <li><a href="/en-US/docs/Mozilla/Add-ons/Add-on_guidelines">Add-on guidelines</a></li>
  </ol>
 </li>
</ol>

