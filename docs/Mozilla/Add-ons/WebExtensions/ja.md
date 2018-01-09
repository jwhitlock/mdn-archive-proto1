---
version: prototype1
revision_id: 1344807
locale: ja
slug: Mozilla/Add-ons/WebExtensions
tags: "Add-ons" "Landing" "Extensions" "WebExtensions"
title: ブラウザー拡張機能
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>{{AddonSidebar}}</p>

<p>拡張機能はブラウザーの能力を拡張・修正するものです。Firefoxの拡張機能はWebExtensions API を使ってビルドされ、拡張機能をクロスブラウザーで開発するシステムです。このシステムの大半は Google Chrome と Opera と <a href="https://browserext.github.io/browserext/">W3C Draft Community Group</a> でサポートされている <a class="external-icon external" href="https://developer.chrome.com/extensions">extension API</a> と互換性があります。これらのブラウザー用に書かれた拡張機能は大抵の場合、<a href="https://developer.mozilla.org/ja/Add-ons/WebExtensions/Porting_from_Google_Chrome">ほんの少し変更を加えるだけで</a> Firefox や <a href="https://developer.microsoft.com/en-us/microsoft-edge/platform/documentation/extensions/">Microsoft Edge</a> でも動かすことができます。このAPIは <a href="https://developer.mozilla.org/ja/Firefox/Multiprocess_Firefox">マルチプロセス Firefox</a> にも完全互換です。</p>

<p>お持ちのアイデアや質問があったり、レガシーアドオンをWebExtensions APIを使うように移行するのに助力が要る場合、<a href="https://mail.mozilla.org/listinfo/dev-addons">dev-addons のメーリングリスト</a>（英語）や <a href="https://wiki.mozilla.org/IRC">IRC</a> の <a href="irc://irc.mozilla.org/webextensions">#webextensions</a> （英語）にてご連絡ください。</p>

<div class="row topicpage-table">
<div class="section">
<p>{{英語版章題("Getting started")}}</p>

<h2 id="始めましょう">始めましょう</h2>

<ul>
 <li><a href="https://developer.mozilla.org/ja/Add-ons/WebExtensions/What_are_WebExtensions">拡張機能とは何か?</a></li>
 <li><a href="/ja/Add-ons/WebExtensions/Your_first_WebExtension">初めての拡張機能</a></li>
 <li><a href="/ja/Add-ons/WebExtensions/Your_second_WebExtension">2 つめの拡張機能</a></li>
 <li><a href="/ja/Add-ons/WebExtensions/Anatomy_of_a_WebExtension">拡張機能の中身</a></li>
 <li><a href="/ja/Add-ons/WebExtensions/Examples">拡張機能の例</a></li>
</ul>

<p>{{英語版章題("Concepts")}}</p>

<h2 id="概念">概念</h2>

<ul>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/Using_the_JavaScript_APIs">JavaScript API 群の利用</a></li>
 <li><a href="/ja/Add-ons/WebExtensions/Content_scripts">コンテンツスクリプト</a></li>
 <li><a href="/ja/Add-ons/WebExtensions/Match_patterns">マッチパターン</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/Working_with_files">ファイルの操作</a></li>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/Internationalization">多言語対応</a></li>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/Content_Security_Policy">Content Security Policy</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/Native_messaging">Native messaging</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/Using_the_devtools_APIs">Using the devtools APIs</a></li>
 <li><a href="https://developer.mozilla.org/ja/Add-ons/WebExtensions/User_experience_best_practices">ユーザー体験の成功事例</a></li>
 <li><a href="https://developer.mozilla.org/ja/Add-ons/WebExtensions/Native_manifests">Native manifests</a></li>
</ul>

<p>{{英語版章題("User interface")}}</p>

<h2 id="ユーザーインターフェイス">ユーザーインターフェイス</h2>

<ul>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/user_interface">導入</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/user_interface/Browser_action">Browser toolbar button</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/user_interface/Popups">Browser toolbar button with a popup</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/user_interface/Page_actions">Address bar button</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/user_interface/Popups">Address bar button with a popup</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/user_interface/Context_menu_items">Context menu items</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/user_interface/Sidebars">Sidebars</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/user_interface/Options_pages">Options page</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/user_interface/Bundled_web_pages">Bundled web pages</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/user_interface/Notifications">Notifications</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/user_interface/Omnibox">Address bar suggestions</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/user_interface/devtools_panels">Developer tools panels</a></li>
</ul>

<p>{{英語版章題("How to")}}</p>

<h2 id="逆引きリファレンス">逆引きリファレンス</h2>

<ul>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/Intercept_HTTP_requests">HTTP リクエストへの介入</a></li>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/Modify_a_web_page">web ページの変更</a></li>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/Add_a_button_to_the_toolbar">ツールバーボタンの追加</a></li>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/Implement_a_settings_page">設定画面の実装</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/Interact_with_the_clipboard">クリップボードとのやりとり</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/Working_with_the_Tabs_API">Work with the Tabs API</a></li>
</ul>

<p>{{英語版章題("Porting")}}</p>

<h2 id="移行">移行</h2>

<ul>
 <li><a href="/ja/Add-ons/WebExtensions/Porting_from_Google_Chrome">Google Chrome extension からの移行</a></li>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">古い Firefox アドオンの移行</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/Developing_WebExtensions_for_Firefox_for_Android">Developing for Firefox for Android</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/Embedded_WebExtensions">Embedded WebExtensions</a></li>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_the_Add-on_SDK">Add-on SDK との比較</a></li>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_XUL_XPCOM_extensions">XUL/XPCOM 拡張との比較</a></li>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/Chrome_incompatibilities">Chrome との非互換性</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/Differences_between_desktop_and_Android">デスクトップと Android の差異</a></li>
</ul>

<p>{{英語版章題("Firefox workflow")}}</p>

<h2 id="Firefox_でのワークフロー">Firefox でのワークフロー</h2>

<ul>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/User_experience_best_practices">User experience</a></li>
 <li><a href="/ja/Add-ons/WebExtensions/Temporary_Installation_in_Firefox">インストール</a></li>
 <li><a href="/ja/Add-ons/WebExtensions/Debugging">デバッグ</a></li>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/Getting_started_with_web-ext">web-ext を使って始めよう</a></li>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/web-ext_command_reference">web-ext コマンドリファレンス</a></li>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/WebExtensions_and_the_Add-on_ID">WebExtensions と Add-on ID</a></li>
 <li><a href="https://developer.mozilla.org/ja/Add-ons/WebExtensions/Alternative_distribution_options">Alternative distribution options</a></li>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/Publishing_your_WebExtension">WebExtension の公開</a></li>
</ul>
</div>

<div class="section">
<p>{{英語版章題("Reference")}}</p>

<h2 id="リファレンス">リファレンス</h2>

<h3 id="JavaScript_API_群">JavaScript API 群</h3>

<ul>
 <li><a href="/ja/docs/Mozilla/Add-ons/WebExtensions/API">JavaScript API の概要</a></li>
 <li><a href="/ja/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">JavaScript API 群のブラウザ実装状況</a></li>
</ul>

<div class="twocolumns">{{ ListSubpages ("/ja/Add-ons/WebExtensions/API") }}</div>

<h3 id="Manifest_keys" name="Manifest_keys">Manifest keys</h3>

<ul>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/manifest.json">manifest.json overview</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/Browser_compatibility_for_manifest.json">Browser compatibility for manifest.json</a></li>
</ul>

<div class="twocolumns">{{ ListSubpages ("/ja/Add-ons/WebExtensions/manifest.json") }}</div>
</div>
</div>

