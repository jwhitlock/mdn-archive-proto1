---
version: prototype1
revision_id: 1056670
locale: id
slug: Tools
tags: "Panduan" "Pengembangan Web : Alat" "Mengembangkan Mozilla"
title: Tools
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>Berikut adalah daftar tools dan resource yang akan membantu dalam proses pengembangan web anda, serta berguna saat debugging add-ons browser Firefox anda.</p>

<h2 id="Pengembangan_Web">Pengembangan Web</h2>

<p>&nbsp;</p>

<h3 id="Integrasi_ke_Firefox">Integrasi ke Firefox</h3>

<p>Tool dan resources yang dibangun kedalam Firefox dan yang dalam pengembangan padat</p>

<dl>
 <dt><a href="/en-US/docs/Tools/Page_Inspector" title="en/Tools/Page_Inspector">Page Inspector</a> {{ fx_minversion_inline("10.0") }}</dt>
 <dd>Sebuah tool yang berguna untuk menampilkan HTML dari elemen yang sedang anda tunjuk dengan mouse pada context</dd>
</dl>

<dl>
 <dt><a href="/en-US/docs/Tools/Web_Console" title="en/Tools/Web_Console">Web Console</a> {{ fx_minversion_inline("4.0") }}</dt>
 <dd>Sebuah konsol yang memungkinkan anda memantau informasi output secara interaktif, menjalankan snippets JavaScripts dan bereksperimen dengan konten anda.</dd>
</dl>

<dl>
 <dt><a href="/en-US/docs/Tools/Scratchpad" title="en/Tools/Scratchpad">Scratchpad</a> {{ fx_minversion_inline("6.0") }}</dt>
 <dd>Editor teks yang dibangun dalam Firefox yang memungkinkan anda mengubah dan menjalankan kode JavaScript.</dd>
 <dt><a href="/en-US/docs/Tools/Style_Editor" title="en/Tools/Style Editor">Style Editor</a> {{ fx_minversion_inline("11.0") }}</dt>
 <dd>Memungkinkan anda mengubah gaya pada halaman yang tampil saat itu secara langsung. Selain itu, anda dapat beralih ke bagian-bagian style lain. Sebuah cara yang fantastis untuk bekerja secara seketika dengan tampilan dan nuansa dari konten web.</dd>
 <dt><a href="/en-US/docs/Tools/Debugger" title="/en-US/docs/Tools/Debugger">JavaScript Debugger</a> {{ fx_minversion_inline("15.0") }}</dt>
 <dd>Langkah melalui kode JavaScript yang berjalan pada browser (atau bahkan pada remote browser!) dan melihat variabel-variabel untuk membantu melacak bugs. Dokumentasi ini juga mencakup Remote Debugger, yang bisa anda gunakan untuk melakukan debug pada kode yang sedang berjalan pada perangkat Sistem Operasi Firefox&nbsp; atau dalam Firefox pada perangkat Android</dd>
 <dt><a href="/en-us/docs/Tools/Responsive_Design_View" title="/en-us/docs/Tools/Responsive_Design_View">Responsive Design View</a> {{ fx_minversion_inline("15.0") }}</dt>
 <dd>Melihat bagaimana desain anda akan tampak pada ukuran layar yang berbeda tanpa mengubah ukuran keseluruhan jendela browser.</dd>
 <dt><a href="/en-US/docs/Tools/Using_the_Source_Editor" title="en/Tools/Using the Source Editor">Using the Source Editor</a></dt>
 <dd>Source Editor bukanlah alat yang berdiri sendiri, malahan, inilah yang mendasari editor yang digunakan Stratchpad dan Style Editor. Artikel berikut memberikan informasi umum pada semua tools yang memanfaatkan <a href="/en-US/docs/JavaScript_code_modules/source-editor.jsm" title="source-editor.jsm">Source Editor API</a>.</dd>
 <dt><a href="/en-US/docs/Tools/GCLI" title="en/Tools/GCLI">Developer Toolbar</a> {{ fx_minversion_inline("16.0") }}</dt>
 <dd>Developer Toolbar memberikan sebuah antarmuka command-line untuk mengontrol dan bekerja dengan alat-alat pengembangan dalam Firefox, dan tombol-tombol kombinasi untuk akses cepat pada tools yang paling umum digunakan.</dd>
</dl>

<h3 id="Extensions" name="Extensions">Ekstensi</h3>

<dl>
 <dt><a class="link-https" href="https://addons.mozilla.org/en-US/firefox/addon/1843">Firebug</a></dt>
 <dd>mengintegrasikan kemudahan dari tool pengembangan untuk melakukan edit, debug, dan pemantau CSS,HTML, dan JavaScript secara langsung pada setiap halaman web (<a class="external" href="http://www.getfirebug.com/">selengkapnya</a>).</dd>
</dl>

<dl>
 <dt><a href="/en-US/docs/DOM_Inspector" title="en/DOM_Inspector">DOM Inspector</a></dt>
 <dd>Sebuah alat pengembangan yang digunakan untuk meneliti, membaca-baca, dan mengubah DOM dari dokumen, biasanya halaman web atau XUL windows.</dd>
</dl>

<dl>
 <dt><a class="link-https" href="https://addons.mozilla.org/en-US/firefox/addon/60">Web Developer</a></dt>
 <dd>Menambahkan menu dan toolbar pada web browser dengan alat pengembangan web yang beragam. (<a class="external" href="http://chrispederick.com/work/web-developer/">selengkapnya</a>)</dd>
</dl>

<dl>
 <dt><a class="link-https" href="https://addons.mozilla.org/en-US/firefox/addon/4111">Aardvark</a></dt>
 <dd>Memperlihatkan elemen-elemen DOM yang ditunjuk mouse saat anda menjelajahi halaman web.(<a class="external" href="http://www.karmatics.com/aardvark/">selengkapnya</a>)</dd>
</dl>

<dl>
 <dt><a class="link-https" href="https://addons.mozilla.org/en-US/firefox/browse/type:1/cat:4">More on Firefox Add-ons</a></dt>
 <dd>Kategori pengembangan web dalam situs Firefox Add-ons</dd>
</dl>

<h2 id="Validators" name="Validators">Validator</h2>

<dl>
 <dt><a href="/en-US/docs/Tools/Validators" title="en/Tools/Validators">Daftar validator</a></dt>
 <dd>Beragam validator untuk hal seperti HTML, CSS, RDF, Ekstensi Firefox, dan banyak lagi yang lainnya.</dd>
</dl>

<h2 id="Authoring_Software" name="Authoring_Software">Authoring Software</h2>

<dl>
 <dt><a class="external" href="http://tidy.sourceforge.net/">HTMLTidy</a></dt>
 <dd>Alat yang digunakan untuk memperbaiki atau menunjukan bagian HTML yang tidak benar serta meningkatkan layout dan lekukan gaya yang dihasilkan markup.</dd>
</dl>

<h2 id="JavaScript" name="JavaScript">JavaScript</h2>

<dl>
 <dt><a href="/en-US/docs/Error_Console" title="en/Error_Console">Error Console</a></dt>
 <dd>Alat yang digunakan untuk melaporkan kesalahan atau error dalam aplikasi chrome dan halaman web user yang terbuka. Juga melaporkan kesalahan dan peringatan terkait dengan JavaScript, kesalahan-kesalahan pada CSS dan juga pesan-pesan kewenangan dari kode chrome.</dd>
</dl>

<dl>
 <dt><a href="/en-US/docs/Venkman" title="en/Venkman">Venkman</a></dt>
 <dd>JavaScript Debugger milik mozilla</dd>
 <dt><a class="external" href="http://www.jshint.com/">JSHint</a></dt>
 <dd>Alat analisis statis dan kualitas kode JavaScript</dd>
</dl>

<dl>
 <dt><a class="external" href="http://www.jslint.com/">JSLint</a></dt>
 <dd>Alat kualitas kode JavaScript</dd>
</dl>

<dl>
 <dt><a class="external" href="http://jsdoc.sourceforge.net/">JSDoc</a></dt>
 <dd>Alat yang digunakan untuk melakukan generalisasi sebuah dokumentasi (biasanya HTML) dari komen kode (hampir sama dengan JavaDoc)</dd>
</dl>

<h2 id="DOM" name="DOM">DOM</h2>

<dl>
 <dt><a href="/en-US/docs/DOM_Inspector" title="en/DOM_Inspector">DOM Inspector</a></dt>
 <dd>Alat pengembangan yang digunakan untuk menginspeksi, menjelajah, dan mengubah DOM(<em>Document Object Model</em>) dari dokumen-dokumen.</dd>
</dl>

<dl>
 <dt><a class="external" href="http://slayeroffice.com/tools/modi/v2.0/modi_help.html">MODI</a></dt>
 <dd>(<em>Mouseover DOM Inspector</em>) adalah <em>bookmarklet</em> yang mengijinkan anda untuk melihat dan memanipulasi DOM sebuah web secara mudah dengan menjelajahi dokumen dengan mouse.</dd>
</dl>

<h2 id="Localization" name="Localization">Lokalisasi</h2>

<dl>
 <dt><a class="external" href="http://www.mozilla.org/projects/l10n/mlp_tools.html">Lokasisasi dan pemanfaatan alat</a></dt>
 <dd>Alat dan sumber daya untuk membantu proses penglokalan dan penerjemahan ekstensi anda ke dalam bahasa yang lain.</dd>
</dl>

<h2 id="Accessibility" name="Accessibility">Aksesbilitas</h2>

<h3 id="Kebijakan">Kebijakan</h3>

<dl>
 <dt><a class="external" href="http://www.w3.org/WAI/intro/aria" title="WAI-ARIA Overview">Tinjauan WAI-ARIA </a></dt>
 <dd>WAI-ARIA, <em>Accessible Rich Internet Applications</em> (aplikasi internet berharga yang mudah diakses) rangkaian himpunan dokumen yang tersusun bagaimana membuat situs Web 2.0 dan aplikasi-aplikasi lebih mudah diakses.</dd>
</dl>

<h3 id="Testing_Tools">Testing Tools</h3>

<dl>
 <dt><a class="external" href="http://achecker.ca/checker/index.php" title="AChecker">AChecker</a></dt>
 <dd>AChecker&nbsp; adalah alat yang memungkinkan anda untuk menuliskan url dan menguji aksesbilitasnya.</dd>
 <dt><a class="external" href="http://www.w3.org/WAI/ER/tools/complete" title="W3C Complete list of tools">Daftar lengkap alat-alat W3C</a></dt>
 <dd>Sebuah daftar lengkap alat untuk mengevaluasi aksesbilitas sebuah web.</dd>
</dl>

<p>Untuk daftar sumber aksesbilitas yang lebih komprehensif, bisa dilihat pada: <a class="external" href="http://wiki.fluidproject.org/display/fluid/Accessibility+Resources" title="Accessibility resources">Fluid Project accessibility resources</a> dan <a href="/en-US/docs/Accessibility/ARIA" title="ARIA">ARIA</a>.</p>

<h2 id="Tree_and_branch_management" name="Tree_and_branch_management">Manajemen tree and branch(Pohon dan cabang)</h2>

<dl>
 <dt><a href="/en-US/docs/Using_cross_commit" title="en/Using_cross_commit"><code>cross-commit</code> script</a></dt>
 <dd>Concurrent Versions System(CVS) adalah script yang memungkinkan sebuah <em>patch</em> tunggal menjadi mudah diperiksa dalam banyak bagian cabang.</dd>
</dl>

<h2 id="User_Profile_Tools" name="User_Profile_Tools">Perkakas Profil Pengguna</h2>

<p><a href="/en-US/docs/Mozilla/Multiple_Firefox_Profiles" title="Multiple Firefox profiles">Profil ganda Firefox</a></p>

<h2 id="Navigating_the_Mozilla_Codebase">Navigating the Mozilla Codebase</h2>

<p><a class="external" href="http://mxr.mozilla.org/" title="http://mxr.mozilla.org/">MXR</a> (if you use vim, mxr-vim speeds up the process)</p>

<p><a class="external" href="http://dxr.mozilla.org/clang/" title="http://dxr.mozilla.org/clang/">DXR</a></p>

<dl>
 <dt><a class="external" href="/en-US/docs/Profile_Manager" title="en/Profile_Manager">Profile Manager</a></dt>
</dl>

<p><span class="comment">Categories</span></p>

<p><span class="comment">Interwiki Language Links</span></p>

<div>{{CommunityBox("Developer tools", "dev-developer-tools", "mozilla.dev.developer-tools", "devtools", "Team info|https://wiki.mozilla.org/DevTools|Dev tools wiki|Designs and plans for the dev tools||Blog|https://hacks.mozilla.org/|Hacks blog|Hacks blog", "FirefoxDevTools", "firefox-developer-tools")}}</div>

<h2 id="Subnav">Subnav</h2>

<ol>
 <li><a href="#">Creating</a>

  <ol>
   <li><a href="/en-US/docs/Tools/Scratchpad">Scratchpad</a></li>
   <li><a href="/en-US/docs/Tools/Style_Editor">Style Editor</a></li>
   <li><a href="/en-US/docs/Tools/Shader_Editor">Shader Editor</a></li>
   <li><a href="/en-US/docs/Tools/Web_Audio_Editor">Web Audio Editor</a></li>
  </ol>
 </li>
 <li><a href="#">Debugging</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Page_Inspector">Page Inspector</a></li>
   <li><a href="/en-US/docs/Tools/Web_Console">Console</a></li>
   <li><a href="/en-US/docs/Tools/Debugger">Debugger</a></li>
   <li><a href="/en-US/docs/Tools/Network_Monitor">Network Monitor</a></li>
   <li><a href="/en-US/docs/Tools/Storage_Inspector">Storage Inspector</a></li>
   <li><a href="/en-US/docs/Tools/DOM_Property_Viewer">DOM Property Viewer</a></li>
   <li><a href="/en-US/docs/Tools/GCLI">Developer Toolbar</a></li>
   <li><a href="/en-US/docs/Tools/3D_View">3D View</a></li>
   <li><a href="/en-US/docs/Tools/Eyedropper">Eyedropper</a></li>
   <li><a href="/en-US/docs/Tools/about:debugging">about:debugging</a></li>
   <li><a href="/en-US/docs/tools/Working_with_iframes">Selecting iframes</a></li>
   <li><a href="/en-US/docs/Tools/View_source">View Source</a></li>
  </ol>
 </li>
 <li><a href="#">Mobile</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Responsive_Design_Mode">Responsive Design Mode</a></li>
   <li><a href="/en-US/docs/Tools/WebIDE">WebIDE</a></li>
   <li><a href="/en-US/docs/Tools/Remote_Debugging/Firefox_for_Android">Firefox for Android</a></li>
   <li><a href="/en-US/docs/Tools/Firefox_OS_Simulator">Firefox OS Simulator</a></li>
  </ol>
 </li>
 <li><a href="#">Performance</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Performance">Performance Tool</a></li>
   <li><a href="/en-US/docs/Tools/Memory">Memory</a></li>
   <li><a href="/en-US/docs/Tools/Performance/Frame_rate">Frame rate graph</a></li>
   <li><a href="/en-US/docs/Tools/Performance/Waterfall">Waterfall</a></li>
   <li><a href="/en-US/docs/Tools/Performance/Call_Tree">Call Tree</a></li>
   <li><a href="/en-US/docs/Tools/Performance/Flame_Chart">Flame Chart</a></li>
   <li><a href="/en-US/docs/Tools/Paint_Flashing_Tool">Paint Flashing Tool</a></li>
   <li><a href="/en-US/docs/Tools/Web_Console/Console_messages#Reflow_events">Reflow Event Logging</a></li>
   <li><a href="/en-US/docs/Tools/Network_Monitor#Performance_analysis">Network Performance</a></li>
  </ol>
 </li>
 <li><a href="#">Debugging the browser</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Browser_Console">Browser Console</a></li>
   <li><a href="/en-US/docs/Tools/Browser_Toolbox">Browser Toolbox</a></li>
  </ol>
 </li>
 <li><a href="#">Extending the devtools</a>
  <ol>
   <li><a href="/en-US/docs/Tools/Adding_a_panel_to_the_toolbox">Adding a panel to the toolbox</a></li>
   <li><a href="/en-US/docs/Tools/Example_add-ons">Example devtools add-ons</a></li>
   <li><a href="https://wiki.mozilla.org/Remote_Debugging_Protocol">Remote Debugging Protocol</a></li>
   <li><a href="https://wiki.mozilla.org/Remote_Debugging_Protocol_Stream_Transport">Stream Transport</a></li>
   <li><a href="/en-US/docs/Tools/Editor">Source Editor</a></li>
   <li><a href="/en-US/docs/Tools/Debugger-API">The <code>Debugger</code> Interface</a></li>
   <li><a href="/en-US/docs/Tools/Web_Console/Custom_output">Web Console custom output</a></li>
  </ol>
 </li>
 <li><a href="/en-US/docs/Tools/Settings">Settings</a></li>
 <li><a href="/en-US/docs/Tools/Release_notes">Release notes</a></li>
</ol>

