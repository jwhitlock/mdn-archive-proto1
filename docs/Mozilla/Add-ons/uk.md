---
version: prototype1
revision_id: 1328561
locale: uk
slug: Mozilla/Add-ons
tags: 
title: Add-ons
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<p>{{AddonSidebar}}</p>

<div class="summary">Modify and extend Mozilla applications</div>

<p><span class="seoSummary">Add-ons add new functionality to <a href="/en-US/docs/Mozilla/Gecko">Gecko</a>-based applications such as Firefox, SeaMonkey, and Thunderbird.</span><strong> </strong>There are two main types of add-on: <a href="#Extensions">Extensions</a> add new features to the application, while <a href="#Themes">Themes</a> modify the application's user interface.</p>

<p>Add-ons can greatly affect the behavior of the application that hosts them. We've developed a <a href="/en-US/docs/Mozilla/Add-ons/Add-on_guidelines">set of guidelines</a> to help ensure that they provide a good experience to users. These guidelines apply for all sorts of add-ons, whether they are hosted at <a href="https://addons.mozilla.org/">addons.mozilla.org</a> or not.</p>

<hr>
<h2 id="Extensions_2"><a name="Extensions">Extensions</a></h2>

<p>Extensions add new functionality to Mozilla applications such as Firefox and Thunderbird. They can add new features to the browser, such as a different way to manage tabs, and they can modify web content to improve the usability or security of particular websites.</p>

<p>There are three different techniques you can use to build extensions: Add-on SDK-based extensions, manually bootstrapped restartless extensions, and legacy extensions.</p>

<ul class="card-grid">
 <li><span><a href="https://developer.mozilla.org/en-US/Add-ons/SDK">Add-on SDK extensions</a></span><br>
  Extensions built using a set of high-level JavaScript APIs, which don't require a browser restart to install.</li>
 <li><span><a href="/en-US/Add-ons/Bootstrapped_extensions">Restartless extensions</a></span><br>
  Extensions which don't require a browser restart to install.</li>
 <li><a href="/en-US/Add-ons/Overlay_Extensions"><span>Legacy extensions</span></a><br>
  Legacy extensions which require a browser restart to install, generally using <a href="/en-US/docs/Mozilla/Tech/XUL/Overlays">XUL overlays</a>.</li>
</ul>

<div class="note">
<p><strong>WebExtensions</strong></p>

<p>We're working on a system called WebExtensions, which is a new way to develop WebExtensions for Firefox, that will be largely compatible with the system used by Chrome and Opera.</p>

<p>In the future this will be the preferred way to develop extensions for Firefox.</p>

<p>At the moment the implementation of this is experimental, but you can <a href="/en-US/Add-ons/WebExtensions">see the docs here</a> if you want to give it a spin.</p>
</div>

<p>If you can, it's advisable to use the Add-on SDK, which uses the restartless extension mechanism but simplifies certain tasks and cleans up after itself. If the Add-on SDK isn't sufficient for your needs, implement a manual restartless extension instead.</p>

<p>For more information on choosing which technique to use, read this <a href="/en-US/Add-ons/Comparing_Extension_Toolchains">comparison</a>.</p>

<h3 id="Debugging">Debugging</h3>

<p>Extension development is hard without being able to debug to see what lines errors were made on. You must enable the developer preferences in order for the logs to be show in the Browser Console. For desktop see here: <a href="/en-US/docs/Mozilla/Add-ons/Setting_up_extension_development_environment#Development_preferences">Setting up an extension development environment</a>.</p>

<p>For desktop follow <a href="/en-US/Add-ons/Overlay_Extensions/XUL_School/Setting_Up_a_Development_Environment">Setting Up a Development Environment</a>, for Mobile (Android/iOS) follow <a href="/en-US/docs/Tools/Remote_Debugging/Debugging_Firefox_for_Android_with_WebIDE">Debugging Firefox for Android with WebIDE </a>which uses the "Browser Toolbox" from within the desktop WebIDE to catch errors occuring on the mobile device, for Firefox OS also use the WebIDE.</p>

<div class="column-container">
<div class="column-half">
<h3 id="Recommended_practices">Recommended practices</h3>

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

<hr>
<h2 id="Publishing_your_add-on">Publishing your add-on</h2>

<p>Mozilla operates a platform for reviewing, signing, and distributing add-ons and themes at <a href="https://addons.mozilla.org/">addons.mozilla.org</a>, also known as AMO.</p>

<p>You don't have to list your add-on on AMO, but starting in Firefox 43, you must submit your add-on to AMO so it can be reviewed and signed, or Firefox release users won't be able to install your add-on. If you do list your add-on on AMO, you can benefit from its visibility as a source for useful add-ons.</p>

<ul>
 <li><a href="https://developer.mozilla.org/en-US/Add-ons/Distribution">Signing and distributing your add-on</a>: how to get your add-on signed and published, whether it's listed on AMO or not.</li>
 <li><a href="https://developer.mozilla.org/en-US/Add-ons/AMO/Policy/Reviews">AMO review policies</a>: the checks that are made on add-ons when they are reviewed.</li>
 <li><a href="/en-US/Add-ons/AMO/Add-ons_manager_API">AMO API</a>: the <a href="https://addons.mozilla.org">addons.mozilla.org</a> website has an API that allows you to retrieve data about a single add-on, groups of add-ons, or to search add-ons.</li>
 <li><a href="https://developer.mozilla.org/en-US/Add-ons/AMO/Policy/Featured">Policies for Featured add-ons</a>: featured add-ons are top-quality extensions and themes highlighted on <a href="https://addons.mozilla.org/en-US/firefox/extensions/?sort=featured" class="external external-icon">AMO</a>, Firefox's Add-ons Manager, and across other Mozilla websites.</li>
 <li><a href="/en-US/Add-ons/AMO/Policy/Contact">AMO contact information</a></li>
</ul>

<hr>
<h2 id="Other_types_of_add-ons">Other types of add-ons</h2>

<p><a href="/Add-ons/Themes/Background">Lightweight themes</a> are much simpler to implement than complete themes, but provide very limited customization.</p>

<p>With <a href="/en-US/docs/Themes">complete themes</a> you can make much deeper modifications to the application UI. The documentation for complete themes is out of date, but is linked to here as a possible basis for updated documentation.</p>

<p><a href="/en-US/docs/Creating_OpenSearch_plugins_for_Firefox">Search engine plugins</a> are a simple and very specific type of add-on: they add new search engines to the browser's search bar.</p>

<p><strong><a href="/en-US/docs/Plugins">Plugins</a> </strong>help the application understand web content that it does not natively support. NPAPI plugins are a legacy technology and new sites should not use them. In general, plugins are not available on most modern mobile systems including, and websites should transition away from using plugins.</p>

<hr>
<p>{{CommunityBox("extension development", "dev-extensions", "mozilla.dev.extensions", "extdev","Add-ons forums|https://discourse.mozilla-community.org/c/add-ons|discussion and support|Visit the add-ons forums||AMO|https://addons.mozilla.org/en-US/firefox/|addons.mozilla.org|Visit addons.mozilla.org")}}</p>

