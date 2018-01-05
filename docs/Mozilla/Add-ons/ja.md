---
version: prototype1
revision_id: 1343566
locale: ja
slug: Mozilla/Add-ons
tags: "Add-ons" "Landing" "Mozilla" "Extension" "Extensions"
title: アドオン
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: True
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<div>&nbsp;</div>

<p><span class="seoSummary">開発者は{{gengoheiki("アドオン","add-on")}} を作成して Firefox を拡張したり機能を変更できます。</span> アドオンは JavaScript、HTML、CSS といったWeb標準技術と、幾つかの専用JavaScript APIを使って作成します。アドオンは、主に以下のようなことを実現できます。</p>

<ul>
 <li>特定のウェブサイトの見た目や内容を変更する</li>
 <li>Firefoxのユーザーインタフェースを変更する</li>
 <li>Firefoxに新しい機能を追加する</li>
</ul>

<p>アドオンには幾つかの種類がありますが、もっとも一般的なのは<a href="/ja/docs/Extensions" title="Extensions">{{gengoheiki("拡張機能","extension")}}</a>です。</p>

<h2 id="Developing_extensions" name="Developing_extensions">拡張機能の開発</h2>

<p>以前はFirefoxの拡張機能を開発するためのツールセットが幾つかありましたが、2017年11月末までに<a href="/ja/docs/Mozilla/Add-ons/WebExtensions">WebExtensions API</a>を使って拡張機能をビルドするようにしなければいけません。 それ以外のツールセットは同期間で非推奨になる予定です（例えば overlay add-on, bootstrapped add-on, add-on SDK）。</p>

<p>新しく拡張機能を作成するには <a href="https://developer.mozilla.org/ja/Add-ons/WebExtensions">WebExtensions API</a> を使いましょう。</p>

<p>WebExtensions APIを使ってFirefox向けに作った拡張機能は、ブラウザ間の互換性を持つように設計されています。大抵の場合、Chrome、Edge、Operaでも修正無しか、わずかな修正で動作するでしょう。マルチプロセスFirefoxとも完全な互換性があります。<br />
 <br />
 現在の<a href="/ja/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">各ブラウザのAPIサポート状況</a>もご覧下さい。私たちは開発者のニーズに応えて新しいAPIの設計・実装を続けています。<br />
 <br />
 ほとんどの WebExtensions API は、Android向けのFirefoxでも利用可能です。</p>

<h3 id="Migrate_an_existing_extension" name="Migrate_an_existing_extension">既存の拡張機能を移行するには</h3>

<p>もしあなたが既存の拡張機能（XUL overlay、bootstrapped、add-on SDK を使ったもの）を保守しているなら、WebExtension APIを使って移植できます。 MDNの<a href="/ja/docs/Mozilla/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">関連記事</a>をご覧ください。</p>

<p>移行全般のサポート情報は、<a href="https://wiki.mozilla.org/Add-ons/developer/communication">Wikiページ</a>を見てください。</p>

<h2 id="Publishing_add-ons" name="Publishing_add-ons">アドオンを公開するには</h2>

<p><a href="https://addons.mozilla.org">Addons.mozilla.org</a> は、「AMO」という名前で知られるMozilla公式サイトです。開発者はアドオンを掲載し、ユーザーはアドオンを探すことができます。アドオンを開発したらAMOにアップロードして、ユーザーやクリエイターのコミュニティに注目してもらいましょう。</p>

<p>開発したアドオンをAMOに掲載することは必須ではありませんが、Mozillaが署名しない限り、ユーザーはインストールできません。</p>

<p>アドオンを公開する手順の概要については、<a href="/ja/Add-ons/Distribution">アドオンに署名して配布するには</a>をご覧ください。</p>

<h2 id="Other_types_of_add-ons" name="Other_types_of_add-ons">その他の種類のアドオン</h2>

<p>拡張機能の他にも、ユーザーがFirefoxをカスタマイズするためのアドオンが何種類かあります。</p>

<ul>
 <li><a href="/Add-ons/Themes/Background">{{gengoheiki("テーマ","Lightweight themes")}}</a> を使うと、限定的ですが簡単にFirefoxをカスタマイズできます</li>
 <li><a href="/Add-ons/Firefox_for_Android">Mobile add-ons</a> はAndroid向け Firefox 用のアドオンです。ただし、これらのAPIは一部の基盤技術が非推奨に変更される方向ですので、ご注意下さい。将来は、Android向けFirefoxでもWebExtensions APIを一定範囲でフルサポートする予定です。</li>
 <li><a href="/ja/docs/Creating_OpenSearch_plugins_for_Firefox">Search engine plugins</a> は、ブラウザの検索バーに新しい検索エンジンを追加します。</li>
 <li><a href="/ja/docs/Mozilla/Creating_a_spell_check_dictionary_add-on">User dictionaries</a> は、色々な言語のスペルチェックを可能にします。</li>
 <li><a href="https://support.mozilla.org/kb/use-firefox-interface-other-languages-language-pack">Language packs</a> は、Firefoxのユーザーインタフェースで更に多くの言語をサポートできるようにします。</li>
</ul>

<hr />
<h2 id="Contact_us" name="Contact_us">Contact us</h2>

<p>疑問や質問、アドオン関連の最新ニュース、フィードバックなどは、下記のリンクからどうぞ。</p>

<h3 id="Add-ons_forum" name="Add-ons_forum">アドオン フォーラム</h3>

<p><a href="https://discourse.mozilla.org/c/add-ons">Add-ons Discourse forum</a> は、アドオン開発全般の議論や質問に使って下さい。</p>

<h3 id="Mailing_lists" name="Mailing_lists">メーリング リスト</h3>

<p><strong>dev-addons</strong> は、アドオン関連するシステムの議論（WebExtensionsシステムやAMOの開発を含む）に使ってください。</p>

<ul>
 <li><a href="https://mail.mozilla.org/listinfo/dev-addons">dev-addons list info</a></li>
 <li><a href="https://mail.mozilla.org/pipermail/dev-addons/">dev-addons archives</a></li>
</ul>

<h3 id="IRC" name="IRC">IRC</h3>

<p>IRCがお好きなら、こちらで連絡できます。</p>

<ul>
 <li><a href="irc://irc.mozilla.org/addons">#addons</a> (add-ons エコシステムの議論)</li>
 <li><a href="irc://irc.mozilla.org/extdev">#extdev</a> (add-on 開発一般の議論)</li>
 <li><a href="irc://irc.mozilla.org/webextensions">#webextensions</a> (特に WebExtensions API in 関連の議論)</li>
</ul>

<h3 id="Report_problems" name="Report_problems">問題を報告する</h3>

<h4 id="Security_vulnerabilities" name="Security_vulnerabilities">セキュリティ欠陥</h4>

<p>アドオンのセキュリティ欠陥を見つけた場合は、それがMozillaのサイトで提供しているものでなくても、私たちまでお知らせ下さい。私たちは開発者と協力して問題を修正します。 連絡は<a href="http://www.mozilla.org/projects/security/security-bugs-policy.html">非公開で</a>、 <a href="https://bugzilla.mozilla.org/enter_bug.cgi?product=addons.mozilla.org&amp;component=Add-on%20Security&amp;maketemplate=Add-on%20Security%20Bug&amp;bit-23=1&amp;rep_platform=All&amp;op_sys=All">Bugzilla</a> または <a href="mailto:amo-admins@mozilla.org">amo-admins@mozilla.org 宛てのメール</a>でお願いします。</p>

<h4 id="Bugs_on_addons.mozilla.org_(AMO)" name="Bugs_on_addons.mozilla.org_(AMO)">サイト addons.mozilla.org (AMO)のバグ</h4>

<p>もしサイト自体の問題を見つけたら、是非修正したいと思います。 <a href="https://github.com/mozilla/addons/issues/new">バグ報告して</a>、できるだけ多くの詳細を含めてください。</p>

