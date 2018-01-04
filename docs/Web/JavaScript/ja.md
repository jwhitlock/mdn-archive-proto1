---
version: prototype1
revision_id: 1342276
locale: ja
slug: Web/JavaScript
tags: "Learn" "Landing" "JavaScript"
title: JavaScript
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{JsSidebar}}</div>

<p class="summary"><strong>JavaScript</strong> (JS) は軽量で、インタプリタ型の、<a href="https://ja.wikipedia.org/wiki/%E7%AC%AC%E4%B8%80%E7%B4%9A%E9%96%A2%E6%95%B0">第一級関数</a>を備えたプログラミング言語です。Web ページでよく使用されるスクリプト言語として知られ、<a href="https://nodejs.org/">node.js</a> や <a href="https://couchdb.apache.org/">Apache CouchDB</a> といった<a href="http://en.wikipedia.org/wiki/JavaScript#Uses_outside_Web_pages">多くの非ブラウザ環境においても使用されています</a>。 JavaScript は <a href="https://en.wikipedia.org/wiki/Prototype-based_programming">プロトタイプベース</a>で、動的型付けを持ち、そしてオブジェクト指向、命令形、そして関数プログラミングといったスタイルをサポートするマルチパラダイムのスクリプト言語です。詳しくは <a href="/ja/docs/Web/JavaScript/About_JavaScript">JavaScript について</a>をお読みください。</p>

<p>このセクションでは JavaScript 言語自体について、すなわち Web ページ他の環境に限定されないコアの部分について専門に解説しています。Web ページ特有の {{Glossary("API","API")}} 群の情報を得たい場合は <a href="/ja/docs/Web/API">Web APIs</a> と <a href="/ja/docs/DOM">DOM</a> を参照してください。</p>

<p>JavaScript の標準仕様は <a href="/ja/docs/Web/JavaScript/Language_Resources">ECMAScript</a> と呼ばれています。2012年現在、全てのモダンブラウザは ECMAScript 5.1 を完全にサポートしています。過去のブラウザも、少なくとも ECMAScript 3 はサポートしています。2015 年 6 月 17 日、<a href="https://www.ecma-international.org/">ECMA International</a> はECMAScript のメジャーバージョン 6 を策定しました。このバージョンは公式には ECMAScript 2015 と呼ばれていますが、通常は ECMAScript 6 や ES6 と呼ばれます。それ以降、ECMAScript 標準は年単位でリリースされています。このドキュメントは最新のドラフトバージョン、現在は&nbsp;<a href="https://tc39.github.io/ecma262/">ECMAScript 2018</a> を参照しています。</p>

<p>JavaScript を<a href="https://ja.wikipedia.org/wiki/Java">プログラミング言語 Java</a> と混同しないでください. Java と JavaScript は両方ともアメリカやその他の国においてオラクルの商標または登録商標です。しかし、この 2 つのプログラミング言語は非常に異なる構文、セマンティック、利用形態を持っています。</p>

<div class="column-container">
<div class="column-half">
<h2 id="チュートリアル">チュートリアル</h2>

<p>ガイドやチュートリアルを使って JavaScript をプログラムする方法を学びましょう。</p>

<h3 id="初心者向け" name="初心者向け">完全な初心者向け</h3>

<p>JavaScript について学びたいと思っているが、JavaScript あるいはプログラミングについて過去に経験がないのであれば、<a href="/ja/docs/Learn/JavaScript">JavaScript 学習エリア</a>に向かいましょう。次のモジュールが利用可能です。</p>

<dl>
 <dt><a href="/ja/docs/Learn/JavaScript/First_steps">JavaScript の第一歩</a></dt>
 <dd>変数、文字列、数値、配列のような鍵となる JavaScript の機能のディスカッションに加え、　「JavaScript とは何か」「何に似ているか」「何ができるか」といった基本的な質問に答えます。</dd>
 <dt><a href="/ja/docs/Learn/JavaScript/Building_blocks">JavaScript の構成要素</a></dt>
 <dd>条件分岐、ループ、関数、イベントなどのよく目にするタイプのコードブロックに注意を向け、引き続き JavaScript の鍵となる基本機能について説明します。</dd>
 <dt>
 <h3>JavaScript ガイド</h3>
 </dt>
</dl>

<dl>
 <dt><a href="/ja/docs/Web/JavaScript/Guide">JavaScript ガイド</a></dt>
 <dd>JavaScript、または他のプログラミング言語の経験がある人に向けた、JavaScript のより詳細なガイド。</dd>
</dl>

<h3 id="中級者向け" name="中級者向け">中級者向け</h3>

<dl>
 <dt><a href="/ja/docs/Learn/JavaScript/Objects">JavaScript オブジェクトの紹介</a></dt>
 <dd>言語に関する知識をさらに深め、より効率的なコードを書きたいのであれば、JavaScript のオブジェクト指向の性質を理解することは重要です。そこで、私たちが提供するこのモジュールが役立つでしょう。</dd>
 <dt><a href="https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs">クライアントサイド Web&nbsp;API</a></dt>
 <dd>Web サイトや Web アプリケーションのためにクライアントサイドの JavaScript を記述するとき、API — Web サイト、あるいは他の Web サイトや Web サービスからのデータを実行する、異なるブラウザや OS を操作するためのインターフェース — を使い始める前に、そう遠くへは行かないでしょう。このモジュールでは API とは何か、それをどのように使うかについて、開発の中でしばしば出遭ういくつかの最も一般的な API を通じて説明します。</dd>
 <dt><a href="/ja/docs/Web/JavaScript/A_re-introduction_to_JavaScript">JavaScript 「再」入門</a></dt>
 <dd>JavaScript なら知ってるよ、と思っている方々に送る概説。</dd>
</dl>

<dl>
 <dt><a href="/ja/docs/Web/JavaScript/Data_structures">JavaScript のデータ構造</a></dt>
 <dd>JavaScript で利用できるデータ構造の概覧.</dd>
 <dt><a href="/ja/docs/Web/JavaScript/Equality_comparisons_and_sameness">等値比較と同一性</a></dt>
 <dd>JavaScript には3つの異なる値の比較演算子があります: <code>===</code> を使う厳格な等値性比較、<code>==</code> を使う寛容な等値性比較、そして {{jsxref("Global_Objects/Object/is", "Object.is()")}} メソッド。</dd>
</dl>

<h3 id="上級者向け" name="上級者向け">上級者向け</h3>

<dl>
 <dt><a href="/ja/docs/Web/JavaScript/Inheritance_and_the_prototype_chain">継承とプロトタイプチェーン</a></dt>
 <dd>プロトタイプベースの継承にまつわるよくある誤解と過小評価に対する説明。</dd>
 <dt><a href="/ja/docs/Web/JavaScript/Reference/Strict_mode">Strict モード</a></dt>
 <dd>JavaScript の厳格版。</dd>
 <dt><a href="/ja/docs/Web/JavaScript/Typed_arrays">JavaScript 型付き配列</a></dt>
 <dd>JavaScript の型付き配列は未加工のバイナリデータにアクセスするメカニズムを提供します。</dd>
 <dt><a href="/ja/docs/Web/JavaScript/Memory_Management">メモリ管理</a></dt>
 <dd>JavaScript におけるメモリのライフサイクルとガベージコレクション。</dd>
 <dt><a href="/ja/docs/Web/JavaScript/EventLoop">並列モデルとイベントループ</a></dt>
 <dd>JavaScript は「イベントループ」に基づく並列モデルを持っています。</dd>
</dl>
</div>

<div class="column-half">
<h2 id="リファレンス" name="リファレンス">リファレンス</h2>

<p>すべてを網羅した <a href="/ja/docs/Web/JavaScript/Reference">JavaScript リファレンス</a> ドキュメントを閲覧できます。</p>

<dl>
 <dt><a href="/ja/docs/Web/JavaScript/Reference/Global_Objects">標準オブジェクト</a></dt>
 <dd>{{jsxref("Array")}}、 {{jsxref("Boolean")}}、 {{jsxref("Date")}}, {{jsxref("Error")}}、 {{jsxref("Function")}}、 {{jsxref("JSON")}}、 {{jsxref("Math")}}、 {{jsxref("Number")}}、 {{jsxref("Object")}}、 {{jsxref("RegExp")}}、 {{jsxref("String")}}、 {{jsxref("Map")}}、 {{jsxref("Set")}}、 {{jsxref("WeakMap")}}、 {{jsxref("WeakSet")}} などの標準ビルトインオブジェクトについて理解しましょう。</dd>
 <dt><a href="/ja/docs/Web/JavaScript/Reference/Operators">式と演算子</a></dt>
 <dd>{{jsxref("Operators/instanceof", "instanceof")}}、 {{jsxref("Operators/typeof", "typeof")}}、 {{jsxref("Operators/new", "new")}}、 {{jsxref("Operators/this", "this")}} といった JavaScript における演算子の挙動、そして<a href="/en-US/docs/Web/JavaScript/Reference/Operators/Operator_Precedence">演算子の優先順位</a>などについて学びましょう。</dd>
 <dt><a href="/ja/docs/Web/JavaScript/Reference/Statements">文と宣言</a></dt>
 <dd>{{jsxref("Statements/var", "var")}}、{{jsxref("Statements/let", "let")}}、&nbsp;{{jsxref("Statements/const", "const")}}、&nbsp;{{jsxref("Statements/function", "function")}}、{{jsxref("Statements/return", "return")}}、 {{jsxref("Statements/if...else", "if...else")}}、{{jsxref("Statements/try...catch", "try-catch")}}、 {{jsxref("Statements/switch", "switch")}}、{{jsxref("Statements/do...while", "do-while")}}、{{jsxref("Statements/for", "for")}}、&nbsp;{{jsxref("Statements/for...in", "for-in")}}、 {{jsxref("Statements/for...of", "for-of")}}<span style="display:none">&nbsp;</span>&nbsp;などの JavaScript の文やキーワードがどのように機能するか学びましょう。</dd>
 <dt><a href="/ja/docs/Web/JavaScript/Reference/Functions">関数</a></dt>
 <dd>アプリケーション開発においてJavaScriptの関数を扱う方法については、こちらをご覧ください。</dd>
</dl>

<h2 id="ツールとリソース" name="ツールとリソース">ツールとリソース</h2>

<p>JavaScript コードを書き、デバッグするのに役立つツールたち。</p>

<dl>
 <dt><a href="/ja/docs/Tools">Firefox 開発ツール</a></dt>
 <dd><a href="/ja/docs/Tools/Scratchpad">スクラッチパッド</a>、<a href="/ja/docs/Tools/Web_Console">Web コンソール</a>、<a href="/ja/docs/Tools/Profiler">JavaScript プロファイラ</a>、<a href="/ja/docs/Tools/Debugger">デバッガ</a>など。</dd>
 <dt><a href="/ja/docs/Web/JavaScript/Shells">JavaScript シェル</a></dt>
 <dd>ちょっとした JavaScript のコードを簡単にテストできる&nbsp;JavaScript シェル。</dd>
 <dt><a href="https://togetherjs.com/">TogetherJS</a></dt>
 <dd>
 <p>簡単にリアルタイムコラボレーションを行えるライブラリ。TogetherJS をサイトに追加することで、ユーザーがウェブサイト上でリアルタイムに助け合えるようになります。</p>
 </dd>
 <dt><a href="http://stackoverflow.com/questions/tagged/javascript">Stack Overflow</a></dt>
 <dd>"JavaScript" のタグが付いた Stack Overflow の質問一覧ページ。</dd>
 <dt><a href="/ja/docs/Web/JavaScript/New_in_JavaScript">JavaScript のバージョンとリリースノート</a></dt>
 <dd>JavaScript 機能の歴史と実装状況について。</dd>
 <dt><a href="https://jsfiddle.net/">JSFiddle</a></dt>
 <dd>JavaScript、CSS、HTML を編集し、リアルタイムで実行結果を表示できるサイト。外部リソースを使い、オンライン上でチームと共同作業が行えます。</dd>
 <dt><a href="https://plnkr.co/">Plunker</a></dt>
 <dd>Plunker は Web 開発のアイデアを作成、共同作業、共有するためのオンラインコミュニティです。JavaScript や CSS、HTML ファイルを編集し、ライブでの実行結果やファイル構造を取得することができます。</dd>
</dl>
</div>
</div>

<p>{{CommunityBox("JavaScript", "js-engine.internals", "mozilla.dev.tech.js-engine.internals", "js", "ES discuss|https://esdiscuss.org/|esdiscuss.org|ECMAScript standard discussion mailing list||SpiderMonkey|https://wiki.mozilla.org/JavaScript|Project page|Contribute to the JavaScript Engine||Twitter|https://twitter.com/SpiderMonkeyJS|@SpiderMonkeyJS|SpiderMonkey updates on Twitter")}}</p>

