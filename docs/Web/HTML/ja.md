---
version: prototype1
revision_id: 1343871
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

<p class="summary"><span class="seoSummary"><strong>HTML</strong> (HyperText Markup Language) はウェブのもっとも基本的な構成要素です。 HTML はウェブページの<em>コンテンツ</em>を記述し定義するものです。 HTML に隣接する他の技術としては、ウェブページの表示や表現を記述するもの (<a href="/ja/docs/Web/CSS">CSS</a>) または機能や振る舞いを記述するもの (<a href="/ja/docs/Web/JavaScript">JavaScript</a>) があります。</span></p>

<p>「ハイパーテキスト」はウェブページから別なページに、ウェブサイト内でもウェブサイト間でも、接続するリンクを示します。リンクはウェブの基礎的な特徴です。コンテンツをインターネットにアップロードして他の人々が作成したページにリンクすれば、 World Wide Web の活発な参加者になれます。</p>

<p>HTML ではウェブブラウザーのテキスト、画像、その他のコンテンツを記述するために「マークアップ」を使用します。 HTML のマークアップには、 {{HTMLElement("head")}}、 {{HTMLElement("title")}}、 {{HTMLElement("body")}}、 {{HTMLElement("header")}}、 {{HTMLElement("footer")}}、 {{HTMLElement("article")}}、 {{HTMLElement("section")}}、 {{HTMLElement("p")}}、 {{HTMLElement("div")}}、 {{HTMLElement("span")}}、 {{HTMLElement("img")}}、その他のたくさんの特殊な「要素」を用います。</p>

<p>以下の記事は HTML に関してもっと学ぶのに役立つでしょう。</p>

<section class="cleared" id="sect1">
<ul class="card-grid">
 <li><span>HTML 概論</span>

  <p>ウェブ開発が初めてであれば、 HTML とは何か、 HTML の使用方法を説明する<a href="/ja/docs/Learn/Getting_started_with_the_web/HTML_basics">HTMLの基本</a>をご覧ください。</p>
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

<p><a href="/ja/docs/Learn/HTML">HTML 学習エリア</a>は HTML を基礎から学ぶための複数のモジュールを中心としています。――前提知識は必要ありません。</p>

<dl>
 <dt><a href="/ja/docs/Learn/HTML/Introduction_to_HTML">HTML 概論</a></dt>
 <dd>このモジュールでは、 HTML を文章に適用する方法、ハイパーリンクを作成する方法、 HTML を使用してウェブページを構築する方法など、重要な概念と構文に慣れていく段階を設定します。</dd>
 <dt><a href="/ja/docs/Learn/HTML/Multimedia_and_embedding">マルチメディアとその埋め込み方</a></dt>
 <dd>このモジュールでは、ウェブページにマルチメディアを埋め込むための HTML の使い方を探ります。画像を入れるための様々な方法、映像、音声、他のウェブページ全体を含める場合も含みます。</dd>
 <dt><a href="/ja/docs/Learn/HTML/Tables">HTML テーブル</a></dt>
 <dd>ウェブページ上で表形式のデータを分かりやすく使いやすい方法で表現するのは難しいことです。このモジュールでは、基本的なテーブルのマークアップと、キャプションやサマリーの追加などのより複雑な機能を扱います。</dd>
 <dt><a href="/ja/docs/Learn/HTML/Forms">HTML フォーム</a></dt>
 <dd>フォームはウェブで非常に重要な部分です。――これはウェブサイトとのやり取り（登録やログイン、フィードバックの送信、商品の購入など）に必要な多くの機能を提供します。このモジュールでは、フォームのクライアント側／フロントエンド部分の作成から始めます。</dd>
 <dt><a href="/ja/docs/Learn/HTML/Howto">よくある問題解決に HTML を使う</a></dt>
 <dd>HTML を使用してウェブページを作成する際に、とてもよくある問題（タイトルの扱い、画像や動画の追加、コンテンツの強調、基本フォームの作成など）を解決する方法を説明する記事の章へのリンクを紹介します。</dd>
</dl>

<h2 id="Advanced_topics">高度なトピック</h2>

<dl>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/CORS_enabled_image">CORS を利用した画像</a></dt>
 <dd class="landingPageList">{{htmlattrxref("crossorigin", "img")}} 属性と <a class="glossaryLink" href="/ja/docs/Glossary/CORS">CORS</a> ヘッダを組み合わせることで、 {{HTMLElement("img")}} 要素で定義された画像を異なるドメインから読み出し、 それを {{HTMLElement("canvas")}} 要素の中で同じドメインから読み出したかのように扱うことができます。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/CORS_settings_attributes">CORS 設定属性</a></dt>
 <dd class="landingPageList"><a href="/ja/docs/HTTP/Access_control_CORS">CORS</a> をサポートするいくつかの HTML 要素（{{HTMLElement("img")}} や {{HTMLElement("video")}} など）は <code>crossorigin</code> 属性（<code>crossOrigin</code> プロパティ）を持っており、要素が取得したデータに関する CORS リクエストを設定することができます。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Focus_management_in_HTML">HTML でのフォーカス管理</a></dt>
 <dd class="landingPageList">DOMの <code><a href="/ja/docs/Web/API/Document/activeElement">activeElement</a></code> 属性と <code><a href="/ja/docs/Web/API/Document/hasFocus">hasFocus()</a></code> メソッドは、ウェブページ上の要素でユーザーのやりとりを追跡し制御するのに役立ちます。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Using_the_application_cache">アプリケーションキャッシュの使用</a></dt>
 <dd class="landingPageList">アプリケーションキャッシュは、ウェブベースのアプリケーションをオフラインで実行させるためのものです。ブラウザがキャッシュし、オフライン状態のユーザが利用できるようにすべきリソースを指定するために <strong>Application Cache</strong> (<em>AppCache</em>) インターフェースを利用できます。キャッシュが行われたアプリケーションは、ユーザがオフラインになったときに更新ボタンを押した場合でも、正常に読み込まれ、正常に動作します。</dd>
 <dt class="landingPageList"><a href="https://developer.mozilla.org/ja/docs/Web/HTML/Preloading_content">rel="preload" でコンテンツを先読み</a></dt>
 <dd class="landingPageList">HTML の {{htmlelement("head")}} 要素内において、 {{htmlelement("link")}} 要素で {{htmlattrxref("rel", "link")}} 属性に <code>preload</code> を指定することで、読み込み後すぐにページに必要なリソース、つまりページ読み込みの過程の初期の、ブラウザの主なレンダリング機構が起動する前に、先読みを始めたいものを指定する宣言的なフェッチ要求を記述することができます。これにより、ページの最初のレンダリングがブロックされにくくなり、パフォーマンスが向上します。この記事では <code>preload</code> がどのように動作するのかについての基本的なガイドを提供します。</dd>
</dl>
</div>

<div class="section">
<h2 class="Documentation" id="References">リファレンス</h2>

<dl>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Reference">HTML リファレンス</a></dt>
 <dd class="landingPageList">HTML は<strong>要素</strong>の集まりで、それぞれの要素がいくつかの<strong>属性</strong>で修飾される場合があります。 HTML 文書は互いに<a href="/en-US/docs/Web/HTML/Link_types">リンク</a>で接続されます。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Element">HTML 要素リファレンス</a></dt>
 <dd class="landingPageList">すべての <a class="glossaryLink" href="/ja/docs/Glossary/HTML">HTML</a> <a class="glossaryLink" href="/ja/docs/Glossary/Element">要素</a>の一覧を閲覧します。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Attributes">HTML 属性リファレンス</a></dt>
 <dd class="landingPageList">HTML の要素には<strong>属性</strong>があります。これは要素を調整したり、さまざまな方法で振る舞いを調整したりするための付加的な値です。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Global_attributes">グローバル属性</a></dt>
 <dd class="landingPageList">グローバル属性は、<em>標準仕様で規定されていないものを含む</em>すべての <a href="/ja/docs/Web/HTML/Element">HTML 要素</a>に指定できるものです。つまり、あらゆる標準外の要素も、それを使用することで文書が HTML5 に準拠しなくなるとしても、グローバル属性を受け入れなければならないということです。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Inline_elements">インライン要素</a>と<a href="/ja/docs/Web/HTML/Block-level_elements">ブロックレベル要素</a></dt>
 <dd class="landingPageList">通常、 HTML の要素は「インライン」要素または「ブロックレベル」要素</a>のどちらかです。インライン要素は、要素を定義するタグによって指定された範囲のみを占有します。ブロックレベル要素は親要素（コンテナ）の範囲全体を占有し、それによって「ブロック」を作成します。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Link_types">リンクタイプ</a></dt>
 <dd class="landingPageList">HTML では、2つの文書の関係を確立し定義するためにさまざまな種類のリンクが使用できます。リンク要素は <a href="/ja/docs/Web/HTML/Element/a"><code>&lt;a&gt;</code></a>、 <a href="/ja/docs/Web/HTML/Element/area"><code>&lt;area&gt;</code></a>、 <a href="/ja/docs/Web/HTML/Element/link"><code>&lt;link&gt;</code></a> などで設定できます。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Supported_media_formats">HTML の audio 要素と video 要素で対応しているメディアフォーマット</a></dt>
 
 <dd class="landingPageList">The <a href="/ja/docs/Web/HTML/Element/audio"><code>&lt;audio&gt;</code></a> 要素と <a href="/ja/docs/Web/HTML/Element/video"><code>&lt;video&gt;</code></a> 要素で音声と映像のメディアを再生できます。これらの要素は、 Adobe Flash やその他のプラグインなどに見られる同様の機能をブラウザーネイティブの機能で代替します。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Content_categories">コンテンツのカテゴリ</a></dt>
 <dd class="landingPageList">HTML は数種類のコンテンツで構成され、それぞれのコンテンツは特定のコンテキストで使用することができ、他のコンテンツでは使用できません。同様に、それぞれのコンテンツを含むことができる一連の他のコンテンツカテゴリと、中で使用できる要素、使用できない要素があります。これは、これらのカテゴリのガイドです。</dd>
 <dt class="landingPageList"><a href="/ja/docs/Web/HTML/Quirks_Mode_and_Standards_Mode">後方互換モードと標準準拠モード</a></dt>
 <dd class="landingPageList">後方互換モードと標準準拠モードの歴史的な情報です。</dd>
</dl>

<h2 class="landingPageList" id="Related_topics">関連トピック</h2>

<dl>
 <dt><a href="/ja/docs/Web/HTML/Applying_color">CSSを使ってHTMLの要素に色をつける</a></dt>
 <dd>この記事では、CSS を使用して HTML コンテンツに色をつける方法、 HTML 文書のどの部分に色付けできるかの一覧、使用する CSS プロパティについて説明します。例えば、パレット作成ツールへのリンクなどが含みます。</dd>
</dl>
</div>
</div>
<span class="alllinks"><a href="/ja/docs/tag/HTML">すべて表示...</a></span>

<p>{{CommunityBox("Web layout", "dev-tech-layout", "mozilla.dev.tech.layout", "", "Stack Overflow|http://stackoverflow.com/questions/tagged/html|HTML に関する話題|協力体制で構築され維持されているQ&amp;Aサイトである Stack Overflow をご覧ください。答えが見つかるか確認してください。見つからない場合は、そちらで質問してください。")}}</p>
</section>

