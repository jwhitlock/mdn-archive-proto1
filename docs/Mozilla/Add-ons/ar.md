---
version: prototype1
revision_id: 1048570
locale: ar
slug: Mozilla/Add-ons
tags: "Add-ons" "TopicStub" "NeedsTranslation"
title: Add-ons
summary: 
keywords: 
needs_technical_review: True
needs_editorial_review: True
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<div class="summary">Modify and extend Mozilla applications</div>

<p><span class="seoSummary">Add-ons add new functionality to <a href="/en-US/docs/Mozilla/Gecko">Gecko</a>-based applications such as Firefox, SeaMonkey, and Thunderbird.</span><strong> </strong>There are two main types of add-on: <a href="#Extensions">Extensions</a> add new features to the application, while <a href="#Themes">Themes</a> modify the application's user interface.</p>

<p>For both extensions and themes, Mozilla operates a repository at <a href="https://addons.mozilla.org/">addons.mozilla.org</a>, also known as AMO. When you <a href="/en-US/Add-ons/Submitting_an_add-on_to_AMO">submit add-ons to AMO</a> they are reviewed, and after passing review they are made available to users. You don't have to submit add-ons to AMO, but if you do, users can take confidence in the fact that they have been reviewed, and you can benefit from AMO's visibility as a source for useful add-ons.</p>

<p>Add-ons can greatly affect the behavior of the application that hosts them. We've developed a <a href="/en-US/docs/Mozilla/Add-ons/Add-on_guidelines">set of guidelines</a> to help ensure that they provide a good experience to users. These guidelines apply for all sorts of add-ons, whether they are hosted at <a href="https://addons.mozilla.org/">addons.mozilla.org</a> or not.</p>

<hr />
<h2 id="Extensions_2"><a name="Extensions">Extensions</a></h2>

<p>Extensions add new functionality to Mozilla applications such as Firefox and Thunderbird. They can add new features to the browser, such as a different way to manage tabs, and they can modify web content to improve the usability or security of particular websites.</p>

<p>There are three different techniques you can use to build extensions: Add-on SDK-based extensions, manually bootstrapped restartless extensions, and overlay extensions.</p>

<ul class="card-grid">
 <li><span><a href="https://developer.mozilla.org/en-US/Add-ons/SDK">Add-on SDK extensions</a></span><br />
  Develop restartless extensions using a set of high-level JavaScript APIs.</li>
 <li><span><a href="/en-US/Add-ons/Bootstrapped_extensions">Restartless extensions</a></span><br />
  Develop extensions that don't require a browser restart.</li>
 <li><a href="/en-US/Add-ons/Overlay_Extensions"><span>Overlay extensions</span></a><br />
  Develop traditional extensions using a XUL overlay.</li>
</ul>

<p>If you can, it's advisable to use the Add-on SDK, which uses the restartless extension mechanism but simplifies certain tasks and cleans up after itself. If the Add-on SDK isn't sufficient for your needs, implement a manual restartless extension instead.</p>

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
<h2 id="Themes_2"><a name="Themes">Themes</a></h2>

<p>Themes are add-ons that customize the application's user interface. There are two sorts of themes: lightweight themes and complete themes.</p>

<div class="column-container">
<div class="column-half">
<p><a href="https://addons.mozilla.org/en-US/developers/docs/themes">Lightweight themes</a> are much simpler to implement than complete themes, but provide very limited customization.</p>
</div>

<div class="column-half">
<p>With <a href="/en-US/docs/Themes">complete themes</a> you can make much deeper modifications to the application UI. The documentation for complete themes is out of date, but is linked to here as a possible basis for updated documentation.</p>
</div>
</div>

<hr />
<h2 id="Other_types_of_add-ons">Other types of add-ons</h2>

<p><a href="/en-US/docs/Creating_OpenSearch_plugins_for_Firefox">Search engine plugins</a> are a simple and very specific type of add-on: they add new search engines to the browser's search bar.</p>

<p><strong><a href="/en-US/docs/Plugins">Plugins</a> </strong>help the application understand web content that it does not natively support. NPAPI plugins are a legacy technology and new sites should not use them. In general, plugins are not available on most modern mobile systems including, and websites should transition away from using plugins.</p>

<hr />
<p>{{CommunityBox("extension development", "dev-extensions", "mozilla.dev.extensions", "extdev","Add-ons forums|https://forums.mozilla.org/addons/viewforum.php?f=3|discussion and support|Visit the add-ons forums||AMO|https://addons.mozilla.org/en-US/firefox/|addons.mozilla.org|Visit addons.mozilla.org")}}</p>

<h2 id="Subnav">Subnav</h2>

<ol>
 <li><a href="/en-US/Add-ons/Overlay_Extensions" title="Overlay extensions">Overlay extensions</a></li>
 <li><a href="/en-US/Add-ons/Bootstrapped_extensions" title="Restartless extensions">Restartless extensions</a></li>
 <li><a href="/en-US/Add-ons/SDK">Add-on SDK</a>{{AddonSDKSubnav}}</li>
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

