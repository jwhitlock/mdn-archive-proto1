---
version: prototype1
revision_id: 1104621
locale: sv-SE
slug: Mozilla/Add-ons
tags: "Landar" "Mozilla" "Tillägg" "Förlänging" "förlängning" "Förlängningar"
title: Add-ons
summary: 
keywords: 
needs_technical_review: False
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
<h2 id="Förlängningar"><a name="Extensions">Förlängningar</a></h2>

<p>Extensions add new functionality to Mozilla applications such as Firefox and Thunderbird. They can add new features to the browser, such as a different way to manage tabs, and they can modify web content to improve the usability or security of particular websites.</p>

<p>There are three different techniques you can use to build extensions: Add-on SDK-based extensions, manually bootstrapped restartless extensions, and legacy extensions.</p>

<ul class="card-grid">
 <li><span><a href="https://developer.mozilla.org/en-US/Add-ons/SDK">Add-on SDK extensions</a></span><br />
  Extensions built using a set of high-level JavaScript APIs, which don't require a browser restart to install.</li>
 <li><span><a href="/en-US/Add-ons/Bootstrapped_extensions">Restartless extensions</a></span><br />
  Extensions which don't require a browser restart to install.</li>
 <li><a href="/en-US/Add-ons/Overlay_Extensions"><span>Legacy extensions</span></a><br />
  Legacy extensions which require a browser restart to install, generally using <a href="/en-US/docs/Mozilla/Tech/XUL/Overlays">XUL overlays</a>.</li>
</ul>

<div class="note">
<p><strong>Webbförlängningar</strong></p>

<p>We're working on a system called WebExtensions, which is a new way to develop WebExtensions for Firefox, that will be largely compatible with the system used by Chrome and Opera.</p>

<p>In the future this will be the preferred way to develop extensions for Firefox.</p>

<p>At the moment the implementation of this is experimental, but you can <a href="/en-US/Add-ons/WebExtensions">see the docs here</a> if you want to give it a spin.</p>
</div>

<p>If you can, it's advisable to use the Add-on SDK, which uses the restartless extension mechanism but simplifies certain tasks and cleans up after itself. If the Add-on SDK isn't sufficient for your needs, implement a manual restartless extension instead.</p>

<p>For more information on choosing which technique to use, read this <a href="/en-US/Add-ons/Comparing_Extension_Toolchains">comparison</a>.</p>

<h3 id="Felsökning">Felsökning</h3>

<p>Extension development is hard without being able to debug to see what lines errors were made on. You must enable the developer preferences in order for the logs to be show in the Browser Console. For desktop see here: <a href="/en-US/docs/Mozilla/Add-ons/Setting_up_extension_development_environment#Development_preferences">Setting up an extension development environment</a>.</p>

<p>For desktop follow <a href="/en-US/Add-ons/Overlay_Extensions/XUL_School/Setting_Up_a_Development_Environment">Setting Up a Development Environment</a>, for Mobile (Android/iOS) follow <a href="/en-US/docs/Tools/Remote_Debugging/Debugging_Firefox_for_Android_with_WebIDE">Debugging Firefox for Android with WebIDE </a>which uses the "Browser Toolbox" from within the desktop WebIDE to catch errors occuring on the mobile device, for Firefox OS also use the WebIDE.</p>

<div class="column-container">
<div class="column-half">
<h3 id="Recommended_practices">Recommended practices</h3>

<p>No matter how you develop an extension, there are some guidelines you can follow to help ensure your extension provides as good a user experience as possible.</p>

<dl>
 <dt><a href="/en-US/Add-ons/Performance_best_practices_in_extensions">Performance</a></dt>
 <dd>Ensuring your extension is fast, responsive and memory-efficient.</dd>
 <dt><a href="/en-US/Add-ons/Security_best_practices_in_extensions">Säkerhet</a></dt>
 <dd>Ensuring your extension doesn't expose the user to malicious websites.</dd>
 <dt><a href="/en-US/Add-ons/Extension_etiquette">Etikett</a></dt>
 <dd>Ensuring your extension plays nicely with other extensions.</dd>
</dl>
</div>

<div class="column-half">
<h3 id="Application-specific">Application-specific</h3>

<p>Most of the documentation assumes you're developing for Firefox Desktop. If you're developing for some other Gecko-based application, there are major differences you need to know about.</p>

<dl>
 <dt><a href="/en-US/Add-ons/Thunderbird">Thunderbird</a></dt>
 <dd>Developing extensions for the Thunderbird mail client.</dd>
 <dt><a href="/en-US/Add-ons/Firefox_for_Android">Firefox för Android</a></dt>
 <dd>Developing extensions for Firefox for Android.</dd>
 <dt><a href="/en-US/Add-ons/SeaMonkey_2">SeaMonkey</a></dt>
 <dd>Developing extensions for the <a href="http://www.seamonkey-project.org/">SeaMonkey</a> software suite.</dd>
</dl>
</div>
</div>

<hr />
<h2 id="Teman"><a name="Themes">Teman</a></h2>

<p>Themes are add-ons that customize the application's user interface. There are two sorts of themes: lightweight themes and complete themes.</p>

<div class="column-container">
<div class="column-half">
<p><a href="/Add-ons/Themes/Background">Lightweight themes</a> are much simpler to implement than complete themes, but provide very limited customization.</p>
</div>

<div class="column-half">
<p>With <a href="/en-US/docs/Themes">complete themes</a> you can make much deeper modifications to the application UI. The documentation for complete themes is out of date, but is linked to here as a possible basis for updated documentation.</p>
</div>
</div>

<hr />
<h2 id="Andra_typer_av_tillägg">Andra typer av tillägg</h2>

<p><a href="/en-US/docs/Creating_OpenSearch_plugins_for_Firefox">Search engine plugins</a> are a simple and very specific type of add-on: they add new search engines to the browser's search bar.</p>

<p><strong><a href="/en-US/docs/Plugins">Plugins</a> </strong>help the application understand web content that it does not natively support. NPAPI plugins are a legacy technology and new sites should not use them. In general, plugins are not available on most modern mobile systems including, and websites should transition away from using plugins.</p>

<hr />
<p>{{CommunityBox("extension development", "dev-extensions", "mozilla.dev.extensions", "extdev","Add-ons forums|https://discourse.mozilla-community.org/c/add-ons|discussion and support|Visit the add-ons forums||AMO|https://addons.mozilla.org/en-US/firefox/|addons.mozilla.org|Visit addons.mozilla.org")}}</p>

<h2 id="Subnav">Subnav</h2>

<ol>
 <li><a href="/en-US/Add-ons/Bootstrapped_extensions" title="Restartless extensions">Restartless extensions</a></li>
 <li><a href="/en-US/Add-ons/Overlay_Extensions" title="Legacy extensions">Legacy extensions</a></li>
 <li><a href="/en-US/Add-ons/SDK">Add-on SDK</a></li>
 <li><a href="#">Tekniker</a>
  <ol>
   <li><a href="/en-US/Add-ons/Techniques/Promises">Promises</a></li>
  </ol>
 </li>
 <li><a href="#">Recommended practices</a>
  <ol>
   <li><a href="/en-US/Add-ons/Performance_best_practices_in_extensions" title="Performance">Performance</a></li>
   <li><a href="/en-US/Add-ons/Security_best_practices_in_extensions" title="Security">Säkerhet</a></li>
   <li><a href="/en-US/Add-ons/Extension_etiquette" title="Etiquette">Etikett</a></li>
  </ol>
 </li>
 <li><a href="#">Teman</a>
  <ol>
   <li><a href="/Add-ons/Themes/Background" title="Lightweight themes">Lightweight themes</a></li>
   <li><a href="/Add-ons/Themes/Background/FAQ" title="Lightweight themes FAQ">Lightweight themes FAQ</a></li>
   <li><a href="/en-US/docs/Themes" title="Complete themes">Complete themes</a></li>
  </ol>
 </li>
 <li><a href="#">Legacy Plugins </a>
  <ol>
   <li><a href="/en-US/docs/Plugins/Guide/Plug-in_Basics">Plug-in Basics</a></li>
   <li><a href="/en-US/docs/Plugins/Guide/Plug-in_Development_Overview">Plug-in Development Overview</a></li>
   <li><a href="/en-US/docs/Plugins/Guide/Initialization_and_Destruction">Initialization and Destruction</a></li>
   <li><a href="/en-US/docs/Plugins/Guide/Drawing_and_Event_Handling">Drawing and Event Handling</a></li>
   <li><a href="/en-US/docs/Plugins/Guide/Streams">Strömmar</a></li>
   <li><a href="/en-US/docs/Plugins/Guide/URLs">URLs</a></li>
   <li><a href="/en-US/docs/Plugins/Guide/Memory">Minne</a></li>
   <li><a href="/en-US/docs/Plugins/Guide/Version%2C_UI%2C_and_Status_Information">Version, UI, och Status Information</a></li>
   <li><a href="/en-US/docs/Plugins/Guide/Plug-in_Side_Plug-in_API">Plug-in side Plug-in API</a>
    <ol>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPP_Destroy">NPP_Destroy</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPP_DestroyStream">NPP_DestroyStream</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPP_GetValue">NPP_GetValue</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NP_GetValue">NP_GetValue</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPP_HandleEvent">NPP_HandleEvent</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NP_Initialize">NP_Initialize</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPP_New">NPP_New</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPP_NewStream">NPP_NewStream</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPP_Print">NPP_Print</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPP_SetValue">NPP_SetValue</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPP_SetWindow">NPP_SetWindow</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NP_Shutdown">NP_Shutdown</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPP_StreamAsFile">NPP_StreamAsFile</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPP_URLNotify">NPP_URLNotify</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPP_Write">NPP_Write</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPP_WriteReady">NPP_WriteReady</a></li>
    </ol>
   </li>
   <li><a href="/en-US/docs/Plugins/Guide/Browser_Side_Plug-in_API">Browser Side Plug-in API</a>
    <ol>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_DestroyStream" title="Closes and deletes a stream.">NPN_DestroyStream</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_ForceRedraw" title="Asks the plugin host to immediately (synchronously) repaint invalid areas.">NPN_ForceRedraw</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_GetAuthenticationInfo" title="The function is called by plugins to get HTTP authentication information from the browser.">NPN_GetAuthenticationInfo</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_GetURL" title="Asks the browser to create a stream for the specified URL.">NPN_GetURL</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_GetURLNotify" title="Requests creation of a new stream with the contents of the specified URL; gets notification of the result.">NPN_GetURLNotify</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_GetValue" title="Allows the plug-in to query the browser for information.">NPN_GetValue</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_GetValueForURL" title="Provides information to a plugin which is associated with a given URL, for example the cookies or preferred proxy.">NPN_GetValueForURL</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_InvalidateRect" title="Invalidates the specified portion of the plugin's drawing area, adding it to the region that needs to be redrawn when the plugin next repaints its contents.">NPN_InvalidateRect</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_InvalidateRegion" title="Invalidates the specified drawing region prior to repainting or refreshing a windowless plug-in.">NPN_InvalidateRegion</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_MemAlloc" title="Allocates memory from the browser's memory space.">NPN_MemAlloc</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_MemFlush" title="Requests that the browser free a specified amount of memory.">NPN_MemFlush</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_MemFree" title="Deallocates a block of allocated memory.">NPN_MemFree</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_NewStream" title="Requests the creation of a new data stream produced by the plug-in and consumed by the browser.">NPN_NewStream</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_PluginThreadAsyncCall" title="Thread safe way to request that the browser calls a plug-in function on the browser or plugin thread (the thread on which the plug-in was initiated).">NPN_PluginThreadAsyncCall</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_PostURL" title="Posts data to a URL.">NPN_PostURL</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference//NPN_PostURLNotify" title="Posts data to a URL, and receives notification of the result.">NPN_PostURLNotify</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_ReloadPlugins" title="Reloads all of the installed plugins.">NPN_ReloadPlugins</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_RequestRead" title="Requests a range of bytes from a seekable stream. This initiates a read operation; the actual data is received through subsequent calls to NPP_WriteReady() and NPP_Write().">NPN_RequestRead</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_SetValue" title="Implemented by browsers. This call is used to inform the browser of variable information controlled by the plugin.">NPN_SetValue</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_SetValueForURL" title="Allows a plugin to change the stored information associated with a URL, in particular its cookies. (While the API theoretically allows the preferred proxy for a given URL to be changed, doing so does not have much meaning given how proxies are configured, and is not supported.)">NPN_SetValueForURL</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_Status" title="Lets a plug-in display a message on the browser's status line.">NPN_Status</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_UserAgent" title="Returns the browser's user agent field. This can be used to handle variations in different browsers (or versions thereof) when implementing your plug-in.">NPN_UserAgent</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/docs/NPN_Version" title="Lets plugins obtain version information, both of the plug-in API and of the browser itself.">NPN_Version</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_Write" title="Pushes data into a stream produced by the plug-in and consumed by the browser.">NPN_Write</a></li>
    </ol>
   </li>
   <li><a href="/en-US/docs/Plugins/Guide/Scripting_plugins">Scripting plugins</a>
    <ol>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPString">NPString</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPVariant">NPVariant</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_ReleaseVariantValue">NPN_ReleaseVariantValue</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_GetStringIdentifier">NPN_GetStringIdentifier</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_GetStringIdentifiers">NPN_GetStringIdentifiers</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_GetIntIdentifier">NPN_GetIntIdentifier</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_IdentifierIsString">NPN_IdentifierIsString</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_UTF8FromIdentifier">NPN_UTF8FromIdentifier</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_IntFromIdentifier">NPN_IntFromIdentifier</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPObject">NPObject</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_CreateObject">NPN_CreateObject</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_RetainObject">NPN_RetainObject</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_ReleaseObject">NPN_ReleaseObject</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_Invoke">NPN_Invoke</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_InvokeDefault">NPN_InvokeDefault</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_Evaluate">NPN_Evaluate</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_GetProperty">NPN_GetProperty</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_SetProperty">NPN_SetProperty</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_RemoveProperty">NPN_RemoveProperty</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_HasProperty">NPN_HasProperty</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_HasMethod">NPN_HasMethod</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPN_SetException">NPN_SetException</a></li>
     <li><a href="/en-US/Add-ons/Plugins/Reference/NPClass">NPClass</a></li>
    </ol>
   </li>
   <li><a href="/en-US/docs/Plugins/Guide/Structures">Strukturer</a></li>
   <li><a href="/en-US/docs/Plugins/Guide/Constants">Constants</a></li>
   <li><a href="/en-US/Add-ons/Plugins/External_resources_for_plugin_creation">Externa resurser</a></li>
  </ol>
 </li>
 <li><a href="#">Publishing add-ons</a>
  <ol>
   <li><a href="/en-US/Add-ons/Distribution">Signing and distributing your add-on</a></li>
   <li><a href="https://addons.mozilla.org/developers/addon/submit/">Skicka in ett nytt tillägg</a></li>
   <li><a href="/en-US/Add-ons/AMO/Policy">Policies</a>
    <ol>
     <li><a href="/en-US/Add-ons/AMO/Policy/Extensions">Förlängningar</a></li>
     <li><a href="/en-US/Add-ons/AMO/Policy/Agreement">Developer Agreement</a></li>
     <li><a href="/en-US/Add-ons/AMO/Policy/Reviews">Review Process</a></li>
     <li><a href="/en-US/Add-ons/Add-on_guidelines">Add-on guidelines</a></li>
     <li><a href="/en-US/Add-ons/AMO/Policy/Featured">Featured Add-ons</a></li>
     <li><a href="/en-US/Add-ons/AMO/Policy/Contact">Contacting Us</a></li>
    </ol>
   </li>
  </ol>
 </li>
 <li><a href="#">Community and Support</a>
  <ol>
   <li><a href="https://blog.mozilla.org/addons">Add-ons Blog</a></li>
   <li><a href="https://discourse.mozilla-community.org/c/add-ons">Add-on Forums</a></li>
   <li><a href="http://stackoverflow.com/questions/tagged/firefox-addon">Stack Overflow</a></li>
   <li><a href="https://groups.google.com/forum/#!forum/mozilla.dev.extensions">Development Newsgroup</a></li>
   <li><a href="irc://irc.mozilla.org/extdev">IRC-kanal</a></li>
  </ol>
 </li>
</ol>

