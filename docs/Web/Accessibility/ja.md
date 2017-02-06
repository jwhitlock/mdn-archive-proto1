---
version: prototype1
revision_id: 1183211
locale: ja
slug: Web/Accessibility
tags: "Landing" "Advanced" "Accessibility" "Web Development"
title: Accessibility
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p><span class="seoSummary">ウェブ開発におけるアクセシビリティとは、何らかの理由により能力に制約がある場合でも、可能な限り多くの人々がウェブサイトを使用できるようにすることを意味します。この記事では、アクセシビリティを考慮したコンテンツを開発するための情報を提供します。</span></p>

<p>"アクセシビリティは "車椅子対応" のように障害を持つ人々を支援する設備や施設を説明するためによく利用されます。これが指し示すものは、点字表示、車椅子用傾斜路、横断歩行者用音声信号、歩道標識、ウェブサイトのデザインなどにも広げられます。" {{Ref(1)}}</p>

<p>"ハードウェア、ソフトウェア、言語、文化、所在地、物理的/精神的能力にかかわらず、<strong>ウェブは基本的にすべての人に向けて設計されています</strong>。ウェブがこの目的を達成できると、さまざまな聴力、視力、認知能力をもつ人々がウェブにアクセスできるようになります。" {{ Ref(2) }}</p>


<div class="cleared topicpage-table">
<div class="section">
<h2 name="Key_accessibility_tutorials" class="Key_accessibility_tutorials" id="Key_accessibility_tutorials">主なアクセシビリティのチュートリアル</h2>

<p>MDN の<a href="/ja/docs/Learn/Accessibility">アクセシビリティ学習エリア</a>には、アクセシビリティの基本事項を含むモダンな最新のチュートリアルが含まれています:</p>

<dl>
 <dt><a href="/ja/docs/Learn/Accessibility/What_is_accessibility">アクセシビリティとは何か？</a></dt>
 <dd>この記事では、アクセシビリティが実際にどのようなものであるかをよく見てモジュールを開始します。これには、どのグループを考慮する必要があるのかとそのグループの理由、さまざまな人々がウェブとやりとりするために使用するツール、アクセシビリティをウェブ開発ワークフローの一部にする方法を含みます。</dd>
 <dt><a href="/ja/docs/Learn/Accessibility/HTML">HTML: アクセシビリティのための良い基礎</a></dt>
 <dd>適切な HTML 要素が常に正しい目的で使用されていることを確認するだけで、大量のウェブコンテンツをアクセシブルにすることができます。この記事では、最大限のアクセシビリティを確保するために HTML をどのように使用できるかについて詳しく説明します。</dd>
 <dt><a href="/ja/docs/Learn/Accessibility/CSS_and_JavaScript">CSS と JavaScript のアクセシビリティベストプラクティス</a></dt>
 <dd>CSS と JavaScript を適切に使用すると、アクセシブルなウェブ体験を可能にするポテンシャルがあります。また、悪用されるとアクセシビリティに大きな悪影響を与える可能性があります。この記事では、複雑なコンテンツでさえも可能な限りアクセシブルであることを保証するために考慮する必要がある CSS と JavaScript のベストプラクティスの概要を説明します。</dd>
 <dt><a href="/ja/docs/Learn/Accessibility/WAI-ARIA_basics">WAI-ARIA の基礎</a></dt>
 <dd>前の記事に従って、セマンティックでない HTML や動的に JavaScript で更新されたコンテンツを含む複雑なUIコントロールを作成することは理解しづらい場合があります。WAI-ARIA は、ブラウザーや支援技術が認識して使用できるセマンティクスを追加することで、このような問題の解決に役立つ技術です。ここでは、アクセシビリティを向上させるために基本レベルで使用する方法を示します。</dd>
 <dt><a href="/ja/docs/Learn/Accessibility/Multimedia">アクセシブルなマルチメディア</a></dt>
 <dd>アクセシビリティの問題を引き起こす可能性のある別のカテゴリーのコンテンツは、マルチメディアです。映像、音声、および画像のコンテンツには、補助的なテクノロジーとそのユーザーが理解できるように適切なテキストの代替が必要です。この記事では、その方法を示します。</dd>
 <dt><a href="/ja/docs/Learn/Accessibility/Mobile">モバイルアクセシビリティ</a></dt>
 <dd>モバイル端末でのウェブアクセスが普及しており、iOS や Android などの普及しているプラットフォームではアクセシビリティツールが完全に提供されているため、これらのプラットフォームでのウェブコンテンツのアクセシビリティを考慮する必要があります。この記事では、モバイル固有のアクセシビリティの考慮事項について説明します。</dd>
</dl>

<p> </p>
</div>


<div class="section">
<h2 name="Other_documentation" class="Other_documentation" id="Other_documentation">他の文書</h2>

<dl>
 <dt><a href="/ja/docs/Accessibility/Web_Development">ウェブ開発</a></dt>
 <dd>アクセシビリティの世界での Web 開発の問題点をハイライトした記事のコレクション</dd>
 <dt><a href="/ja/docs/Accessibility/ARIA">ARIA</a></dt>
 <dd>ARIAを使用してHTML文書をより使いやすくする方法を学ぶための記事のコレクション。</dd>
 <dt><a href="/ja/docs/Accessibility/AT_Development">支援技術 (AT) 開発</a></dt>
 <dd>支援技術の開発者向け記事のコレクション</dd>
 <dt><a href="/ja/docs/Web/Accessibility/Mobile_accessibility_checklist">モバイルアクセシビリティチェックリスト</a></dt>
 <dd>このドキュメントは、モバイルアプリ開発者向けのアクセシビリティ要求事項の簡潔なチェックリストを提供します。</dd>
</dl>

<p><span class="alllinks"><a href="/ja/docs/tag/Accessibility">アクセシビリティについてのすべての記事を見る...</a></span></p>

<p> </p>
</div>
 

<p><br>
  </p>
</div>



<p>{{ endnote(1) }} <a class="external" href="http://en.wikipedia.org/wiki/Accessibility">Wikipedia</a> から (英語版)</p>

<p>{{ endnote(2) }} <a href="http://www.w3.org/standards/webdesign/accessibility">W3C - Accessibility</a> から (英語版)</p>

<p>{{CommunityBox("Accessibility", "accessibility", "mozilla.accessibility", "accessibility", "Other links|http://www.w3.org/WAI/IG/|WAI Interest Group|Web Accessibility Interest Group web site++https://mozillians.org/group/1-accessibility|Mozilla accessibility community directory|Mozillians members interested in accessibility++/docs/Web/Accessibility/Community|Other community links...|Links to other accessibility community sites")}}</p>

<p>{{MakeSimpleQuicklinks("/ja/docs/Web_Development", "/ja/docs/Web_Standards", "/ja/docs/XUL", "/ja/docs/Mozilla/Accessibility")}}</p>

