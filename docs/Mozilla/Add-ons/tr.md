---
version: prototype1
revision_id: 1130323
locale: tr
slug: Mozilla/Eklentiler
tags: "Landing" "Mozilla" "Eklentiler" "uzantılar"
title: Eklentiler
summary: 
keywords: 
needs_technical_review: True
needs_editorial_review: True
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div class="summary">Mozilla uygulamalarını değiştirin ve genişletin.</div>

<p><span class="seoSummary">Eklentiler<a href="/en-US/docs/Mozilla/Gecko">, Gecko</a>-tabanlı uygulamalara (Firefox,SeaMonkey ve Thunderbird gibi) yeni fonksiyonellikler eklerler. İki çeşit ana eklenti tipi vardır:</span> <a href="#Extensions">Uzantılar</a>, uygulamaya yeni özellikler eklerler, ve <a href="#Themes">Temalar</a> ise kullanıcı arayüzünü modifiye ederler.</p>

<p>Her iki eklenti tipi için Mozilla, AMO diye bilinen, <a href="https://addons.mozilla.org/">addons.mozilla.org</a>'da bir dizinde çalışır. <a href="/en-US/Add-ons/Submitting_an_add-on_to_AMO">AMO'ya gönderdiğiniz eklentiler</a>, gözden geçirilir ve incelemeyi geçtikten sonra&nbsp; kullanıcılara uygun hale gelir. Eklentiler AMO'ya gönderilmek zorunda değildir, ama gönderilirse, kullanıcılar gözden geçirilmiş eklentilere güvenebilirler ve kullanışlı eklentiler için bir kaynak olan AMO görünürlüğünden faydalanabilirsiniz.</p>

<p>Eklentiler, onları barındıran uygulamanın davranışını büyük ölçüden etkileyebilirler. Bu sebeple eklentilerin, kullanıcılara iyi bir deneyim sağlamasına yardım etmek için <a href="/en-US/docs/Mozilla/Add-ons/Add-on_guidelines">kuralları</a> geliştirdik.Bu kurallar, eklenti <a href="https://addons.mozilla.org/">addons.mozilla.org</a>'da barındırılsın ya da barındırlmasın, bütün eklentiler için geçerlidir.</p>

<hr />
<h2 id="Uzantılar_2"><a id="Uzantılar" name="Uzantılar">Uzantılar</a></h2>

<p>Uzantılar, Firefox ve Thunderbird gibi Mozilla uygulamarına yeni fonksiyonellikler eklerler. Sekmeleri yönetmek için farklı bir yol gibi yeni özellikler ekleyebilir veya belirli web sitelerinin kullanılabilirliğini ve güvenliğini atırmak için web içeriğini değiştirebilirler.</p>

<p>Uzantıları yaratabileceğiniz üç farklı teknik vardır: Add-on SDK-tabanlı uzantılar, manüel olarak önyüklenmiş yeniden başlatma gerektirmeyen uzantılar, legacy uzantılar.</p>

<ul class="card-grid">
 <li><span><a href="https://developer.mozilla.org/en-US/Add-ons/SDK">Add-on SDK uzantıları</a></span><br />
  Yüksek seviyede bir dizi JavaScript API'leri kullanılarak inşa edilirler. Yüklenmeleri için tarayıcının yeniden başlatılmasına gerek yoktur.</li>
 <li><span><a href="/en-US/Add-ons/Bootstrapped_extensions">Yeniden başlatma gerektirmeyen uzantılar</a></span><br />
  Yüklenmeleri için tarayıcının yeniden başlatılmasına gerek olmayan uzantılardır.</li>
 <li><a href="/en-US/Add-ons/Overlay_Extensions"><span>Legacy extensions</span></a><br />
  Legacy uzantılar yüklenirken tarayıcının yeniden başlatılmasına ihtiyaç duyarlar, genelde <a href="/en-US/docs/Mozilla/Tech/XUL/Overlays">XUL overlays</a> kullanılır.</li>
</ul>

<div class="note">
<p><strong>WebExtensions</strong></p>

<p>Biz, WebExtensions olarak adlandırılan ve Firefox için ve aynı zaman Google ve Opera tarafından kullanılanılan sistemlerle büyük ölçüde uyumlu olacak, eklenti geliştirmenin yeni bir yolu olan bir sistem üzerinde çalışıyoruz.</p>

<p>Gelecekte, Firefox için tercih edilen bir uygulama geliştirme yolu olacaktır.</p>

<p>Şu anda bu uygulama deneyseldir, ama yine de bir göz atmak isterseniz <a href="https://developer.mozilla.org/en-US/Add-ons/WebExtensions">see the docs here</a> bağlantısından dökümanlara ulaşabilirsiniz.</p>
</div>

<p>Eğer yapabiliyorsanız, yeniden başlatma gerektirmeyen mekanızmayı kullanan Add-on SDK-tabanlı tekniği kullanmak uygundur, eğer bu teknik sizin ihtiyacınız için yeterli değilse, manuel olanı, JavaScript API'leri kullanmayan ikinci yöntemi uygulayın.</p>

<p>Teknik seçiminde daha fazla bilgi için, okuyun <a href="/en-US/Add-ons/Comparing_Extension_Toolchains">comparison</a>.</p>

<h3 id="Hata_ayıklama">Hata ayıklama</h3>

<p>Eklenti geliştirmede, hangi satırlarda hatalar yapıldığını görmek hata ayıklama olmadan mümkün değildir. Masaüstü için <a href="/en-US/Add-ons/Overlay_Extensions/XUL_School/Setting_Up_a_Development_Environment">Setting Up a Development Environment</a>, mobil için(Android/iOS) <a href="/en-US/docs/Tools/Remote_Debugging/Debugging_Firefox_for_Android_with_WebIDE">Debugging Firefox for Android with WebIDE</a> 'ya göz atın. Mobil cihazlarda meydana gelen hataları yakalamak için masaüstü tarayıcı araçlarından WebIDE kullanılır.</p>

<div class="column-container">
<div class="column-half">
<h3 id="Önerilen_Pratikler">Önerilen Pratikler</h3>

<p>Uzantınızı hangi teknikle geliştirdiğinizin önemi olmamasına rağmen,&nbsp;mümkün olduğunca iyi bir kullanıcı deneyimi sağlaması için birkaç yönerge vardır.</p>

<dl>
 <dt><a href="/en-US/Add-ons/Performance_best_practices_in_extensions">Performans</a></dt>
 <dd>Uzantınızın hızlı, duyarlı ve bellek-tasarruflu olmasını sağlamak için.</dd>
 <dt><a href="/en-US/Add-ons/Security_best_practices_in_extensions">Güvenlik</a></dt>
 <dd>Zararlı web sitelerinin uzantınızı etkisi altına almamasını sağlamak için.</dd>
 <dt><a href="/en-US/Add-ons/Extension_etiquette">Etiquette</a></dt>
 <dd>uzantınızın diğer uzantılar ile uyum içerisinde çalışması için.</dd>
</dl>
</div>

<div class="column-half">
<h3 id="Uygulama_Özel">Uygulama Özel</h3>

<p>Çoğu dokümantasyon, masaüstü Firefox için geliştirme yapıyor olduğunuz varsayar. Eğer diğer bir Gecko tabanlı uygulama için geliştirme yapıyorsanız, bilmeniz gereken başlıca farklılıklar vardır.</p>

<dl>
 <dt><a href="/en-US/Add-ons/Thunderbird">Thunderbird</a></dt>
 <dd>Thunderbird mail istemcisi için uzantılar geliştirmek için.</dd>
 <dt><a href="/en-US/Add-ons/Firefox_for_Android">Firefox Android</a></dt>
 <dd>Firefox Android için uzantılar geliştirmek için.</dd>
 <dt><a href="/en-US/Add-ons/SeaMonkey_2">SeaMonkey</a></dt>
 <dd><a href="http://www.seamonkey-project.org/">SeaMonkey</a> yazılım takımı için uzantılar geliştirmek için.</dd>
</dl>
</div>
</div>

<hr />
<h2 id="Temalar"><a name="Themes">Temalar</a></h2>

<p>Temalar, kullanıcı arayüzünü ihtiyaca göre düzenleyebileceğiniz eklentilerdir. İki çeşit tema vardır: <a href="/Add-ons/Themes/Background">Lightweight </a>temalar ve<a href="/en-US/docs/Themes"> complete </a>temalar.</p>

<div class="column-container">
<div class="column-half">
<p><a href="/Add-ons/Themes/Background">Lightweight temalar</a>, diğerine göre uygulanması daha basittir, fakat sağladığı düzenleme alanı çok limitlidir.</p>
</div>

<div class="column-half">
<p><a href="/en-US/docs/Themes">Complete temalar</a> ile kullanıcı arayüzünde daha derin modifikasyonlar yapabilirsiniz. Complete temaların dökümantasyonu güncel değildir, ancak olası güncelleştirmeler aynı linke bağlıdır.</p>
</div>
</div>

<hr />
<h2 id="Diğer_çeşit_eklentiler">Diğer çeşit eklentiler</h2>

<p><a href="/en-US/docs/Creating_OpenSearch_plugins_for_Firefox">Search engine plugins</a> basit ve özel bir çeşit eklenti tipidir: arama alanına yeni bir arama motoru eklerler.</p>

<p><strong><a href="/en-US/docs/Plugins">Plugins</a> </strong>help the application understand web content that it does not natively support. NPAPI plugins are a legacy technology and new sites should not use them. In general, plugins are not available on most modern mobile systems including, and websites should transition away from using plugins.</p>

<hr />
<p>{{CommunityBox("extension development", "dev-extensions", "mozilla.dev.extensions", "extdev","Add-ons forums|https://forums.mozilla.org/addons/viewforum.php?f=3|discussion and support|Visit the add-ons forums||AMO|https://addons.mozilla.org/en-US/firefox/|addons.mozilla.org|Visit addons.mozilla.org")}}</p>

<h2 id="Subnav">Subnav</h2>

<ol>
 <li><a href="/en-US/Add-ons/Bootstrapped_extensions" title="Restartless extensions">Restartless extensions</a></li>
 <li><a href="/en-US/Add-ons/Overlay_Extensions" title="Legacy extensions">Legacy extensions</a></li>
 <li><a href="/en-US/Add-ons/SDK">Add-on SDK</a>{{AddonSDKSubnav}}</li>
 <li><a href="#">Techniques</a>
  <ol>
   <li><a href="/en-US/Add-ons/Techniques/Promises">Promises</a></li>
  </ol>
 </li>
 <li><a href="#">Recommended practices</a>
  <ol>
   <li><a href="/en-US/Add-ons/Performance_best_practices_in_extensions" title="Performance">Performance</a></li>
   <li><a href="/en-US/Add-ons/Security_best_practices_in_extensions" title="Security">Security</a></li>
   <li><a href="/en-US/Add-ons/Extension_etiquette" title="Etiquette">Etiquette</a></li>
  </ol>
 </li>
 <li><a href="#">Themes</a>
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
   <li><a href="/en-US/docs/Plugins/Guide/Streams">Streams</a></li>
   <li><a href="/en-US/docs/Plugins/Guide/URLs">URLs</a></li>
   <li><a href="/en-US/docs/Plugins/Guide/Memory">Memory</a></li>
   <li><a href="/en-US/docs/Plugins/Guide/Version%2C_UI%2C_and_Status_Information">Version, UI, and Status Information</a></li>
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
   <li><a href="/en-US/docs/Plugins/Guide/Structures">Structures</a></li>
   <li><a href="/en-US/docs/Plugins/Guide/Constants">Constants</a></li>
   <li><a href="/en-US/Add-ons/Plugins/External_resources_for_plugin_creation">External Resources</a></li>
  </ol>
 </li>
 <li><a href="#">Publishing add-ons</a>
  <ol>
   <li><a href="/en-US/Add-ons/Distribution">Signing and distributing your add-on</a></li>
   <li><a href="https://addons.mozilla.org/developers/addon/submit/">Submit a new add-on</a></li>
   <li><a href="/en-US/Add-ons/AMO/Policy">Policies</a>
    <ol>
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
   <li><a href="https://forums.mozilla.org/addons">Add-on Forums</a></li>
   <li><a href="http://stackoverflow.com/questions/tagged/firefox-addon">Stack Overflow</a></li>
   <li><a href="https://groups.google.com/forum/#!forum/mozilla.dev.extensions">Development Newsgroup</a></li>
   <li><a href="irc://irc.mozilla.org/extdev">IRC Channel</a></li>
  </ol>
 </li>
</ol>

