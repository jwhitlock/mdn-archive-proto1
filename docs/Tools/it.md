---
version: prototype1
revision_id: 961809
locale: it
slug: Tools
tags: "Tools" "TopicStub" "NeedsMarkupWork" "Web Development" "NeedsTranslation" "Developing Mozilla" "Web Development:Tools" "NeedsTechnicalReview"
title: Strumenti di Sviluppo di Firefox
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>La seguente è una lista di strumenti e risorse che vi aiuteranno nel vostro processo di sviluppo web, così come vi potranno aiutare, potenzialmente, nel debugging dei vostri add-ons per Firefox.</p>

<h2 id="Web_Development" name="Web_Development">Sviluppo Web</h2>

<h3 id="Integrati_in_Firefox">Integrati in Firefox</h3>

<p>Strumenti e risorse che sono integrati in Firefox e che sono utili nello sviluppo.</p>

<dl>
 <dt><a href="/en-US/docs/Tools/Page_Inspector" title="en/Tools/Page_Inspector">Page Inspector</a> {{ fx_minversion_inline("10.0") }}</dt>
 <dd>Un utile strumento che mostra l'HTML dell'elemento che si sta puntando con il Mouse, nel contesto in cui si trova.</dd>
</dl>

<dl>
 <dt><a href="/en-US/docs/Tools/Web_Console" title="en/Tools/Web_Console">Web Console</a> {{ fx_minversion_inline("4.0") }}</dt>
 <dd>Una console che offre interattivamente informazioni sull'output, esegue dei frammenti in JavaScript e li sperimenta con il contenuto.</dd>
</dl>

<dl>
 <dt><a href="/en-US/docs/Tools/Scratchpad" title="en/Tools/Scratchpad">Scratchpad</a> {{ fx_minversion_inline("6.0") }}</dt>
 <dd>Un editor di testo integrato in Firefox che vi permette di editare ed eseguire del codice JavaScript.</dd>
 <dt><a href="/en-US/docs/Tools/Style_Editor" title="en/Tools/Style Editor">Style Editor</a> {{ fx_minversion_inline("11.0") }}</dt>
 <dd>Vi permette di editare gli stili CSS della pagina corrente in tempo reale; in aggiunta, è possibile attivarli o disattivarli. Un fantastico modo di lavorare in tempo reale sull'aspetto del sito!</dd>
 <dt><a href="/en-US/docs/Tools/Debugger" title="/en-US/docs/Tools/Debugger">JavaScript Debugger</a> {{ fx_minversion_inline("15.0") }}</dt>
 <dd>Scorrendo il codice JavaScript in esecuzione nel Browser (o eventualmente in un Browser remoto!) e visualizzando le variabili, vi aiuta a rilevare i bugs. Questa documentazione inoltre include il Debugger Remoto, che potrete usare per il debug di codice in esecuzione in un dispositivo Firefox OS o in Firefox in un dispositivo Android.</dd>
 <dt><a href="/en-us/docs/Tools/Responsive_Design_View" title="/en-us/docs/Tools/Responsive_Design_View">Responsive Design View</a> {{ fx_minversion_inline("15.0") }}</dt>
 <dd>Visualizza come, il vostro design, si mostra con le differenti risoluzioni senza cambiare la dimensione di finestra del vostro browser.</dd>
 <dt><a href="/en-US/docs/Tools/Using_the_Source_Editor" title="en/Tools/Using the Source Editor">Using the Source Editor</a></dt>
 <dd>Il Source Editor non è uno strumento integrato; mentre, invece, è l'editor usato in Scratchpad e in Style Editor. Questo articolo fornisce le informazioni comuni di tutti gli strumenti che fanno uso delle <a href="/en-US/docs/JavaScript_code_modules/source-editor.jsm" title="source-editor.jsm">Source Editor API</a>.</dd>
 <dt><a href="/en-US/docs/Tools/GCLI" title="en/Tools/GCLI">Developer Toolbar</a> {{ fx_minversion_inline("16.0") }}</dt>
 <dd>La Developer Toolbar fornisce una interfaccia a riga di comando per manipolare e lavorare con gli strumenti di sviluppo in Firefox e dei bottoni per un accesso rapido agli strumenti usati più comunemente.</dd>
</dl>

<h3 id="Extensions" name="Extensions">Estensioni</h3>

<dl>
 <dt><a class="link-https" href="https://addons.mozilla.org/en-US/firefox/addon/1843">Firebug</a></dt>
 <dd>Integra una ricca quantità di strumenti di sviluppo per editare, eseguire il debug, e visualizzare CSS, HTML, e JavaScript in tempo reale in qualunque pagina web (<a class="external" href="http://www.getfirebug.com/">details</a>)</dd>
</dl>

<dl>
 <dt><a href="/en-US/docs/DOM_Inspector" title="en/DOM_Inspector">DOM Inspector</a></dt>
 <dd>Uno strumento di sviluppo utilizzato per ispezionare, sfogliare, e editare i DOM di documenti - solitamente pagine web o finestre XUL.</dd>
</dl>

<dl>
 <dt><a class="link-https" href="https://addons.mozilla.org/en-US/firefox/addon/60">Web Developer</a></dt>
 <dd>Aggiunge un menu e una toolbar al browser con vari strumenti di sviluppo web. (<a class="external" href="http://chrispederick.com/work/web-developer/">details</a>)</dd>
</dl>

<dl>
 <dt><a class="link-https" href="https://addons.mozilla.org/en-US/firefox/addon/4111">Aardvark</a></dt>
 <dd>Rivela elementi DOM come si trascina il mouse sulla pagina. (<a class="external" href="http://www.karmatics.com/aardvark/">details</a>)</dd>
</dl>

<dl>
 <dt><a class="link-https" href="https://addons.mozilla.org/en-US/firefox/browse/type:1/cat:4">More on Firefox Add-ons</a></dt>
 <dd>Nella Categoria Web development nel sito Firefox Add-ons</dd>
</dl>

<h2 id="Validators" name="Validators">Validatori</h2>

<dl>
 <dt><a href="/en-US/docs/Tools/Validators" title="en/Tools/Validators">List of validators</a></dt>
 <dd>Vari validatori per elementi di tipo HTML, CSS, RDF, Firefox extensions e molti altri.</dd>
</dl>

<h2 id="Authoring_Software" name="Authoring_Software">Software di Authoring</h2>

<dl>
 <dt><a class="external" href="http://tidy.sourceforge.net/">HTMLTidy</a></dt>
 <dd>Strumento utilizzato per riparare o segnalare HTML invalidi, nonchè per migliorare il layout e lo stile di rientro nel markup risultante.</dd>
</dl>

<h2 id="JavaScript" name="JavaScript">JavaScript</h2>

<dl>
 <dt><a href="/en-US/docs/Error_Console" title="en/Error_Console">Error Console</a></dt>
 <dd>Strumento usato per segnalare errori in applicazioni chrome e pagine web user-opened. Inoltre, segnala errori e warnings relativi ai JavaScript, Errori dei CSS e messaggi arbitrari dal codice chrome.</dd>
</dl>

<dl>
 <dt><a href="/en-US/docs/Venkman" title="en/Venkman">Venkman</a></dt>
 <dd>Il Debugger JavaScript di Mozilla</dd>
 <dt><a class="external" href="http://www.jshint.com/">JSHint</a></dt>
 <dd>Strumento di Analisi statica e di controllo qualità del codice JavaScript</dd>
</dl>

<dl>
 <dt><a class="external" href="http://www.jslint.com/">JSLint</a></dt>
 <dd>Strumento di controllo qualità del codice JavaScript</dd>
</dl>

<dl>
 <dt><a class="external" href="http://jsdoc.sourceforge.net/">JSDoc</a></dt>
 <dd>Strumento usato per generare (solitamente in HTML) documentazione di riferimento dai commenti nel codice (simile a JavaDoc).</dd>
</dl>

<h2 id="DOM" name="DOM">DOM</h2>

<dl>
 <dt><a href="/en-US/docs/DOM_Inspector" title="en/DOM_Inspector">DOM Inspector</a></dt>
 <dd>Strumento di sviluppo usato per ispezionare, editare i Document Object Model di documenti</dd>
</dl>

<dl>
 <dt><a class="external" href="http://slayeroffice.com/tools/modi/v2.0/modi_help.html">MODI</a></dt>
 <dd>Mouseover DOM Inspector è un bookmarklet che vi consente di vedere e manipolare il DOM di una pagina web semplicemente scorrendo il mouse sul documento.</dd>
</dl>

<h2 id="Localization" name="Localization">Localizzazione</h2>

<dl>
 <dt><a class="external" href="http://www.mozilla.org/projects/l10n/mlp_tools.html">Localization and Leveraging Tools</a></dt>
 <dd>Strumenti e risorse che aiutano a localizzare e tradurre le vostre estensioni in altre lingue.</dd>
</dl>

<h2 id="Accessibility" name="Accessibility">Accessibilità</h2>

<h3 id="Policy">Policy</h3>

<dl>
 <dt><a class="external" href="http://www.w3.org/WAI/intro/aria" target="external" title="WAI-ARIA Overview">WAI-ARIA Overview</a></dt>
 <dd>una overview di WAI-ARIA, la Suite Acessible Rich Internet Applications; un set di documenti per rendere i siti Web 2.0 e le applicazioni più accessibili.</dd>
</dl>

<h3 id="Strumenti_di_Testing">Strumenti di Testing</h3>

<dl>
 <dt><a class="external" href="http://achecker.ca/checker/index.php" target="external" title="AChecker">AChecker</a></dt>
 <dd>AChecker è un tool che vi consente di inserire un url e testarne l'accessibilità.</dd>
 <dt><a class="external" href="http://www.w3.org/WAI/ER/tools/complete" target="external" title="W3C Complete list of tools">W3C complete list of tools</a></dt>
 <dd>Una Completa lista di strumenti di valutazione di accessibilità nel web</dd>
</dl>

<p>per consultare una più globale lista di risorse sull'accessibilità, guarda: <a class="external" href="http://wiki.fluidproject.org/display/fluid/Accessibility+Resources" target="external" title="Accessibility resources">Fluid Project accessibility resources</a> e <a href="/en-US/docs/Accessibility/ARIA" title="ARIA">ARIA</a></p>

<h2 id="Tree_and_branch_management" name="Tree_and_branch_management">Tree e branch management</h2>

<dl>
 <dt><a href="/en-US/docs/Using_cross_commit" title="en/Using_cross_commit"><code>cross-commit</code> script</a></dt>
 <dd>Il Concurrent Versions System(CVS) script permette, ad una singola patch, di essere facilmente verificata in multipli branches.</dd>
</dl>

<h2 id="User_Profile_Tools" name="User_Profile_Tools">Strumenti profilo utente</h2>

<p><a href="/en-US/docs/Mozilla/Multiple_Firefox_Profiles" title="Multiple Firefox profiles">Multiple Firefox profiles</a></p>

<h2 id="Navigazione_del_Mozilla_Codebase">Navigazione del Mozilla Codebase</h2>

<p><a class="external" href="http://mxr.mozilla.org/" title="http://mxr.mozilla.org/">MXR</a> (se usate vim, mxr-vim velocizza il processo)</p>

<p><a class="external" href="http://dxr.mozilla.org/clang/" title="http://dxr.mozilla.org/clang/">DXR</a></p>

<dl>
 <dt><a class="external" href="/en-US/docs/Profile_Manager" title="en/Profile_Manager">Profile Manager</a></dt>
</dl>

<p><span class="comment">Categories</span></p>

<p><span class="comment">Interwiki Language Links</span></p>

