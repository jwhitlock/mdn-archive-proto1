---
version: prototype1
revision_id: 1041264
locale: ja
slug: Web/MathML
tags: "XML" "Web" "MathML" "Landing" "Reference"
title: MathML
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p><strong>Mathematical Markup Language (MathML)</strong> は、数学的表記を記述し、その構造と内容を表現するための <a href="/docs/XML" title="/docs/XML">XML</a> マークアップ言語です。このページには、MathML のパワフルな技術を用いた仕事を助けるための文書、サンプル、ツールへのリンクがあります。簡単な概要は、<a href="http://fred-wang.github.io/MozSummitMathML/index.html">Mozilla Summit 2013 で行われた innovation fair 向けのスライド</a> をご覧ください。</p>

<div class="row topicpage-table">
<div class="section">
<h2 id="MathML_reference">MathML リファレンス</h2>

<dl>
 <dt><a href="/docs/Web/MathML/Element">MathML 要素リファレンス</a></dt>
 <dd>各 MathML 要素の詳細とデスクトップおよびモバイルのブラウザの互換性情報。</dd>
 <dt><a href="/docs/Web/MathML/Attribute">MathML 属性リファレンス</a></dt>
 <dd>MathML 要素の見た目や振る舞いを変更する MathML 属性についての情報。</dd>
 <dt><a href="/docs/Web/MathML/Examples">MathML の例</a></dt>
 <dd>MathML の動作についての理解を深めるためのサンプルと例。</dd>
 <dt><a href="/docs/Web/MathML/Authoring">MathML の書き方</a></dt>
 <dd>MathML を書くための提案とヒント、おすすめの MathML エディタ、その出力を Web コンテンツへ統合する方法。</dd>
</dl>

<p><a href="/ja/docs/tag/MathML">すべて見る...</a></p>
</div>

<div class="section">
<h2 id="Getting_help_from_the_community">コミュニティから助けを得る</h2>

<ul>
 <li>Mozilla のフォーラムを見る<br>
  {{ DiscussionList("dev-tech-mathml", "mozilla.dev.tech.mathml") }}</li>
 <li><a class="link-irc" href="irc://irc.mozilla.org/%23mathml" rel="external" title="#mathml">IRC チャンネル</a></li>
 <li><a class="link-https" href="https://wiki.mozilla.org/MathML:Home_Page">Mozilla 貢献者の使う Wiki</a></li>
 <li><a href="http://www.w3.org/Math/">W3C Math Home</a></li>
 <li><a href="http://lists.w3.org/Archives/Public/www-math/">www-math w3.org メールアーカイブ</a></li>
</ul>

<h2 id="Tools">ツール</h2>

<ul>
 <li><a class="external" href="http://validator.w3.org">W3C Validator</a></li>
 <li><a class="link-https" href="https://addons.mozilla.org/firefox/addon/8969/">FireMath Firefox アドオン</a></li>
 <li><a href="https://addons.mozilla.org/firefox/collections/fred_wang/mathzilla/">Mathzilla Firefox アドオンコレクション</a></li>
 <li><a href="https://github.com/fred-wang/TeXZilla">TeXZilla</a> — Javascript で書かれた LaTeX から MathML へのコンバータ (<a href="http://fred-wang.github.io/TeXZilla/">ライブデモ</a>、<a href="http://r-gaia-cs.github.io/TeXZilla-webapp/">Firefox OS ウェブアプリ</a>、<a href="https://addons.mozilla.org/firefox/addon/texzilla/">Firefox アドオン</a>、<a href="https://github.com/fred-wang/TeXZilla/wiki/Using-TeXZilla">Web ページやJS プログラム内での使用</a>)</li>
 <li><a href="http://dlmf.nist.gov/LaTeXML/">LaTeXML</a> - LaTeX ドキュメントを HTML+MathML Web ページへ変換</li>
 <li><a href="http://webdemo.myscript.com/#/demo/equation">Web Equation</a> - 手書きの数式を MathML や LaTeX へ変換</li>
 <li><a href="http://www.mathjax.org/">MathJax</a> - 数式のためのクロスブラウザ JavaScript 表示エンジン。Mathjax をネイティブ MathML で使用するには、<a href="https://addons.mozilla.org/ja/firefox/addon/mathjax-native-mathml/">Mozilla アドオン</a>、<a href="http://fred-wang.github.io/mathjax-native-mathml-safari/mathjax-native-mathml.safariextz">Safari 拡張</a>、<a href="https://openuserjs.org/scripts/fred.wang/MathJax_Native_MathML/">GreaseMonkey スクリプト</a> を試してください。</li>
</ul>

<h2 id="Related_topics">関連トピック</h2>

<ul>
 <li><a href="/docs/Web/CSS">CSS</a></li>
 <li><a href="/docs/Web/HTML">HTML</a></li>
 <li><a href="/docs/Web/SVG">SVG</a></li>
</ul>
</div>
</div>

<h2 id="Browser_compatibility">ブラウザの実装状況</h2>

<p>{{CompatibilityTable}}</p>

<div id="compat-desktop">
<table class="compat-table">
 <tbody>
  <tr>
   <th>機能</th>
   <th>Chrome</th>
   <th>Firefox (Gecko)</th>
   <th>Internet Explorer</th>
   <th>Opera</th>
   <th>Safari</th>
  </tr>
  <tr>
   <td>基本サポート</td>
   <td>{{CompatNo}} [1]</td>
   <td>{{CompatGeckoDesktop("1.8")}}</td>
   <td>{{CompatNo}} [1]</td>
   <td>{{CompatNo}} [1]</td>
   <td>{{CompatSafari(5.1)}}</td>
  </tr>
 </tbody>
</table>
</div>

<div id="compat-mobile">
<table class="compat-table">
 <tbody>
  <tr>
   <th>機能</th>
   <th>Android</th>
   <th>Firefox Mobile (Gecko)</th>
   <th>IE Mobile</th>
   <th>Opera Mobile</th>
   <th>Safari Mobile</th>
  </tr>
  <tr>
   <td>基本サポート</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatGeckoMobile("1.8")}}</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatUnknown}}</td>
   <td>5.1</td>
  </tr>
 </tbody>
</table>
</div>

<p>[1] プラグインを使用して利用できます。</p>

