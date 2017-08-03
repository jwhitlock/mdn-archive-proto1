---
version: prototype1
revision_id: 1282969
locale: en-US
slug: user:jwhitlock/TextFormatting
tags: 
title: TextFormatting
summary: 
keywords: 
needs_technical_review: True
needs_editorial_review: True
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>Characters whose Unicode scalar values are greater than U+FFFF (such as some rare Chinese/Japanese/Korean/Vietnamese characters and some emoji) are stored in UTF-16 with two surrogate code units each. For example, a string containing the single character U+1F600 "Emoji grinning face" (&#128512;) will have length 2. Accessing the individual code units in such a string using brackets may have undesirable consequences such as the formation of strings with unmatched surrogate code units, in violation of the Unicode standard. (Examples should be added to this page after MDN bug 857438 is fixed.) See also {{jsxref("String.fromCodePoint()")}} or {{jsxref("String.prototype.codePointAt()")}}.</p>

