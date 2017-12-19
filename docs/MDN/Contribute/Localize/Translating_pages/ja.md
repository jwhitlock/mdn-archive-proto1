---
version: prototype1
revision_id: 1338193
locale: ja
slug: MDN/Contribute/Localize/Translating_pages
tags: "MDN" "l10n" "MDN Meta" "Guide" "Localization" "Page Tlanslation"
title: MDNページの翻訳
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>この記事はMDNのページを翻訳する際に参考にしていただく記事です。翻訳の手順や、コンテンツの内容に応じた適切な翻訳を行う際のヒントが含まれています。</p>

<h2 id="ページの翻訳を始める"><strong style="font-size:2.142857142857143rem; font-weight:700; letter-spacing:-1px; line-height:30px">ページの翻訳を始める</strong></h2>

<p>このサイトのページを日本語などに翻訳してみたいと思われたときは、以下の手順にしたがってください。</p>

<ol>
 <li>言語アイコン ({{FontAwesomeIcon("icon-language")}})をクリックし <strong>言語</strong> メニューを開きます。メニューの中から<strong> Add a Translation </strong>を選択すると言語選択画面が現れます。&nbsp;</li>
 <li>日本語など、あなたが新たに翻訳したい先の言語を選択します。翻訳用のビューが開かれ、その左側には翻訳前の記事が表示されます。</li>
 <li><strong>翻訳についての説明</strong> では記事タイトルとslugの翻訳をしていただけます。slugはページのURLの最後の部分のことをいいます (例えばこの記事のslugは"Translating_pages"になります) 。slugは翻訳するかどうかは各言語のコミュニティによりますが、翻訳しない場合は英語版のものを利用してください。他の日本語版の記事を参考にしながら翻訳の一般的な方法に従っておくといいでしょう。<strong>翻訳についての説明 </strong>の横にあるマイナスのマークをクリックするとこれらの編集画面を閉じておいて、<strong>内容を翻訳</strong> の節のスペースを増やすことも可能です。</li>
 <li><strong>内容を翻訳</strong> よりも下がページの記事本文です。翻訳を始めてください。</li>
 <li>ページに付加する<strong> タグ </strong>を1つ以上付けます。</li>
 <li>終わったら <strong>変更を保存</strong> をクリックして内容を保存します。</li>
</ol>

<div class="note"><strong>Note:</strong>&nbsp;翻訳ビューは最初は英語版のユーザインターフェイス(UI)で表示されます。次回以降に翻訳ビューを開いた場合、日本語版が使用可能であれば日本語版のUIで表示されます。MDNのUIは <a href="https://localize.mozilla.org/projects/mdn/" title="https://localize.mozilla.org/projects/mdn/">Verbatim</a>を使用して日本語化が可能です。詳細とツールの使い方については&nbsp;<a href="/docs/Mozilla/Localization/Localizing_with_Verbatim" title="/en-US/docs/Mozilla/Localization/Localizing_with_Verbatim">Localizing with Verbatim</a>&nbsp;を御覧ください。</div>

<div class="note">{{Yakuchu("日本語翻訳向けUserScirptのご紹介")}}<br />
MDN公式の機能ではなく翻訳コミュニティの成果ですが、下記のUserScriptを導入すると処理の手間が省けます。<br />
<a href="https://groups.google.com/forum/#!topic/mozilla-translations-ja/0CxlXZDeJB4">Google Groups: MDNで新規翻訳する際に下ごしらえするUserScript</a><br />
<a href="https://github.com/mozilla-japan/translation/tree/master/MDN">UserScriptのリポジトリ(インストールはこちらから)</a></div>

<h2 id="翻訳されたページの編集">翻訳されたページの編集</h2>

<ul>
 <li>翻訳されたページで<strong> 編集</strong> ボタンをクリックしてください。翻訳ビューが開きます。</li>
</ul>

<p>もし英語バージョンの記事が日本語版の最新記事よりも新しい場合は、英語版記事のソースレベルの"差分"を表示します。その差分を元に翻訳記事を更新してください。</p>

<h2 id="タグの翻訳">タグの翻訳</h2>

<p>たとえ記事が英語版の翻訳であったとしても、すべてのページに少なくともひとつのタグを付ける必要があります。一般的に、オリジナル記事と同じタグを使うのがいい考えです。</p>

<p>検索結果のフィルタリングや貢献者同士の規約として使われているタグもあります。これらは翻訳されるべきではありません。より詳しいルールや使い方などは、<a href="https://developer.mozilla.org/ja/docs/MDN/Contribute/Howto/Tag">適切にタグづけする方法</a>をご参照ください。なお、既存のタグが記事の中身を表せない場合には新たなタグを自由に作ることができます。</p>

<h2 id="新しい翻訳者向けTips">新しい翻訳者向けTips</h2>

<p>MDN のローカライズに慣れていない場合、いくつかヒントがあります:</p>

<ul>
 <li><a href="https://developer.mozilla.org/ja/docs/Glossary">Glossary</a> 内の記事は、短くシンプルなので、新規翻訳者に良いです。</li>
 <li><a href="https://developer.mozilla.org/ja/docs/tag/l10n%3Apriority">"l10n:priority" とタグづけされた</a> 記事は優先度が高いと考えられています。また、一般に、チュートリアルと概念的な記事は、読者が新しい概念を学ぶ時に翻訳の必要性が最も高いために、リファレンスページと比べて高優先です。</li>
 <li><code>\{{some-text("more text")}}</code> のように二重波括弧で囲まれたテキストを見かけたら、そのまま訳さずに、 句読点も変えずにおきます。これは<a href="https://developer.mozilla.org/ja/docs/MDN/Contribute/Structures/Macros">マクロ</a>で、たぶんページの構造を作ったり、その他の役立つことを行っています。 マクロで生成された訳されないテキストが見えるでしょうが、もっと MDN の経験を踏むまで気にしないでください。 (マクロはとても強力なので、このテキストを変更するには<a href="https://developer.mozilla.org/ja/docs/MDN/Contribute/Tools/Template_editing">特別な権限</a>が必要です。気になるなら、<a href="https://developer.mozilla.org/ja/docs/MDN/Contribute/Structures/Macros/Commonly-used_macros">よく使われるマクロ</a>を見て、マクロにできることを見てください。</li>
 <li><a href="https://developer.mozilla.org/ja/docs/MDN/Contribute/Localize/Localization_projects">Localization プロジェクトのページ</a>を見てあなたのロケールのローカライゼーションの詳細を発見してください。</li>
</ul>

<h2 id="日本語版での翻訳作業について">日本語版での翻訳作業について</h2>

<p>日本語版での翻訳作業の手順や役に立つ情報については、Firefox OS コミュニティサイトの「<a href="http://fxos.org/hacks/mdn_doc_fest/">Mozillaドキュメント翻訳の始め方</a>」というページにまとめられています。</p>

<p>翻訳コミュニティの Github の <a href="https://github.com/mozilla-japan/translation/wiki">Wiki</a> や <a href="https://github.com/mozilla-japan/translation/issues">Issues</a> で募集されている翻訳なども参考にしてください。</p>

<p>&nbsp;</p>

