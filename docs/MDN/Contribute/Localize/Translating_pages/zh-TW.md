---
version: prototype1
revision_id: 1282899
locale: zh-TW
slug: MDN/Contribute/Localize/Translating_pages
tags: 
title: 翻譯 MDN 頁面
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>本文為翻譯 MDN 內容提供基本指南，包括翻譯的運作機制及正確處理各種類型內容的訣竅。</p>

<h2 id="開始翻譯新的頁面">開始翻譯新的頁面</h2>

<p>當你來到一個欲翻譯成你的語言的頁面時，請按照下述步驟進行：</p>

<ol>
 <li>點選語言圖示（{{FontAwesomeIcon("icon-language")}}）以開啟<strong>語言</strong>選單，接著點選 <strong>Add a Translation</strong>，選擇語言頁面將會出現。</li>
 <li>點選你想翻譯的語言，開啟翻譯文章介面。原文會顯示於畫面左側。</li>
 <li>在<strong>翻譯描述</strong>裡，你可以翻譯標題並（選擇性的）翻譯「條目連結代碼」（slug）。條目連結代碼就是頁面網址的最末段（例如本文網址中的「Translating_pages」）。在某些語言社群中並不翻譯條目名稱，而會保持與英文一致。比較你語言中的其它文章，以了解習慣作法（編按：正體中文版本不翻譯 slug）。當你完成這部份時，你可以點選<strong>翻譯描述</strong>旁的減號將其隱藏，以讓出更多空間給<strong>內容翻譯</strong>的部份。</li>
 <li>在<strong>翻譯內容</strong>裡翻譯頁面的內容。</li>
 <li>為該頁面填至少一個<strong>標籤</strong>。</li>
 <li>當你完成時點選<strong>儲存修改</strong>。</li>
</ol>

<div class="note"><strong>注意：</strong> 翻譯新文章的使用者介面會以英文顯示。 更新文章時，如果 MDN 的介面有被在地化，則會以適當的語言顯示翻譯介面。 MDN 的使用者介面可以在 <a href="https://pontoon.mozilla.org/projects/mdn/" title="https://pontoon.mozilla.org/projects/mdn/">Pontoon</a> 上進行在地化。請參見<a href="/zh-TW/docs/Mozilla/Localization/Localizing_with_Pontoon" title="/zh-TW/docs/Mozilla/Localization/Localizing_with_Pontoon">使用 Pontoon 來在地化</a>以詳細了解如何使用該工具。</div>

<h2 id="編輯已翻譯的頁面">編輯已翻譯的頁面</h2>

<ul>
 <li>在已翻譯的頁面，點選 <strong>Edit</strong> 按鈕（有時會以目標語系呈現），即會開啟文章翻譯界面。</li>
</ul>

<p>如果英文原文在前次譯文更新之後有所變動，文章翻譯介面會以程式碼的風格，顯示英文版的「前後差異比對」，幫助你找到需要更新的部份。</p>

<h2 id="翻譯標籤">翻譯標籤</h2>

<p>幫每個頁面都標上至少一個標籤非常重要，即使這是譯文。</p>

<p>某些標籤用於搜尋篩選、或是貢獻者之間的約定用法，它們不應該被翻譯。 想要知道有哪些標籤，請閱讀<a href="/en-US/docs/Project:MDN/Contributing/Tagging_standards">標籤準則</a>一文。如果文章還沒有被任何標準的標籤標記，你可以自由的建立翻譯過的標籤以將內容分組。</p>

<h2 id="針對新譯者的指引">針對新譯者的指引</h2>

<p>如果你是 MDN 的新譯者，這裡有些指引：</p>

<ul>
 <li>在 <a href="/zh-TW/docs/Glossary">Glossary</a> 的文章很適合新譯者翻譯，因為它們很簡短。</li>
 <li><a href="/en-US/docs/tag/l10n%3Apriority">被標示為 "l10n:priority" </a> 的文章被認定是高優先翻譯。另外，教學與概念性文章的優先度，通常比參考頁面高，這是因為讀者在理解新觀念的時候，最需要翻譯的東西。</li>
 <li>如果你看到兩個大括號的文字，例如 <code>\{{some-text("more text")}}</code>，讓它在文章內保持原樣、不要改動標點符號。這是 <a href="/zh-TW/docs/MDN/Contribute/Structures/Macros">Macro</a>，它可能用於創建頁面的架構、或其他的用途。你可能看到一些由 macro 產生的原文，在你從 MDN 得到更多經驗以前，不用操心這個（改變那邊的文字需要<a href="/zh-TW/docs/MDN/Contribute/Tools/Template_editing">特殊權限</a>，這是因為 macro 有著十分強大的效果）如果你感到好奇，可以看看 <a href="/zh-TW/docs/MDN/Contribute/Structures/Macros/Commonly-used_macros">Commonly-used macros</a> 來了解各種 macro 如何做動。</li>
 <li>查看 <a href="/zh-TW/docs/MDN/Contribute/Localize/Localization_projects">Localization projects page</a> 以找出更多你語言的在地化。</li>
</ul>

