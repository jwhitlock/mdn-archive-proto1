---
version: prototype1
revision_id: 973849
locale: vi
slug: MDN/Contribute/Localize/dich_trang
tags: "I10n" "MDN Thẻ" "Ngôn ngữ" "Biên dịch" "Hướng dẫn" "Trang dịch"
title: Dịch trang MDN
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<p>Bài viết này là một hướng dẫn cơ bản để biên dịch nội dung trên MDN, điều này bao gồm cả cách dịch và những thủ thuật để xử lý những loại nội dung khác nhau.</p>

<h2 id="Bắt_đầu_một_trang_dịch_mới">Bắt đầu một trang dịch mới</h2>

<p>Khi bạn gặp một trang mà bạn muốn dịch nó sang ngôn ngữ của bạn, hãy làm theo các bước sau:</p>

<ol>
 <li>Click vào biểu tượng <strong>Ngôn ngữ</strong> ({{FontAwesomeIcon("icon-globe")}}) để mở danh mục <strong>Những ngôn ngữ</strong>, rồi click <strong>Thêm một bản dịch</strong>. Trang chọn ngôn ngữ sẽ xuất hiện.</li>
 <li>Click vào ngôn ngữ bạn muốn dịch sang. Giao diện <strong>dịch bài viết</strong> sẽ xuất hiện với ngôn ngữ gốc được hiển thị ở phía bên trái của màn hình hiển thị.</li>
 <li>Phía dưới phần <strong>Mô tả bản dịch</strong>, bạn có thể dịch tiêu đề và slug (tùy chọn) sang ngôn ngữ của bạn. Slug là phần cuối cùng của đường dẫn (URL) của trang (ví dụ, "dich_trang" là Slug của đường dẫn của bài viết này). Một vài ngôn ngữ không dịch phần slug, hãy giữ nó giống với ngôn ngữ tiếng Anh (với tiếng Việt nên để tiếng Việt không dấu và thay dấu cách -space- bằng ký tự "_"). Compare with other articles in your language to determine the common practice. You can click the minus sign next to <strong>Translate Description</strong> to hide this information when you are done with it, to make more room for the <strong>Translate Content</strong> section.</li>
 <li>Under <strong>Translate Content</strong>, translate the body of the page.</li>
 <li>Fill at least one <strong>tag</strong> for the page</li>
 <li>Click <strong>Save Changes</strong> when you are done.</li>
</ol>

<div class="note"><strong>Note:</strong> The user interface elements of the Translating Article view are initially shown in English. On subsequent visits to translate a particular article, the UI is shown in the appropriate language if a localization of MDN is available for that language. The MDN user interface can be localized using <a href="https://localize.mozilla.org/projects/mdn/" title="https://localize.mozilla.org/projects/mdn/">Verbatim</a>. See <a href="/en-US/docs/Mozilla/Localization/Localizing_with_Verbatim" title="/en-US/docs/Mozilla/Localization/Localizing_with_Verbatim">Localizing with Verbatim</a> for details on how to use this tool.</div>

<h2 id="Editing_a_translated_page">Editing a translated page</h2>

<ul>
 <li>On a translated page, click the <strong>Edit</strong> button (sometimes labeled in the target language). The Translating Article view opens.</li>
</ul>

<p>If the English version has been changed since the translation was last updated, the Translating Article view shows a source-level "diff" of the changes in the English version. This helps you see what needs to be updated in the translation.</p>

<h2 id="Translating_tags">Translating tags</h2>

<p>It's important that each page is tagged with at least one tag. Even if this is translation.</p>

<p>Some tags are used for search filters, or as conventions between contributors. They should not be translated. To know these tags, read the <a href="/en-US/docs/Project:MDN/Contributing/Tagging_standards">tagging standards</a>. You are free to create translated tags to group content if this is not covered by one of the standards tags.</p>

