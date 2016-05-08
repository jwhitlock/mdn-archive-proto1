---
version: prototype1
revision_id: 1056668
locale: id
slug: Mozilla/Add-ons
tags: 
title: Add-ons
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>{{AddonSidebar}}</p>

<p><span class="seoSummary">Add-ons Menambah fungsi baru pada aplikasi berbasis <span class="seoSummary"><a href="https://developer.mozilla.org/en-US/docs/Mozilla/Gecko">Gecko</a></span> seperti Firefox, SeaMonkey dan Thunderbird. Ada dua jenis "add-on" :&nbsp; <a href="/en-US/docs/Extensions" title="Extensions">Extensions</a> menambahkan fitur ke aplikasi, sedangkan <a href="https://developer.mozilla.org/id/docs/Mozilla/Add-ons$edit#Themes">Tema</a> merubah tampilan pada aplikasi.</span></p>

<p>Keduanya (Extention, dan Tema) ditemukan dalam <a href="https://addons.mozilla.org/">addons.mozilla.org</a>, dikenal juga sebagai AMO. Ketika Anda <a href="https://developer.mozilla.org/en-US/Add-ons/Submitting_an_add-on_to_AMO">masukan add-ons ke AMO</a> mereka meninjau, dan setelah melewati tinjauan maka mereka menyajikan untuk pengguna. Anda tidak harus masukan add-on ke AMO, tetapi anda lakukan, <span id="result_box" lang="id"><span class="hps">pengguna dapat</span> <span class="hps">menaruh keyakinan </span><span class="hps">bahwa</span> <span class="hps">mereka</span> <span class="hps">telah ditinjau</span></span>, dan Anda dapat keuntungan dari visibilitas AMO sebagai sumber add-on yang berguna.</p>

<p><span id="result_box" lang="id"><span class="atn hps">Add-</span><span>ons</span> <span class="hps">dapat </span><span class="hps">mempengaruhi perilaku</span> <span class="hps">aplikasi</span> <span class="hps">host</span> <span class="hps">mereka</span></span>. Kami telah membangun <a href="https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/Add-on_guidelines">sekumpulan panduan</a> untuk membantu memastikan bahwa mereka telah didukung mendapatkan pengalaman yang baik pada pengguna. Panduan ini digunakan untuk beberapa add-on, apakah mereka juga ditaruh di <a href="https://addons.mozilla.org/">addons.mozilla.org</a> atau tidak.</p>

<h2 id="Extentions"><strong>Extentions</strong></h2>

<p>Extention menambah fungsi dari aplikasi Mozzila seperti Firefox dan Thunderbird. Extension dapat menambahkan fitur pada peramban, seperti mengatur tab, dan mereka dapat merubah konten web untuk meningkatkan pengguanan atau keamanan website tertentu.</p>

<table class="topicpage-table">
 <tbody>
  <tr>
   <td>
    <h2 class="Documentation" id="Documentation" name="Documentation">Dokumentasi</h2>

    <dl>
     <dt><a href="/en-US/docs/Addons/Add-on_Manager" title="Addons/Add-on Manager">Pengatur Add-on</a> {{gecko_minversion_inline("2.0")}}</dt>
     <dd>Cara penggunaan pengatur add-on.</dd>
     <dt><a href="/en-US/docs/Addons/Add-on_Repository" title="Addons/Add-on Repository">Add-on Repository</a> {{gecko_minversion_inline("2.0")}}</dt>
     <dd>Digunakan untuk menemukan add-on yang tersedia.</dd>
     <dt><a href="/en-US/docs/Addons/Interfacing_with_the_Add-on_Repository" title="Addons/Interfacing with the Add-on Repository">Interfacing with the Add-on Repository</a> {{gecko_minversion_inline("2.0")}}</dt>
     <dd><span class="highlight" id="ouHighlight__0_2TO0_3">Cara</span><span id="noHighlight_0.7364044648261486"> </span><span id="ouHighlight__7_9TO5_15">menggunakan</span><span id="noHighlight_0.001846948547626459"> </span><span id="ouHighlight__40_45TO17_21">modul</span><span id="noHighlight_0.4932221761846922"> </span><span id="ouHighlight__35_38TO23_26">kode</span><span id="noHighlight_0.9540285744766477"> </span><a href="/en-US/docs/Addons/Add-on_Repository" title="Addons/Add-on Repository"><code>AddonRepository.jsm</code></a> <span id="ouHighlight__47_48TO48_52">untuk</span><span id="noHighlight_0.4852050260631776"> </span><span id="ouHighlight__50_57TO54_65">berinteraksi</span><span id="noHighlight_0.665524408684204"> </span><span id="ouHighlight__59_62TO67_72">dengan</span><span id="noHighlight_0.556821336906181"> </span><span id="ouHighlight__64_66TO74_76">AMO</span><span id="noHighlight_0.2763824148884182">.</span></dd>
     <dt><a href="/en-US/docs/Addons/Working_with_AMO" title="Addons/Working with AMO">Bekerja Dengan AMO</a> {{gecko_minversion_inline("2.0")}}</dt>
     <dd><span id="ouHighlight__0_3TO0_3">Tips</span><span id="noHighlight_0.5688039621440252"> </span><span id="ouHighlight__5_7TO5_7">dan</span><span id="noHighlight_0.8537482918984186"> </span><span id="ouHighlight__9_19TO9_13">saran</span><span id="noHighlight_0.19901144251963665"> </span><span id="ouHighlight__21_23TO15_19">untuk</span><span id="noHighlight_0.8077123763815125"> </span><span id="ouHighlight__32_35TO26_32">membuat</span><span id="noHighlight_0.9422548028427585"> </span><span id="ouHighlight__42_47TO39_45">Pengaya Anda</span><span id="noHighlight_0.2792045518505175"> </span><span class="highlight" id="ouHighlight__49_52TO52_58">bekerja</span><span id="noHighlight_0.3565413615066263"> </span><span id="ouHighlight__54_57TO60_65">dengan</span><span id="noHighlight_0.7838500768179173"> </span><span id="ouHighlight__82_91TO67_76">repositori</span> <a class="external" href="http://addons.mozilla.org" title="http://addons.mozilla.org/">addons.mozilla.org</a> .</dd>
     <dt><a href="/en-US/docs/Extensions" title="Extensions">Extensions</a></dt>
     <dd>
     <div class="Wrap" id="OutputText" style="direction: ltr; text-align: left;" tabindex="99999">
     <div><span id="ouHighlight__0_10TO0_8">Informasi</span><span id="noHighlight_0.3428004874881513"> </span><span id="ouHighlight__12_16TO10_16">tentang</span><span id="noHighlight_0.11819473220936372"> </span><span id="ouHighlight__18_27TO18_30">mengembangkan</span><span id="noHighlight_0.8155911046397254"> </span><span id="ouHighlight__29_38TO32_39">ekstensi</span><span id="noHighlight_0.4256537437293869"> </span><span id="ouHighlight__40_42TO41_45">untuk</span><span id="noHighlight_0.25349153498185173"> </span><span class="highlight" id="ouHighlight__44_50TO47_53">aplikasi Mozilla</span><span id="noHighlight_0.7308544285843325">.</span></div>
     </div>
     </dd>
     <dt><a href="/en-US/docs/Addons/Add-on_guidelines" title="/en-US/docs/Addons/Add-on_guidelines">Panduan Add-on</a></dt>
     <dd>
     <div class="Wrap" id="OutputText" style="direction: ltr; text-align: left;" tabindex="99999">
     <div><span id="ouHighlight__0_9TO0_6">Pedoman</span><span id="noHighlight_0.6590539411012253"> </span><span id="ouHighlight__11_13TO8_12">untuk</span><span id="noHighlight_0.6389256313956393"> </span><span id="ouHighlight__15_22TO14_24">menciptakan</span><span id="noHighlight_0.49781949370259526"> </span><span id="ouHighlight__30_36TO26_32">Pengaya</span><span id="noHighlight_0.3398709708800992"> </span><span id="ouHighlight__24_28TO34_38">yang baik</span><span id="noHighlight_0.4182708173806071"> !</span></div>
     </div>
     </dd>
     <dt><a href="/en-US/docs/Plugins" title="Plugins">Plugins</a></dt>
     <dd>
     <div class="Wrap" id="OutputText" style="direction: ltr; text-align: left;" tabindex="99999">
     <div><span id="ouHighlight__0_2TO0_8">Bagaimana</span><span id="noHighlight_0.6472528681404855"> </span><span id="ouHighlight__7_13TO10_22">mengembangkan</span><span id="noHighlight_0.30412433136699624"> </span><span id="ouHighlight__15_21TO24_29">plugin</span><span id="noHighlight_0.4990728745365166">.</span></div>
     </div>
     </dd>
     <dt><a href="/en-US/docs/Themes" title="Themes">Tema</a></dt>
     <dd>
     <div class="Wrap" id="OutputText" style="direction: ltr; text-align: left;" tabindex="99999">
     <div><span class="highlight" id="ouHighlight__0_9TO0_12">Mengembangkan</span><span id="noHighlight_0.11519698699943359"> </span><span id="ouHighlight__11_16TO14_17">tema</span><span id="noHighlight_0.5555241600438355"> </span><span id="ouHighlight__18_20TO19_23">(atau</span><span id="noHighlight_0.8368830349360896"> </span><span id="ouHighlight__22_27TO25_30">kulit)</span><span id="noHighlight_0.4067025365491751"> </span><span id="ouHighlight__29_31TO32_36">untuk</span><span id="noHighlight_0.39512781563838784"> </span><span id="ouHighlight__41_52TO38_45">aplikasi</span><span id="noHighlight_0.5647933115923259"> </span><span id="ouHighlight__33_39TO47_53">Mozilla</span><span id="noHighlight_0.6020125936090621">.</span></div>
     </div>
     </dd>
     <dt><a href="/en-US/docs/Creating_OpenSearch_plugins_for_Firefox" title="Creating OpenSearch plugins for Firefox">Mencipatakn OpenSearch plugin untuk Firefox</a></dt>
     <dd>
     <div class="Wrap" id="OutputText" style="direction: ltr; text-align: left;" tabindex="99999">
     <div><span id="ouHighlight__0_2TO0_8">Bagaimana</span><span id="noHighlight_0.9244053394814954"> </span><span id="ouHighlight__7_13TO10_22">mengembangkan</span><span id="noHighlight_0.18163457858436738"> </span><span id="ouHighlight__22_29TO34_40">plug-in</span><span id="noHighlight_0.14261229836676825"> <span id="ouHighlight__15_20TO24_32">pencarian</span><span id="noHighlight_0.401744621711146"> </span></span><span id="ouHighlight__31_33TO42_46">untuk</span><span id="noHighlight_0.506226934679552"> </span><span id="ouHighlight__35_41TO48_54">Firefox</span><span id="noHighlight_0.5675475350044076">.</span></div>
     </div>
     </dd>
     <dt><a href="/en-US/docs/Performance" title="Performance">Kinerja</a></dt>
     <dd>
     <div class="Wrap" id="OutputText" style="direction: ltr; text-align: left;" tabindex="99999">
     <div><span id="ouHighlight__12_17TO8_14">Panduan<span id="ouHighlight__0_10TO0_6"> Kinerja</span><span id="noHighlight_0.12694588280522112"> </span></span><span id="noHighlight_0.8703026364660557"> </span><span id="ouHighlight__19_21TO16_18">dan</span><span id="noHighlight_0.4729487174206325"> </span><span id="ouHighlight__23_31TO20_27">utilitas</span><span id="noHighlight_0.015512705349606914"> </span><span id="ouHighlight__33_34TO29_33">untuk</span><span id="noHighlight_0.5004067064811378"> </span><span id="ouHighlight__36_39TO35_42">membantu</span><span id="noHighlight_0.8801185084261491"> </span><span class="highlight" id="ouHighlight__45_48TO49_55">membuat</span><span id="noHighlight_0.5591527696637159"> </span><span id="ouHighlight__55_60TO62_68">Pengaya</span><span id="noHighlight_0.6943106412637858"> Anda </span><span id="ouHighlight__62_68TO75_80">tampil</span><span id="noHighlight_0.43777089662123225"> </span><span id="ouHighlight__70_73TO82_85">baik</span><span id="noHighlight_0.4751778868965798"> </span><span id="ouHighlight__75_78TO87_90">(dan</span><span id="noHighlight_0.599402277603739"> </span><span id="ouHighlight__83_86TO92_98">bermain</span><span id="noHighlight_0.6972850158580534"> </span><span id="ouHighlight__88_93TO100_103">baik</span><span id="noHighlight_0.05900018779569882"> </span><span id="ouHighlight__95_98TO105_110">dengan</span><span id="noHighlight_0.07123670734596044"> </span><span id="ouHighlight__100_107TO112_123">orang lain).</span></div>
     </div>
     </dd>
    </dl>

    <p><span class="alllinks"><a href="/en-US/docs/tag/Add-ons" title="tag/Add-ons">Lihat Semua halaman dengan tag "Add-ons"...</a></span></p>
   </td>
   <td>
    <h2 class="Community" id="Community" name="Community"><span id="ouHighlight__0_8TO0_8">Community</span></h2>

    <ul>
     <li><a class="link-irc" href="irc://irc.mozilla.org/extdev">#extdev IRC channel</a></li>
     <li><a class="external" href="http://forums.mozillazine.org/?c=11">MozillaZine forum</a></li>
     <li><a class="external" href="/devnews/index.php/categories/about-addons" title="https://developer.mozilla.org/editor/fckeditor/core/editor/devnews/index.php/categories/about-addons/">about:addons newsletter</a></li>
     <li><a class="external" href="/web-tech" title="https://developer.mozilla.org/editor/fckeditor/core/editor/web-tech/">Mozilla's Web-Tech blog</a></li>
     <li><a class="external" href="http://mozdev.org/mailman/listinfo/project_owners">mozdev project owners</a></li>
     <li><a class="external" href="http://planet.mozilla.org/" title="http://planet.mozilla.org/">Planet Mozilla</a></li>
     <li><a href="/en-US/docs/Extensions/Community" title="Extensions/Community">Other community links...</a></li>
    </ul>

    <h2 class="Tools" id="Tools" name="Tools">Peralatan</h2>

    <ul>
     <li><a href="/en-US/docs/DOM_Inspector" title="DOM Inspector">DOM Inspector</a> -

      <div class="Wrap" id="OutputText" style="direction: ltr; text-align: left;" tabindex="99999">
      <div><span id="ouHighlight__0_6TO0_8">memeriksa</span><span id="noHighlight_0.2549244811712643"> </span><span id="ouHighlight__8_10TO10_12">DOM</span><span id="noHighlight_0.3038362005870763">,</span><span id="noHighlight_0.15822842773565138"> </span><span id="ouHighlight__13_15TO15_17">CSS</span><span id="noHighlight_0.24713042532913">,</span><span id="noHighlight_0.6033512257824745"> </span><span id="ouHighlight__18_20TO20_22">dan</span><span id="noHighlight_0.9615891268260267"> </span><span id="ouHighlight__22_24TO24_26">XBL</span><span id="noHighlight_0.03690125878487127"> </span><span id="ouHighlight__26_33TO28_35">(Firefox</span><span id="noHighlight_0.507520364077718"> </span><span id="ouHighlight__35_37TO37_39">dan</span><span id="noHighlight_0.4980821444849991"> </span><span id="ouHighlight__39_50TO41_52">Thunderbird)</span></div>
      </div>
     </li>
     <li><a class="external" href="http://www.hacksrus.com/~ginda/venkman/" rel="external nofollow" target="_blank" title="http://www.hacksrus.com/~ginda/venkman/">Venkman</a>, a JavaScript debugger (<a class="external" href="http://addons.mozilla.org/en-US/firefox/addon/216" rel="external nofollow" target="_blank" title="http://addons.mozilla.org/en-US/firefox/addon/216">Firefox</a>, <a class="external" href="http://addons.mozilla.org/en-US/thunderbird/addon/216" rel="external nofollow" target="_blank" title="http://addons.mozilla.org/en-US/thunderbird/addon/216">Thunderbird</a>)</li>
     <li><a class="link-https" href="https://builder.mozillalabs.com/" title="https://builder.mozillalabs.com/">Mozilla Labs Add-on Builder</a></li>
     <li><a class="link-https" href="https://addons.mozilla.org/en-US/firefox/addon/7434/" rel="external nofollow" target="_blank" title="https://addons.mozilla.org/en-US/firefox/addon/7434/">Extension Developer's Extension</a> suite alat pengembang</li>
     <li><a class="external" href="http://www.gijsk.com/" rel="external nofollow" target="_blank" title="http://www.gijsk.com/">Chrome List</a> view files in chrome:// (<a class="external" href="http://addons.mozilla.org/en-US/firefox/addon/4453" rel="external nofollow" target="_blank" title="http://addons.mozilla.org/en-US/firefox/addon/4453">Firefox</a>, <a class="external" href="http://addons.mozilla.org/en-US/thunderbird/addon/4453" rel="external nofollow" target="_blank" title="http://addons.mozilla.org/en-US/thunderbird/addon/4453">Thunderbird</a>)</li>
     <li><a class="external" href="http://ted.mielczarek.org/code/mozilla/extensionwiz/" rel="external nofollow" target="_blank" title="http://ted.mielczarek.org/code/mozilla/extensionwiz/">Extension Wizard</a>
      <div class="Wrap" id="OutputText" style="direction: ltr; text-align: left;" tabindex="99999">
      <div><span class="highlight" id="ouHighlight__12_20TO0_7">ekstensi</span><span id="noHighlight_0.7714346712016384"> </span><span id="ouHighlight__2_10TO9_20">berbasis web<span id="ouHighlight__31_39TO31_39"> generator</span></span><span id="noHighlight_0.7120773680497127"> </span><span id="ouHighlight__22_29TO22_29">kerangka</span><span id="noHighlight_0.9429421167353065"> </span><span id="ouHighlight__41_48TO41_48">(Firefox</span><span id="noHighlight_0.189437415900361"> </span><span id="ouHighlight__50_52TO50_52">dan</span><span id="noHighlight_0.8859653366547199"> </span><span id="ouHighlight__54_65TO54_65">Thunderbird)</span></div>
      </div>
     </li>
    </ul>

    <p>... <a href="/en-US/docs/Setting_up_extension_development_environment#Development_extensions" title="Setting up extension development environment#Development extensions">alat-alat lain</a> ...</p>

    <h2 class="Related_Topics" id="Related_Topics" name="Related_Topics">Topik Terkait</h2>

    <ul>
     <li><a href="/en-US/docs/XUL" title="XUL">XUL</a>, <a href="/en-US/docs/JavaScript" title="JavaScript">JavaScript</a>, <a href="/en-US/docs/XPCOM" title="XPCOM">XPCOM</a>, <a href="/en-US/docs/Themes" title="Themes">Tema</a>, <a href="/en-US/docs/Developer_Guide" title="Developing_Mozilla">Mengembangkan Mozilla</a>, <a href="/en-US/docs/Extensions" title="Extensions">Extensions</a></li>
    </ul>
   </td>
  </tr>
 </tbody>
</table>

<p>&nbsp;</p>

