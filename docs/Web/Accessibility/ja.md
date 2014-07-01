---
version: prototype1
revision_id: 630127
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
<div>{{outdated("")}}</div>

<div>
  <p>"アクセシビリティーは "車椅子対応" のように障碍を持つ人々を支援する設備や施設を説明するためによく利用されます。これが指し示すものは、点字表示、車椅子用傾斜路、横断歩行者用音声信号、歩道標識、ウェブサイトデザインなどにも広げられます。" {{Ref(1)}}</p>
</div>
<table class="topicpage-table">
  <tbody>
    <tr>
      <td>
        <h2 class="Documentation" id=".E3.83.89.E3.82.AD.E3.83.A5.E3.83.A1.E3.83.B3.E3.83.88" name=".E3.83.89.E3.82.AD.E3.83.A5.E3.83.A1.E3.83.B3.E3.83.88"><a href="Special:Tags?tag=Accessibility&amp;language=ja">ドキュメント</a></h2>
        <div>
          {{英語版章題("Introduction")}}</div>
        <h3 id=".E5.85.A5.E9.96.80" name=".E5.85.A5.E9.96.80">入門</h3>
        <dl>
          <dt>
            <a class="external" href="http://www.mozilla-japan.org/access/today">ソフトウェアアクセシビリティーの現在</a> (<a class="external" href="http://www.mozilla.org/access/today">原文</a>)</dt>
          <dd>
            コンピュータソフトウェアのアクセシビリティーは、ここ 20 年で大きく改善されました。この記事では、その進展とどのように技術が開発されてきたかについて概説します。</dd>
          <dt>
            <a class="external" href="http://www.fliedlice.com/dive/">アクセシビリティーへ飛び込む</a> (<a class="external" href="http://diveintoaccessibility.org/">原文</a>)</dt>
          <dd>
            この本では二つの疑問に答えます。一つ目は「なぜウェブサイトをよりよいアクセシビリティーを持つよう作らなければならないのか」、二つ目は「どうすればわたしのウェブサイトをよりよいアクセシビリティーをもつようにできるか」です。</dd>
          <dt>
            <a class="external" href="http://www-06.ibm.com/jp/accessibility/guideline/accessweb.html">アクセシビリティーを満たすウェブページの制作</a> (<a class="external" href="http://www-306.ibm.com/able/guidelines/web/accessweb.html">原文</a>)</dt>
          <dd>
            IBM による便利なウェブアクセシビリティーチェックリストです。</dd>
        </dl>
        <div>
          {{英語版章題("Guidelines")}}</div>
        <h3 id=".E3.82.AC.E3.82.A4.E3.83.89.E3.83.A9.E3.82.A4.E3.83.B3" name=".E3.82.AC.E3.82.A4.E3.83.89.E3.83.A9.E3.82.A4.E3.83.B3">ガイドライン</h3>
        <dl>
          <dt>
            <a href="ja/docs/Accessibility/Architecture">Accessibility:Architecture</a></dt>
          <dd>
            Mozilla におけるアクセシビリティ階層の実装。</dd>
          <dt>
            <a href="ja/docs/Building_accessible_custom_components_in_XUL">Building accessible custom components in XUL</a></dt>
          <dd>
            カスタム XUL コンポーネントにアクセシビリティを追加する DHTML アクセシビリティ技術の利用方法。</dd>
          <dt>
            <a href="ja/docs/Accessible_XUL_Authoring_Guidelines">アクセシブルな XUL 記述のためのガイドライン</a></dt>
          <dd>
            これらのガイドラインに基づいて記述すれば、XUL はアクセシビリティーを満たすユーザインターフェースを生成することができます。コード作成者、レビュー担当者、デザイナー、QA エンジニアは、これらのガイドラインを熟知しておくべきです。</dd>
          <dt>
            <a class="external" href="http://www.mozilla-japan.org/access/keyboard/tabindex.html">Mozilla や IE における、キーによって移動可能なカスタム HTML ウィジェット</a> (<a class="external" href="http://www.mozilla.org/access/keyboard/tabindex.html">原文</a>)</dt>
          <dd>
            今日まで、キーボードでアクセス可能な <code>&lt;div&gt;</code> や <code>&lt;span&gt;</code> によるスタイル付きのウィジェットを作成しようとするウェブ開発者にとっては、適当な技術はありませんでした。キーボードによるアクセシビリティーはどのウェブ開発者も認識しておかなければならない最低限必要とされるアクセシビリティーの一部です。</dd>
          <dt>
            <a href="ja/docs/Building_XULRunner_with_Python">Building XULRunner with Python</a></dt>
          <dd>
            Windows 上で Python を使用して XULRunner をビルドする方法。この時、comtype が MSAA および IAccessible2 にアクセス権を与えます。</dd>
        </dl>
        <div>
          {{英語版章題("References")}}</div>
        <h3 id=".E3.83.AA.E3.83.95.E3.82.A1.E3.83.AC.E3.83.B3.E3.82.B9" name=".E3.83.AA.E3.83.95.E3.82.A1.E3.83.AC.E3.83.B3.E3.82.B9">リファレンス</h3>
        <dl>
          <dt>
            <a href="ja/docs/Accessibility/AT-APIs">AT APIs Implementation by Gecko</a></dt>
          <dd>
            Gecko による ATK および IAccessible2, MSAA, Universal Access API の扱い。</dd>
          <dt>
            <a href="ja/docs/ARIA/Accessible_Rich_Internet_Applications">ARIA: Accessible Rich Internet Applications</a></dt>
          <dd>
            ARIA は、以前は DHTML アクセシビリティとして知られており、ツリービューやメニューバー、表計算などのデスクトップスタイルのウィジェットを、キーボードおよびスクリーンリーダやスクリーン拡大鏡、その他の代替入力機器などの支援技術から利用可能にします。またページ作者がリアルタイムに更新するウェブページを記述したとき、スクリーンリーダにそれらの変更を知らせることもできます。詳しくは、近くサポートされる <a href="ja/docs/AJAX/WAI_ARIA_Live_Regions">AJAX:WAI ARIA Live Regions</a> のレポートをご覧ください。</dd>
          <dt>
            <a href="ja/docs/Accessibility/XForms">Accessibility XForms References</a></dt>
          <dd>
            XForms コントロールのアクセシブル tree への割り当て。</dd>
        </dl>
        <p><span class="alllinks"><a href="/ja/docs/tag/Accessibility">すべて見る...</a></span></p>
      </td>
      <td>
        <h2 class="Community" id=".E3.82.B3.E3.83.9F.E3.83.A5.E3.83.8B.E3.83.86.E3.82.A3" name=".E3.82.B3.E3.83.9F.E3.83.A5.E3.83.8B.E3.83.86.E3.82.A3">コミュニティ</h2>
        <ul>
          <li>Mozilla フォーラムを見る...</li>
        </ul>
        <p>{{DiscussionList("support-accessibility", "mozilla.support.accessibility")}}</p>
        <ul>
          <li><a class="external" href="http://www.w3.org/WAI/IG/">WAI Interest Group</a></li>
          <li><a href="ja/docs/Accessibility/Community">他のコミュニティへのリンク...</a></li>
        </ul>
        <h2 class="Tools" id=".E3.83.84.E3.83.BC.E3.83.AB" name=".E3.83.84.E3.83.BC.E3.83.AB">ツール</h2>
        <ul>
          <li><a class="external" href="http://www.mozilla-japan.org/quality/embed/plans/accessibility/nsIAccessibleTestPlan.html">Automated Accessibility Tests</a></li>
          <li><a class="external" href="http://www.standards-schmandards.com/index.php?show/fangs">Fangs Screen Reader Emulator</a></li>
        </ul>
        <p><span class="alllinks"><a href="/ja/docs/tag/Accessibility:Tools">すべて見る...</a></span></p>
        <h2 class="Related_Topics" id=".E9.96.A2.E9.80.A3.E4.BA.8B.E9.A0.85" name=".E9.96.A2.E9.80.A3.E4.BA.8B.E9.A0.85">関連事項</h2>
        <p><a href="ja/docs/Web_Development">Web Development</a>, <a href="ja/docs/Web_Standards">Web標準</a>, <a href="ja/docs/XUL">XUL</a></p>
      </td>
    </tr>
  </tbody>
</table>
<div>
  {{endnote(1)}} <a class="external" href="http://en.wikipedia.org/wiki/Accessibility">Wikipedia</a> から (英語版)</div>

