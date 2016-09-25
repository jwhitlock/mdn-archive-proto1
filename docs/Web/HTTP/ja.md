---
version: prototype1
revision_id: 1123253
locale: ja
slug: Web/HTTP
tags: "HTTP" "Web" "Reference" "l10n:priority"
title: HTTP
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{HTTPSidebar}}</div>

<p class="summary"><strong><dfn>Hypertext Transfer Protocol (HTTP)</dfn></strong> は HTML などのハイパーメディアドキュメントを転送するための、<a href="https://ja.wikipedia.org/wiki/%E3%82%A2%E3%83%97%E3%83%AA%E3%82%B1%E3%83%BC%E3%82%B7%E3%83%A7%E3%83%B3%E5%B1%A4">アプリケーション層</a>プロトコルです。これはウェブブラウザーとウェブサーバーの間の通信用に設計されていますが、他の用途でも使用できます。HTTP は伝統的な<a href="https://ja.wikipedia.org/wiki/%E3%82%AF%E3%83%A9%E3%82%A4%E3%82%A2%E3%83%B3%E3%83%88%E3%82%B5%E3%83%BC%E3%83%90%E3%83%A2%E3%83%87%E3%83%AB">クライアントサーバーモデル</a>に従い、クライアントがコネクションを開き、リクエストを送信し、レスポンスを受け取るまで待ちます。また HTTP は<a href="http://en.wikipedia.org/wiki/Stateless_protocol">ステートレスプロトコル</a>であり、サーバーは 2 つのリクエストの間でいかなるデータ (状態) も保持しません。</p>

<p>HTTP は多くの場合 TCP/IP 層をベースにしますが、任意の信頼性がある<a href="https://ja.wikipedia.org/wiki/%E3%83%88%E3%83%A9%E3%83%B3%E3%82%B9%E3%83%9D%E3%83%BC%E3%83%88%E5%B1%A4">トランスポート層</a>プロトコル、すなわち暗黙のうちにメッセージを捨てないプロトコルで使用することもできます。</p>

<div class="column-container">
<div class="column-half">
<h2 id="Tutorials" name="Tutorials">チュートリアル</h2>

<p>ガイドやチュートリアルで、HTTP の使い方を学びましょう。</p>

<dl>
 <dt><a href="/ja/docs/Web/HTTP/Overview">HTTP の概要</a></dt>
 <dd>クライアントサーバープロトコルの基本機能を提供します。何ができるかや使用目的を説明します。</dd>
 <dt><a href="/ja/docs/Web/HTTP/Basics_of_HTTP/Evolution_of_HTTP">HTTP の進化</a></dt>
 <dd>初期バージョンの HTTP から HTTP/2 以降まで、HTTP で発生した変化を手短に説明します。</dd>
 <dt><a href="/ja/docs/Web/HTTP/Messages">HTTP メッセージ</a></dt>
 <dd>HTTP/1.x や HTTP/2 のさまざまなメッセージについて、タイプや構造を説明します。</dd>
 <dt><a href="/ja/docs/Web/HTTP/Session">典型的な HTTP セッション</a></dt>
 <dd>一般的な HTTP セッションを示して、フローを説明します。</dd>
 <dt><a href="/ja/docs/Web/HTTP/Connection_management_in_HTTP_1.x">HTTP/1.x のコネクション制御</a></dt>
 <dd>HTTP/1.x で使用できる 3 種類のコネクション制御モデルについて、長所や短所を説明します。</dd>
 <dt><a href="/ja/docs/Mozilla/HTTP_cache">HTTP キャッシュ</a></dt>
 <dd>キャッシュは、ウェブサイトの良好なパフォーマンスのために重要なツールです。この記事ではさまざまな種類のキャッシュや、HTTP ヘッダーでそれらを設定および制御する方法を説明します。</dd>
 <dt><a href="/ja/docs/Web/HTTP/Cookies">HTTP Cookies</a></dt>
 <dd>Cookie の動作は <a href="http://tools.ietf.org/html/rfc6265">RFC 6265</a> で定義しています。サーバーは HTTP リクエストを受け取ると、そのレスポンスで <code>Set-Cookie</code> ヘッダーを送信できます。その後クライアントは同一のサーバーに対するすべてのリクエストで、<code>Cookie</code> HTTP ヘッダーによって Cookie の値を返します。また、Cookie の有効期限を指定することができます。さらに、Cookie を特定のドメインやパスに限定することもできます。</dd>
 <dt><a href="/ja/docs/HTTP/Access_control_CORS">HTTP Access Control (CORS)</a></dt>
 <dd><strong>クロスサイト HTTP リクエスト</strong>とは、リクエストを出すリソースが存在するドメインとは<strong>異なるドメイン</strong>のリソースに対する HTTP リクエストを指します。例えば、ドメイン A (<code>http://domaina.example</code>) から読み込まれた HTML ウェブページなどから、<code>img</code> 要素を使用してドメイン B (<code>http://domainb.foo</code>) 上の画像 (<code>http://domainb.foo/image.jpg</code>) に対する HTTP リクエストが発行される、という状況を指します。このような状況は今日のウェブ上では非常にありふれたことであり、CSS スタイルシートや画像、スクリプトなどのさまざまなリソースがクロスサイト方式で読み込まれます。</dd>
 <dt><a href="/ja/docs/Web/HTTP/Controlling_DNS_prefetching">DNS プリフェッチの制御</a></dt>
 <dd>Firefox など、現代のほとんどのブラウザーは <strong>DNS プリフェッチ</strong>を行います。これはユーザーがたどるであろうリンクや、ドキュメントが参照する画像、CSS、JavaScript といったリソースのドメイン名解決をブラウザーが事前に行うことです。このプリフェッチはバックグラウンドで行いますので、参照先のアイテムをリクエストするときには、すでに DNS 名前解決が完了しているでしょう。これにより、例えばユーザーが実際にリンクをクリックするときのレイテンシを低減します。</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Reference" name="Reference">リファレンス</h2>

<p>詳細な HTTP リファレンスドキュメントを見ていきましょう</p>

<dl>
 <dt><a href="/ja/docs/Web/HTTP/Headers">HTTP ヘッダー</a></dt>
 <dd>HTTP メッセージヘッダーはリソース、あるいはサーバーやクライアントの動作を精密に示すために使用します。プロプライエタリーなカスタムヘッダーは、'X-' 接頭辞を使用して追加できます。それ以外のヘッダーは <a href="http://www.iana.org/assignments/message-headers/perm-headers.html">IANA レジストリー</a> に収録されており、<a href="http://tools.ietf.org/html/rfc4229">RFC 4229</a> が基になっています。また IANA は <a href="http://www.iana.org/assignments/message-headers/prov-headers.html">新たに提案された HTTP ヘッダのレジストリー</a> も管理しています。</dd>
 <dt><a href="/ja/docs/Web/HTTP/Methods">HTTP リクエストメソッド</a></dt>
 <dd>HTTP では {{HTTPMethod("GET")}} や {{HTTPMethod("POST")}} だけでなく、{{HTTPMethod("OPTIONS")}} や {{HTTPMethod("DELETE")}} や {{HTTPMethod("TRACE")}} などのあまり一般的ではないリクエストを含む、さまざまな操作を行うことができます。</dd>
 <dt><a href="/ja/docs/Web/HTTP/Response_codes">HTTP ステータスレスポンスコード</a></dt>
 <dd>HTTP レスポンスコードは、特定の HTTP リクエストが正常に完了したかを示します。レスポンスは情報レスポンス、成功レスポンス、リダイレクション、クライアントエラー、サーバーエラーの 5 つのクラスに分類されます。</dd>
</dl>

<h2 id="Tools_resources" name="Tools_resources">ツールとリソース</h2>

<p>HTTP コネクションの使用やデバッグに役立つツールです。</p>

<dl>
 <dt><a href="/ja/docs/Tools">Firefox 開発ツール</a></dt>
 <dd><a href="/ja/docs/Tools/Network_Monitor">ネットワークモニター</a></dd>
 <dt><a href="https://redbot.org/">RedBot</a></dt>
 <dd>キャッシュ関係のヘッダーを確認するツールです。</dd>
 <dt><a href="http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/">How Browsers Work</a> (<a href="http://www.html5rocks.com/ja/tutorials/internals/howbrowserswork/">日本語版</a>)</dt>
 <dd>ブラウザの内部処理や HTTP プロトコルのリクエストのフローに関する、とても包括的な記事です。すべてのウェブ開発者が読むべき記事です。</dd>
 <dt>&nbsp;</dt>
 <dt>&nbsp;</dt>
 <dt>&nbsp;</dt>
</dl>
</div>
</div>

