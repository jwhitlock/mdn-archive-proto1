---
version: prototype1
revision_id: 1344905
locale: it
slug: Mozilla/Add-ons
tags: "Add-ons" "TopicStub"
title: Componenti aggiuntivi
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<div class="summary">Modifica ed espandi le applicazioni Mozilla</div>

<p><span class="seoSummary">I componenti aggiuntivi arricchiscono di nuove funzionalità le applicazioni basate su <a href="/it/docs/Gecko">Gecko</a> come Firefox, SeaMonkey e Thunderbird.</span><strong> </strong>Esistono due diversi tipi di componenti aggiuntivi: le <a href="#Estensioni">estensioni</a> che aggiungono nuove funzionalità all'applicazione, mentre i <a href="#Temi">temi</a> modificano l'interfaccia utente.</p>

<p>Sia le estensioni che i temi vengono raccolti in un repository gestito da Mozilla su <a href="https://addons.mozilla.org/">addons.mozilla.org</a>, noto anche come AMO. Quando uno sviluppatore sceglie di <a href="/en-US/Add-ons/Submitting_an_add-on_to_AMO">caricare un componente aggiuntivo su AMO</a>, esso viene sottoposto a una revisione e, se la supera, pubblicato sul sito per essere scaricato dagli utenti. Sottoporre i propri componenti aggiuntivi ad AMO non è obbligatorio, tuttavia costituisce la garanzia per gli utenti che il componente sia stato revisionato e offre agli sviluppatori visibilità su una piattaforma riconosciuta come fonte di applicazioni utili.</p>

<p>I componenti aggiuntivi possono alterare in maniera significativa il funzionamento dell'applicazione che li ospita. Mozilla ha quindi sviluppato una <a href="/en-US/docs/Mozilla/Add-ons/Add-on_guidelines">serie di linee guida</a> per assicurare che ogni componente offra all'utente un'esperienza ottimale. Queste linee guida sono valide per tutti i tipi di componente aggiuntivo, che siano ospitati sul server di <a href="https://addons.mozilla.org/">addons.mozilla.org</a> o meno.</p>

<hr />
<h2 id="Estensioni"><a name="Extensions">Estensioni</a></h2>

<p>Le estensioni aggiungono nuove funzionalità alle applicazioni sviluppate da Mozilla come Firefox o Thunderbird. Possono integrare il browser con funzioni particolari, come per esempio un sistema alternativo per gestire le schede, e modificare i contenuti web per migliorare l'accessibilità o la sicurezza di un sito particolare.</p>

<p>Le estensioni possono essere sviluppate con tre tecniche diverse: estensioni basate su Add-on SDK, estensioni che si avviano manualmente senza richiedere il riavvio del browser ed estensioni overlay.</p>

<ul class="card-grid">
 <li><span><a href="https://developer.mozilla.org/it/docs/Mozilla/Add-ons/SDK">Estensioni con Add-on SDK</a></span><br />
  Sviluppare estensioni con riavvio non richiesto grazie a una raccolta di API JavaScript di livello avanzato.</li>
 <li><span><a href="/en-US/Add-ons/Bootstrapped_extensions">Estensioni con riavvio non richiesto</a></span><br />
  Sviluppare estensioni che funzionano dalla prima attivazione senza bisogno di riavviare il browser.</li>
 <li><a href="/en-US/Add-ons/Overlay_Extensions"><span>Estensioni overlay</span></a><br />
  Sviluppare estensioni tradizionali che utilizzano un overlay XUL.</li>
</ul>

<p>Quando possibile, è consigliabile utilizzare Add-on SDK, che sfrutta lo stesso meccanismo delle estensioni con riavvio non richiesto ma semplificando alcune operazioni ed eliminando automaticamente il codice superfluo. In caso Add-on SDK non soddisfi le proprie esigenze, l'alternativa è implementare manualmente un'estensione con riavvio non richiesto. Le estensioni overlay sono attualmente obsolete, anche se ne rimane in circolazione un numero elevato.</p>

<p>Per un approfondimento su quale tecnica sia più opportuno scegliere, ecco un <a href="/en-US/Add-ons/Comparing_Extension_Toolchains">articolo comparativo</a>.</p>

<div class="column-container">
<div class="column-half">
<h3 id="Pratiche_consigliate">Pratiche consigliate</h3>

<p>Indipendentemente dalle modalità con cui si sceglie di sviluppare un'estensione, esistono linee guida comuni da rispettare per garantire che il proprio componente offra la migliore esperienza utente possibile.</p>

<dl>
 <dt><a href="/en-US/Add-ons/Performance_best_practices_in_extensions">Prestazioni</a></dt>
 <dd>Come rendere un'estensione veloce, reattiva e ottimizzata nel consumo della memoria.</dd>
 <dt><a href="/en-US/Add-ons/Security_best_practices_in_extensions">Sicurezza</a></dt>
 <dd>Come evitare di esporre l'utente a siti dannosi.</dd>
 <dt><a href="/en-US/Add-ons/Extension_etiquette">Etichetta</a></dt>
 <dd>Come gestire l'interazione con altre estensioni correttamente.</dd>
</dl>
</div>

<div class="column-half">
<h3 id="Nozioni_specifiche_per_applicazione">Nozioni specifiche per applicazione</h3>

<p>La maggior parte della documentazione è scritta pensando a chi sviluppa per Firefox Desktop. Gli sviluppatori che intendono progettare per altre applicazioni basate su Gecko devono prendere atto di alcune differenze fondamentali.</p>

<dl>
 <dt><a href="/en-US/Add-ons/Thunderbird">Thunderbird</a></dt>
 <dd>Sviluppare estensioni per il client di posta elettronica Thunderbird.</dd>
 <dt><a href="/en-US/Add-ons/Firefox_for_Android">Firefox per Android</a></dt>
 <dd>Sviluppare estensioni per la versione di Firefox per il sistema operativo Android.</dd>
 <dt><a href="/en-US/Add-ons/SeaMonkey_2">SeaMonkey</a></dt>
 <dd>Sviluppare estensioni per la suite di applicazioni <a href="http://www.seamonkey-project.org/">SeaMonkey</a>.</dd>
</dl>
</div>
</div>

<hr />
<h2 id="Temi"><a name="Themes">Temi</a></h2>

<p>I Temi sono componenti aggiuntivi in grado di personalizzare l'interfaccia utente dell'applicazione. Esistono due tipi di tema: temi di sfondo (o semplicemente "temi") e temi completi.</p>

<div class="column-container">
<div class="column-half">
<p>I <a href="https://addons.mozilla.org/it/developers/docs/themes">temi di sfondo</a> sono significativamente più semplici da implementare rispetto ai temi completi, ma offrono un livello di personalizzazione più limitato.</p>
</div>

<div class="column-half">
<p>I <a href="/it/docs/Temi">temi completi</a> consentono modifiche più radicali all'interfaccia utente dell'applicazione. La documentazione sui temi completi è attualmente incompleta, ma viene qui citata in previsione di futuri aggiornamenti.</p>
</div>
</div>

<hr />
<h2 id="Altri_tipi_di_componente_aggiuntivo">Altri tipi di componente aggiuntivo</h2>

<p>I <a href="/en-US/docs/Creating_OpenSearch_plugins_for_Firefox">plugin dei motori di ricerca</a> sono un tipo di componente aggiuntivo semplice e specifico: aggiungono nuovi motori alla barra di ricerca del browser.</p>

<p>I <a href="/en-US/docs/Plugins">plugin</a> consentono all'applicazione di elaborare contenuti non supportati nativamente. Mozilla sta tentando di scoraggiare l'implementazione dei plugin, che hanno in passato causato problemi di stabilità, prestazioni e sicurezza.</p>

<hr />
<p>{{CommunityBox("extension development", "dev-extensions", "mozilla.dev.extensions", "extdev","Forum dedicato ai componenti aggiuntivi|https://forums.mozilla.org/addons/viewforum.php?f=3|discussione e supporto|Visita il forum dedicato ai componenti aggiuntivi||AMO|https://addons.mozilla.org/it/firefox/|addons.mozilla.org|Visita addons.mozilla.org")}}</p>

