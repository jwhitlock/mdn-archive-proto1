---
version: prototype1
revision_id: 1328139
locale: ja
slug: MDN/Contribute/Localize
tags: "l10n" "MDN Meta" "Landing" "Localization"
title: MDN でのローカライズ
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{IncludeSubnav("/ja/docs/MDN")}}</div>

<p>MDN は世界中の人々から、Firefox そのものと同様に、ウェブテクノロジーのリファレンスおよびガイドとして、使われています。ローカライズコミュニティは Mozilla プロジェクトの中で重要な役割を果たしています。コミュニティによる文書の翻訳および各国言語への対応が、世界各地の人々がオープンなウェブを開発する上で役に立っています。ローカライズについてもっとよく知りたい場合や、新しい言語のローカライズを開始したい場合は、ここがスタート地点です。</p>

<h2 id="Types_of_localization_on_MDN" name="Types_of_localization_on_MDN">ローカライズの種類</h2>

<p>MDN でのローカライズは、必要とするシステムや権限によって 3 つに分けることができます。</p>

<dl>
 <dt>MDN サイトのユーザーインターフェイス</dt>
 <dd>各々の MDN 記事で表示され、記事本文の場所を示したり、ナビゲーション機能やユーザーコントロールで使われる文字列です。これらの文字列は <a href="https://pontoon.mozilla.org/project">MDN プロジェクト</a> にある Mozilla の <a href="https://developer.mozilla.org/ja/docs/Mozilla/Localization/Localizing_with_Pontoon">Pontoon</a> システムで翻訳することができます。もしお使いの言語が MDN になければ、Pontoon の管理者が有効化する必要があります。<a href="/ja/docs/MDN/Contribute/Localize/Starting_a_localization">MDN のローカライゼーションを開始する</a> を参照してください。</dd>
 <dt>MDN 記事</dt>
 <dd>リファレンス、ガイド、チュートリアルといった MDN 記事の本文です。これらの記事は <a href="https://developer.mozilla.org/ja/docs/MDN/Contribute/Localize/Translating_pages">MDN に組み込まれた翻訳機能</a> を使って翻訳します。翻訳先の言語一覧にお使いの言語がない場合、<a href="https://developer.mozilla.org/ja/docs/MDN/Contribute/Localize/Starting_a_localization">MDN のローカライゼーションを開始する</a> を参照してください。</dd>
</dl>

<dl>
 <dt>マクロ文字列</dt>
 <dd>これらの文字列は<a href="https://developer.mozilla.org/ja/docs/MDN/Contribute/Structures/Macros">マクロテンプレート</a> によって出力され、ナビゲーションやメッセージ、文章構造を構築します。テンプレートの編集は広い範囲に破壊的な影響を及ぼすことが考えられるため、編集には <a href="https://developer.mozilla.org/ja/docs/MDN/Contribute/Tools/Template_editing">特別なアクセス権</a> が必要です。この権限を持っていない場合は、あなたが翻訳した文字列を権限を持った人に伝え、適用を依頼してください。</dd>
</dl>

<p>以下のページでは、MDN 上の翻訳についてより詳しく説明しています:</p>

<p>{{LandingPageListSubpages}}</p>

<h2 id="Localization_communities_on_MDN" name="Localization_communities_on_MDN">MDN 上の翻訳コミュニティ</h2>

<p>MDN の翻訳活動は、個人が独立しても (大半の Mozilla 翻訳コミュニティがしているでしょう)、グループで一緒にでも、どちらでも活動できます。MDN の翻訳プロジェクトは、 <strong>翻訳ドライバー</strong>によってリードされています。</p>

<ul>
 <li><a href="https://developer.mozilla.org/ja/docs/MDN/Contribute/Localize/Localization_projects">Localization projects</a></li>
 <li><a href="https://developer.mozilla.org/ja/docs/MDN/Community/Roles/Localization_driver_role">Localization driver role</a></li>
</ul>

<h2 id="Localization_tools" name="Localization_tools">ローカライズのためのツール</h2>

<p>ローカライズの作業で使われる、便利なツールをいくつか紹介します:</p>

<dl>
 <dt><a href="/ja/docs/Mozilla/Localization/Localizing_with_Pontoon" title="/ja/docs/Mozilla/Localization/Localizing_with_Verbatim">Pontoon</a></dt>
 <dd>文字列を翻訳するためのもので、Mozilla の複数のプロジェクトにまたがって使われます。MDN のユーザーインターフェイス (そして Firefox のユーザーインターフェイス) も対象です。</dd>
 <dt><a href="http://transvision.mozfr.org/" title="http://transvision.mozfr.org/">Transvision</a></dt>
 <dd>French Mozilla community によって提供されるユーテリティで、ある英語文字列の存在を Mozilla のプログラムコード全体から検索し、また目的の言語への様々な翻訳を見つけるのに使用できます。単語、フレーズの適切な訳 (定訳) を探すのに便利です。</dd>
</dl>

<h2 id="See_also" name="See_also">関連項目</h2>

<ul>
 <li><a href="/ja/docs/Mozilla/Localization" title="/ja/docs/Mozilla/Localization">Mozilla でのローカライゼイション</a></li>
</ul>

