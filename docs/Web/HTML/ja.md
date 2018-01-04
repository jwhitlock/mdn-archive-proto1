---
version: prototype1
revision_id: 1342797
locale: ja
slug: Web/HTML
tags: "HTML" "HTML プログラミング" "HTML5" "Web" "Landing" "Hyper text" "Reference"
title: HTML
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{HTMLSidebar}}</div>

<p class="summary"><span class="seoSummary"><strong>HTML</strong> (HyperText Markup Language) は Web のもっとも基本的な構成要素です。 HTML は Web ページの<em>コンテンツ</em>を記述し定義するものです。 HTML に隣接する他の技術としては、 Web ページの表示や表現を記述するもの (<a href="/ja/docs/Web/CSS">CSS</a>) または機能や振る舞いを記述するもの (<a href="/ja/docs/Web/JavaScript">JavaScript</a>) があります。</span></p>

<p>「ハイパーテキスト」は Web ページから別なページに、ウェブサイト内でもウェブサイト間でも、接続するリンクを示します。リンクは Web の基礎的な特徴です。コンテンツをインターネットにアップロードして他の人々が作成したページにリンクすれば、 World Wide Web の活発な参加者になれます。</p>

<p>HTML では Web ブラウザーのテキスト、画像、その他のコンテンツを記述するために「マークアップ」を使用します。 HTML マークアップには、 {{HTMLElement("head")}}、 {{HTMLElement("title")}}、 {{HTMLElement("body")}}、 {{HTMLElement("header")}}、 {{HTMLElement("footer")}}、 {{HTMLElement("article")}}、 {{HTMLElement("section")}}、 {{HTMLElement("p")}}、 {{HTMLElement("div")}}、 {{HTMLElement("span")}}、 {{HTMLElement("img")}}、その他のたくさんの特殊な「要素」を用います。</p>

<p>以下の記事は HTML に関してもっと学ぶのに役立つでしょう。</p>

<section class="cleared" id="sect1">
<ul class="card-grid">
 <li><span>HTML 概論</span>

  <p>Web 開発が初めてであれば、 HTML とは何か、 HTML の使用方法を説明する<a href="/ja/docs/Learn/Getting_started_with_the_web/HTML_basics">HTMLの基本</a>をご覧ください。</p>
 </li>
 <li><span>HTML チュートリアル</span>
  <p>チュートリアルや例を含む HTML の使用方法に関する記事は、<a href="/ja/docs/Learn/HTML">HTML 学習エリア</a>を確認してください。</p>
 </li>
 <li><span>HTML リファレンス</span>
  <p>広範な <a href="/ja/docs/Web/HTML/Reference">HTML リファレンス</a>の章で、 HTML のすべての要素と属性についての詳細が分かります。</p>
 </li>
</ul>

<div class="row topicpage-table">
<div class="section">
<h2 class="Tools" id="Tools" name="Tools">初心者向けチュートリアル</h2>

<p><a href="/ja/docs/Learn/HTML">HTML 学習エリア</a>は HTML を基礎から学ぶための複数のモジュールを中心としています — 前提知識は必要ありません。</p>

<dl>
 <dt><a href="/ja/docs/Learn/HTML/Introduction_to_HTML">HTML 概論</a></dt>
 <dd>このモジュールは、 HTML をテキストに適用する方法、ハイパーリンクを作成する方法、 HTML を使用して Web ページを構築する方法など、重要な概念と構文に慣れていく段階を設定します。</dd>
 <dt><a href="/ja/docs/Learn/HTML/Multimedia_and_embedding">マルチメディアとその埋め込み方</a></dt>
 <dd>This module explores how to use HTML to include multimedia in your web pages, including the different ways that images can be included, and how to embed video, audio, and even entire other webpages.</dd>
 <dt><a href="/ja/docs/Learn/HTML/Tables">HTML テーブル</a></dt>
 <dd>Representing tabular data on a webpage in an understandable, accessible way can be a challenge. This module covers basic table markup, along with more complex features such as implementing captions and summaries.</dd>
 <dt><a href="/ja/docs/Learn/HTML/Forms">HTML フォーム</a></dt>
 <dd>Forms are a very important part of the Web — these provide much of the functionality you need for interacting with websites, e.g. registering and logging in, sending feedback, buying products, and more. This module gets you started with creating the client-side/front-end parts of forms.</dd>
 <dt><a href="https://developer.mozilla.org/ja/docs/Learn/HTML/Howto">共通の問題解決に HTML を使う</a></dt>
 <dd>Provides links to sections of content explaining how to use HTML to solve very common problems when creating a web page: dealing with titles, adding images or videos, emphasizing content, creating a basic form, etc.</dd>
</dl>

<h2 id="Advanced_topics">高度なトピック</h2>

<dl>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/CORS_enabled_image">CORS enabled image</a></dt>
 <dd class="landingPageList">HTML 仕様には画像に {{htmlattrxref("crossorigin", "img")}} 属性が定義されています。この属性と適切な <a class="glossaryLink" href="/ja/docs/Glossary/CORS">CORS</a> ヘッダを組み合わせることで、異なる origin から読み出された {{HTMLElement("img")}} 要素の画像を、あたかも同じ origin から読み出したもののように canvas から扱うことができます。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/CORS_settings_attributes">CORS 設定属性</a></dt>
 <dd class="landingPageList">HTML5 では {{HTMLElement("img")}} や {{HTMLElement("video")}} など、<a href="/ja/docs/HTTP/Access_control_CORS">CORS</a> をサポートするいくつかの HTML 要素に <code>crossorigin</code> 属性 (<code>crossOrigin</code> プロパティ) が定義されています。この属性は、要素の取得したデータに関わる CORS リクエストを設定するものです。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Focus_management_in_HTML">HTML でのフォーカス管理</a></dt>
 <dd class="landingPageList">The <code><a href="/ja/docs/Web/API/Document/activeElement">activeElement</a></code> DOM attribute and the <code><a href="/ja/docs/Web/API/Document/hasFocus">hasFocus()</a></code> DOM method help you track and control a user's interactions with elements on a web page.</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Using_the_application_cache">アプリケーションキャッシュの使用</a></dt>
 <dd class="landingPageList">アプリケーションキャッシュは、ウェブベースのアプリケーションをオフラインで実行させるためのものです。ブラウザがキャッシュし、オフライン状態のユーザが利用できるようにすべきリソースを指定するために <strong>Application Cache</strong> (<em>AppCache</em>) インターフェースを利用できます。キャッシュが行われたアプリケーションは、ユーザがオフラインになったときに更新ボタンを押した場合でも、正常に読み込まれ、正常に動作します。</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/ja/docs/Web/HTML/Preloading_content">rel="preload" でコンテンツをプリロード</a></dt>
 <dd class="landingPageList">The <code>preload</code> value of the {{htmlelement("link")}} element's {{htmlattrxref("rel", "link")}} attribute allows you to write declarative fetch requests in your HTML {{htmlelement("head")}}, specifying resources that your pages will need very soon after loading, which you therefore want to start preloading early in the lifecycle of a page load, before the browser's main rendering machinery kicks in. This ensures that they are made available earlier and are less likely to block the page's first render, leading to performance improvements. This article provides a basic guide to how <code>preload</code> works.</dd>
</dl>
</div>

<div class="section">
<h2 class="Documentation" id="References">リファレンス</h2>

<dl>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Reference">HTML リファレンス</a></dt>
 <dd class="landingPageList">HTML は web ドキュメントの構造やセマンティックな内容を記述する言語です。HTML は<strong>要素</strong>で構成されており、それぞれの要素がいくつかの<strong>属性</strong>で調節される場合があります。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Element">HTML 要素リファレンス</a></dt>
 <dd class="landingPageList">このページでは、すべての <a class="glossaryLink" href="/ja/docs/Glossary/HTML">HTML</a> <a class="glossaryLink" href="/ja/docs/Glossary/Element">要素</a>を一覧表示しています。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Attributes">HTML 属性リファレンス</a></dt>
 <dd class="landingPageList">HTML 要素には<strong>属性</strong>があります。これはユーザが求める基準を満たすために、さまざまな方法で要素の設定や動作の調整を行う付加的な値です。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Global_attributes">グローバル属性</a></dt>
 <dd class="landingPageList">グローバル属性は、<em>標準仕様で明示されていないものを含む</em>すべての <a href="/ja/docs/Web/HTML/Element">HTML 要素</a>に定められるでしょう。これはあらゆる非標準の要素が、それを使用することで文書が HTML5 に準拠しなくなるとしても、グローバル属性を受け入れなければならないということです。例えば <code>&lt;foo&gt;</code> は正当な HTML 要素ではありませんが、HTML5 準拠のブラウザは <code>&lt;foo hidden&gt;...&lt;foo&gt;</code> とマークアップされたコンテンツを隠します。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Inline_elements">インライン要素</a> と <a href="/ja/docs/Web/HTML/Block-level_elements">ブロックレベル要素</a></dt>
 <dd class="landingPageList">HTML (Hypertext Markup Language) 要素は通常、"インライン" 要素または <a href="/ja/docs/Web/HTML/Block-level_elements">"ブロックレベル" 要素</a>のいずれかになります。インライン要素は、要素を定義するタグによって結びつけられた領域のみ占有します。以下のサンプルでは、インライン要素が与える影響を示しています。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Link_types">リンクタイプ</a></dt>
 <dd class="landingPageList">HTML では、さまざまな種類のリンクが2つの文書の関係を確立し定義するために使用できます。リンク要素は <a href="/ja/docs/Web/HTML/Element/a"><code>&lt;a&gt;</code></a>、 <a href="/ja/docs/Web/HTML/Element/area"><code>&lt;area&gt;</code></a>、 <a href="/ja/docs/Web/HTML/Element/link"><code>&lt;link&gt;</code></a> などで設定できます。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Supported_media_formats">HTML の audio 要素と video 要素でサポートされているメディアフォーマット</a></dt>
 <dd class="landingPageList">The <a href="/ja/docs/Web/HTML/Element/audio"><code>&lt;audio&gt;</code></a> and <a href="/ja/docs/Web/HTML/Element/video"><code>&lt;video&gt;</code></a> elements allow you to play audio and video media. These elements provide a browser-native alternative to similar capabilities found in Adobe Flash and other plug-ins.</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Kinds_of_HTML_content">Kinds of HTML content</a></dt>
 <dd class="landingPageList">HTML is comprised of several kinds of content, each of which is allowed to be used in certain contexts and is disallowed in others. Similarly, each has a set of other content categories they can contain and elements which can or can't be used in them. This is a guide to these categories.</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Quirks_Mode_and_Standards_Mode">後方互換モードと標準準拠モード</a></dt>
 <dd class="landingPageList">Historical information on quirks mode and standards mode.</dd>
</dl>

<h2 class="landingPageList" id="Related_topics">関連トピック</h2>

<dl>
 <dt><a href="/ja/docs/Web/HTML/Applying_color">CSSを使ってHTMLの要素に色をつける</a></dt>
 <dd>This article covers most of the ways you use CSS to add color to HTML content, listing what parts of HTML documents can be colored and what CSS properties to use when doing so. Includes examples, links to palette-building tools, and more.</dd>
</dl>
</div>
</div>
<span class="alllinks"><a href="/ja/docs/tag/HTML">すべて表示...</a></span>

<p>{{CommunityBox("Web layout", "dev-tech-layout", "mozilla.dev.tech.layout", "", "Stack Overflow|http://stackoverflow.com/questions/tagged/html|HTML topics|Visit Stack Overflow, a collaboratively built and maintained Q&amp;A site. See if you can find an answer; if not, you can ask your question there.")}}</p>
</section>

