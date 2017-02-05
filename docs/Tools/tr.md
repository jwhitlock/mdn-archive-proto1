---
version: prototype1
revision_id: 1182811
locale: tr
slug: Araclar
tags: "firefox aurora" "geliştirici araçları"
title: Firefox Geliştirici Araçları
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: True
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<div class="summary">HTML, CSS ve JavaScript'i telefonundan ve masaüstü bilgisayarından&nbsp;incele, düzenle ve ayıkla. Geliştirici araçları son sürümleri için <a href="https://www.mozilla.org/en-US/firefox/developer/">Firefox Gelistirici Sürümü'nü indir</a>.
<p>&nbsp;</p>
</div>

<div class="column-container zone-callout">
<h3 id="Aurora'_da_neler_yeni"><a href="https://hacks.mozilla.org/2013/11/firefox-developer-tools-episode-27-edit-as-html-codemirror-more/" title="Aurora Hacks post">Aurora' da neler yeni?</a></h3>
Son <a href="http://www.mozilla.org/en-US/firefox/aurora/" title="http://www.mozilla.org/en-US/firefox/aurora/">Firefox Aurora dağıtımı</a> Firefox 27' dir, ve geliştirici araçları için bu güncellemeleri içerir:

<ul>
 <li><a href="/en-US/docs/Tools/Shader_Editor">Shader Editor</a>, WebGL shader'larını görmenizi ve değiştirmenizi sağlar</li>
 <li>Debugger'ı dinlediğiniz <a href="/en-US/docs/Tools/Debugger#Break_on_a_DOM_event">DOM olaylarında durması</a> için talimat verin</li>
 <li><a href="/en-US/docs/Tools/Page_Inspector#Editing_HTML">Denetçide HTML'yi&nbsp;değiştirin</a></li>
 <li>Denetçinin <a href="/en-US/docs/Tools/Page_Inspector#Rules_view">Kurallar Sekmasinde</a>,&nbsp;renk paletlerini ve arkaplanları görün</li>
 <li>The Web Console now <a href="/en-US/docs/Tools/Web_Console#Reflow_events">logs reflow events</a></li>
 <li>Kod Görüntüleyici &nbsp;şimdi&nbsp;çoğu araçta kaynak editörü olarak kullanılmakta</li>
</ul>
</div>

<div class="column-container">
<p><img alt="" src="https://mdn.mozillademos.org/files/6111/debugger-800.png" style="display:block; height:360px; margin-left:auto; margin-right:auto; width:800px" /><span class="seoSummary">Firefox Geliştirici Araçları'nı <a href="/en-US/docs/Tools/Page_Inspector" title="/en-US/docs/Tools/Page_Inspector">HTML and CSS'i incelemek ve düzenlemek</a>, <a href="/en-US/docs/Tools/Debugger" title="/en-US/docs/Tools/Debugger">JavaScript'te</a> hata ayıklamak ve sayfa içinde <a href="/en-US/docs/Tools/Web_Console#The_command_line_interpreter" title="/en-US/docs/Tools/Web_Console#The_command_line_interpreter">JavaScript'i çalıştırmak</a> için kullanabilirsiniz. Bir sayfayı yüklerken tarayıcınızın karşılaştığı JavaScript ve CSS uyarı ve hatalarını görebilmeye ek olarak, ağ isteklerini görmek için de bu geliştirici araçlarını kullanabilirsiniz.&nbsp;</span></p>

<p>You can use the developer tools to <a href="/en-US/docs/Tools/Remote_Debugging" title="/en-US/docs/Tools/Remote_Debugging">debug code running Firefox for Android</a>, and soon, Firefox OS. We've also provided tools that target mobile development: the <a href="/en-US/docs/Tools/Responsive_Design_View" title="/en-US/docs/Tools/Responsive_Design_View">Responsive Design View</a> is a quick way to see how a site will look on a small screen, and the <a href="/en-US/docs/Tools/Firefox_OS_Simulator" title="/en-US/docs/https://developer.mozilla.org/en-US/docs/Tools/Firefox_OS_Simulator">Firefox OS Simulator</a> lets you run and debug a Firefox OS app on the desktop without needing to use a real Firefox OS device.</p>

<p>Firefox add-ons can access the debugger API, so you can build your own developer tools that extend and enhance the built-in tools. With the <a href="https://wiki.mozilla.org/Remote_Debugging_Protocol" title="https://wiki.mozilla.org/Remote_Debugging_Protocol">remote debugging protocol</a> you can implement your own debugging clients and servers, enabling you to debug websites using your own tools or to debug different targets using the Firefox tools.</p>
</div>

<hr />
<div class="column-container">
<div class="column-third">
<h2 id="Tools" name="Tools">Araç Kutusu</h2>

<p><a href="/en-US/docs/Tools/Toolbox" title="/en-US/docs/Tools/Toolbox">Araç Kutusu</a>,&nbsp;Firefox içindeki tüm Geliştirici Araçları'nı tek çatı altına toplamayı sağlamaktadır.</p>

<dl>
 <dt><a href="/en-US/docs/Tools/Page_Inspector" title="Tools/Page_Inspector">Sayfa Denetçisi</a></dt>
 <dd>Görünüm ve seçili öğe için HTML ve CSS ayarları.</dd>
 <dt><a href="/en-US/docs/Tools/Web_Console" title="Tools/Web_Console">Web Konsolu </a></dt>
 <dd>Web sayfası yükleyen browser tarafından gönderilen bilgi, uyarı ve hata mesajlarını görün, ve JavaScript kullanarak sayfayı inceleyin ve degiştirin.</dd>
 <dt><a href="/en-US/docs/Tools/Style_Editor" title="Tools/Style_Editor">Biçim Editörü</a></dt>
 <dd>Sayfanızdaki CSS ayarlarını görün ve düzenleyin.</dd>
 <dt><a href="/en-US/docs/Tools/Debugger" title="Tools/Debugger">JavaScript Debugger</a></dt>
 <dd>Browserda calışan JavaScript kodunu inceleyin ve değişkenleri takip ederek kodunuzu debug edin.</dd>
 <dt><a href="/en-US/docs/Tools/Profiler" title="Tools/Profiler">JavaScript Profiler</a></dt>
 <dd>Profiler'ı kullanarak JavaScript'inizin vaktini nerede harcadığını anlayın.</dd>
 <dt><a href="/en-US/docs/Tools/Network_Monitor" title="Tools/Network_Monitor">Ağ izleyici</a></dt>
 <dd>Bir sayfa yüklendiğinde gerçekleşen bütün ağ taleplerini ve ne kadar süre aldıklarını inceleyin.</dd>
 <dt><a href="/en-US/docs/Tools/Shader_Editor">Shader Editor</a></dt>
 <dd>View and edit the vertex and fragment shaders used by <a href="https://developer.mozilla.org/en-US/docs/Web/WebGL">WebGL</a>.</dd>
</dl>
</div>

<div class="column-third">
<h2 id="Mobil">Mobil</h2>

<p>Elbette mobil web geliştiricileri de web geliştiricileridir. Bu nedenle wen geliştirme araçlarının çoğunun mobil wen geliştiricilerini de ilgilendiriyor.Fakat sadece mobil geliştirmeyi hedefleyen bazı araçlar da hazırladık.</p>

<dl>
 <dt><a href="/en-US/docs/Tools/Remote_Debugging" title="Tools/Remote_Debugging">Uzaktan Hata Ayıklama</a></dt>
 <dd>Android cihazında USB üzerinden hata ayıklamak için geliştirici araçlarını kullanın.</dd>
 <dt><a href="/en-US/docs/Tools/Firefox_OS_Simulator" title="Tools/Firefox_OS_Simulator">Firefox OS Simülatör</a></dt>
 <dd>Gerçek bir Firefox OS cihazı kullanmanıza gerek kalmadan masaüstünde Firefox OS uygulamanızı çalıştırın ve hata ayıklayın.</dd>
 <dt><a href="/en-us/docs/Tools/Responsive_Design_View" title="/en-us/docs/Tools/Responsive_Design_View">Responsive Tasarım Görünümü</a></dt>
 <dd>Tarayıcı pencerenizin boyutunu değiştirmeden web sitenizin veya uygulamanızın farklı ekran boyutlarında nasıl görüneceğini görün..</dd>
</dl>
</div>

<div class="column-third">
<h2 id="Bağımsız_Araçlar">Bağımsız Araçlar</h2>

<p>Bu araçlar Firefox'a dahil edilebilir, ama kullanıcı arayüzleri (GUI) Araç Kutusu'na entegre edilemezler.</p>

<dl>
 <dt><a href="/en-US/docs/Tools/Scratchpad" title="Tools/Scratchpad">Scratchpad</a></dt>
 <dd>A text editor built into Firefox that lets you write and execute JavaScript.</dd>
 <dt><a href="/en-us/docs/Tools/Browser_Console" title="/en-us/docs/Tools/Responsive_Design_View">Browser Console</a></dt>
 <dd>See messages from all JavaScript code running in the browser including content, chrome, and add-ons. Execute JavaScript code in the chrome window's context.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Tools/GCLI" title="en/Tools/GCLI">Developer Toolbar</a></dt>
 <dd>A command-line interface to manipulate and work with the developer tools in Firefox, and buttons for quick access to the most commonly used tools.</dd>
 <dt><a href="/en-US/docs/Tools/3D_View" title="Tools/3D_View">3D View</a></dt>
 <dd>Also known as "Tilt", this provides a 3D visualisation of the current page.</dd>
 <dt><a href="/en-US/docs/Tools/Paint_Flashing_Tool" title="Tools/Paint_Flashing_Tool">Paint Flashing Tool</a></dt>
 <dd>The paint flashing tool highlights the part of the browser window that are repainted in response to events, helping to diagnose potential performance problems with your site.</dd>
</dl>
</div>
</div>

<hr />
<h2 id="Diğer_Kaynaklar">Diğer Kaynaklar</h2>

<p>This section lists resources which aren't maintained by Mozilla's developer tools team, but which are widely used by web developers. We've included a few Firefox add-ons in this list, but for the complete list see the <a href="https://addons.mozilla.org/en-US/firefox/extensions/web-development/" title="https://addons.mozilla.org/en-US/firefox/extensions/web-development/">"Web Development" category on addons.mozilla.org</a>.</p>

<dl>
 <dt><a href="https://www.getfirebug.com/" title="Firebug">Firebug</a></dt>
 <dd>A very popular and powerful web development tool, including a JavaScript debugger, HTML and CSS viewer and editor, and network monitor.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/DOM_Inspector" title="DOM_Inspector">DOM Ayıklayıcı</a></dt>
 <dd>Inspect, browse, and edit the DOM of web pages or XUL windows.</dd>
 <dt><a href="https://addons.mozilla.org/en-US/firefox/addon/web-developer/" title="Web-Developer">Web Geliştirici</a></dt>
 <dd>Adds a menu and a toolbar to the browser with various web developer tools.</dd>
 <dt><a href="https://webmaker.org/en-US/tools/" title="https://webmaker.org/en-US/tools/">Web Tasarım&nbsp;Aracı</a></dt>
 <dd>A set of tools developed by Mozilla, aimed at people getting started with Web development.</dd>
 <dt><a href="http://www.w3.org/Status.html" title="W3C">W3C Doğrulayıcı</a></dt>
 <dd>The W3C website hosts a number of tools to check the validity of your website, including its <a href="http://validator.w3.org/" title="http://validator.w3.org/">HTML</a> and <a href="http://jigsaw.w3.org/css-validator/" title="http://jigsaw.w3.org/css-validator/">CSS</a>.</dd>
 <dt><a href="http://www.jshint.com/" title="JSHint">JSHint</a></dt>
 <dd>JavaScript kod analiz aracı</dd>
</dl>

<hr />
<p>{{CommunityBox("Developer tools", "dev-developer-tools", "mozilla.dev.developer-tools", "devtools", "Team info|https://wiki.mozilla.org/DevTools|Dev tools wiki|Designs and plans for the dev tools||Blog|https://hacks.mozilla.org/|Hacks blog|Hacks blog", "FirefoxDevTools", "firefox-developer-tools")}}</p>

<h2 id="Alt_Başlıklar">Alt Başlıklar</h2>

<ol>
 <li><a href="/en-US/docs/Tools/Toolbox">Araç Kutusu</a>

  <ol>
   <li><a href="/en-US/docs/Tools/Page_Inspector" title="Tools/Page_Inspector">Sayfa Denetçisi</a></li>
   <li><a href="/en-US/docs/Tools/Web_Console" title="Web Console">Web Konsolu</a></li>
   <li><a href="/en-US/docs/Tools/Style_Editor" title="Style Editor">Biçim Editörü</a></li>
   <li><a href="/en-US/docs/Tools/Debugger" title="Debugger">Debugger</a></li>
   <li><a href="/en-US/docs/Tools/Profiler" title="Profiler">Profiler</a></li>
   <li><a href="/en-US/docs/Tools/Network_Monitor" title="Network Monitor">Ağ izleyici</a></li>
   <li><a href="/en-US/docs/Tools/Shader_Editor">Shader Editor</a></li>
  </ol>
 </li>
 <li><a href="#">Mobile</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Remote_Debugging" title="Remote Debugging">Remote Debugging</a></li>
   <li><a href="/en-US/docs/Tools/Firefox_OS_Simulator" title="Firefox OS Simulator">Firefox OS Simulator</a></li>
   <li><a href="/en-US/docs/Tools/Responsive_Design_View" title="Responsive Design View">Responsive Design View</a></li>
  </ol>
 </li>
 <li><a href="#">Standalone tools</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Scratchpad" title="Scratchpad">Scratchpad</a></li>
   <li><a href="/en-US/docs/Tools/Browser_Console" title="Browser Console">Browser Console</a></li>
   <li><a href="/en-US/docs/Tools/GCLI" title="GCLI">Developer Toolbar</a></li>
   <li><a href="/en-US/docs/Tools/3D_View" title="3D View">3D View</a></li>
   <li><a href="/en-US/docs/Tools/Paint_Flashing_Tool" title="Paint Flashing Tool">Paint Flashing Tool</a></li>
   <li><a href="/en-US/docs/Tools/Debugging_Firefox_JS_Code" title="Debugging Firefox JS code">Debugging Firefox JS Code</a></li>
  </ol>
 </li>
</ol>

<p>&nbsp;</p>

<p>&nbsp;</p>

