---
version: prototype1
revision_id: 1190337
locale: tr
slug: MDN/Contribute/Localize/Translating_pages
tags: "MDN" "Rehber" "Çeviri" "Sayfa Çevirisi" "Yerelleştirme"
title: MDN Sayfa Çevirileri
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p><span id="result_box" lang="tr"><span class="hps">Bu</span> <span class="hps">makale, çeviri mekaniklerini ve çeşitli türde içerikler ile çalışma konusunda&nbsp;tavsiyeler&nbsp;içeren,&nbsp;MDN'de içerik çevirisi için temel bir kılavuzdur.</span></span></p>

<h2 id="Yeni_bir_sayfa_çevirisine_başlama">Yeni bir sayfa çevirisine başlama</h2>

<p>Karşılaştığınız bir sayfayı, kendi dilinize çevirmek için aşağıdaki adımları izleyiniz:</p>

<ol>
 <li>Diller simgesine () <strong>Diller</strong> menüsünü açmak için tıklayın ve <strong>Çeviri ekle</strong>'yi seçin. Dil Seçimi sayfası gelecektir.</li>
 <li>Buradan sayfayı&nbsp;çevirmek istediğiniz dili seçiniz. Seçim işleminden sonra Makale Çeviri görünümü&nbsp;ekranın sol tarafında çevirisini yapacağınız makale ile beraber orjinal dilinde görünecektir.</li>
 <li><strong>Çeviri Açıklaması&nbsp;</strong>altında, başlığı çevirebilirsiniz,&nbsp;ve&nbsp;tercihen slug'ı da&nbsp;çevirebilirsiniz. Slug, bir sayfa URL'sinin son kısmıdır&nbsp;(örnek olarak, bu makale için "Sayfa_cevirisi".) Bazı dil toplulukları slug kısmını çevirmez, aynı slug'ı İngilizce bırakır. Slug konusunda genel tercihi görebilmek için dilinize çevrilmiş diğer makalelere göz atın. Burayı okuduğunuzda, <strong>Çeviri İçeriği </strong>kısmı için&nbsp;daha fazla yer açmak için&nbsp;<strong>Çeviri Açıklaması&nbsp;</strong>yanındaki eksi işaretine basarak bu kısmı gizleyebilirsiniz.</li>
 <li><strong>Çeviri İçeriği </strong>altında sayfanın gövdesini çevirin.</li>
 <li>Sayfa için en az bir <strong>etiket </strong>ekleyin.</li>
 <li>İşleminiz bittiğinde <strong>Değişiklikleri Kaydet&nbsp;</strong>butonuna tıklayın.</li>
</ol>

<div class="note"><strong>Not: </strong>Makale Çevirisi görünümünün kullanıcı arayüzü elementleri&nbsp;öcelikli olarak İngilizce gösterilir. Belli bir sayfayı çevirmek için yapılan sürekli ziyaretlerde, o dil için MDN yerelleştirmesi mümkünse&nbsp;UI uygun dilde gösterilir. MDN kullanıcı arayüzü&nbsp;<a href="https://localize.mozilla.org/projects/mdn/" title="https://localize.mozilla.org/projects/mdn/">Pontoon</a>&nbsp;kullanılarak yerelleştirilebilir. Bu aracın kullanım detayları için&nbsp;<a href="https://developer.mozilla.org/en-US/docs/Mozilla/Localization/Localizing_with_Pontoon">Pontoon ile Yerelleştirme</a>&nbsp;linkini&nbsp;ziyaret edin.</div>

<h2 id="Çevrilmiş_bir_sayfayı_düzenleme">Çevrilmiş bir sayfayı düzenleme</h2>

<ul>
 <li>Çevrilmiş sayfada, <strong>Düzenle</strong> butonuna basın (bazen hedef dilde etiketlenmiştir). Makale Çevirisi&nbsp;görünümü açılacaktır.</li>
</ul>

<p>Çevirinin son güncellenmesinden bu yana İngilizce versiyon değiştiyse, Makale Çevirisi görünümü İngilizce versiyonda ve kaynak-kod görünümünde&nbsp;değişiklikleri yansııtır. Bu size neyin güncellenmesi gerektiği konusunda yardımcı olur.</p>

<h2 id="Etiket_çevirileri">Etiket çevirileri</h2>

<p><span id="result_box" lang="tr"><span class="hps">Her</span> <span class="hps">sayfanın&nbsp;en</span> <span class="hps">az bir</span> <span class="hps">etiket ile etiketlenmiş</span> <span class="hps">olması</span> <span class="hps">önemlidir, b</span>u "çeviri" olsa bile. Genel olarak, orjinal makalenin kullandığı etiketleri kullanmak daha iyidir.</span></p>

<p>Bazı etiketler arama filtreleri için kullanılır, ya da katkıda bulunanlar arasında topanma yerleri için. Bunlar çevirilmemelidir. Bu etiketleri öğrenmek için, <a href="https://developer.mozilla.org/en-US/docs/Project:MDN/Contributing/Tagging_standards">etiket standartları</a>'nı okuyun. Eğer standart etiketler tarafından alınmadıysa, içerik gruplamak için çevrilmiş etiketler oluşturmada özgürsünüz.</p>

<h2 id="Yeni_yerelleştiricilere_tavsiyeler">Yeni yerelleştiricilere tavsiyeler</h2>

<p>MDN yerelleştirmede yeniysen, aşağıda bulunan önerileri okuyabilirsin:</p>

<ul>
 <li><a href="https://developer.mozilla.org/en-US/docs/Glossary">Glossary</a>'de bulunan makaleler&nbsp;yeni gelen çevirmenler için mükemmeldir, çünkü kısa ve basit olurlar.</li>
 <li><a href="https://developer.mozilla.org/en-US/docs/tag/l10n%3Apriority">"l10n:priority"</a>&nbsp;şeklinde etiketlenmiş makaleler&nbsp;çeviri için öncelikli olarak görülür. Ayrıca,&nbsp;öğretici ve konseptüel makaleler&nbsp;referans sayfalarından daha önceliklidir, çünkü okuyucular yeni konseptler öğrenirken çeviriye daha çok ihtiyaç duyarlar.</li>
 <li>İki eğik parantez arasında metin görürseniz, örnek olarak&nbsp;<code>\{{rastgele-yazı("daha fazla yazı")}}</code>, makale içinde onları çevirmeyin, ve noktalama işaretlerini değiştirmeyin. Bu bir&nbsp;<a href="https://developer.mozilla.org/en-US/docs/MDN/Contribute/Structures/Macros">macro</a>'dur, sayfa içerisinde belli bir yapı oluşturur, ya da başka bir işlevi vardır. Makro tarafından oluşturulmuş rastgele metin görebilirsiniz; MDN'de daha fazla tecrübe edininceye kadar onları önemsemeyin. (Bu yazıyı değiştirmek <a href="https://developer.mozilla.org/en-US/docs/MDN/Contribute/Tools/Template_editing">özel izinler</a>&nbsp;gerektirir,&nbsp;çünkü makro'lar çok güçlü olabilirler.) Eğer merak ediyorsanız, <a href="https://developer.mozilla.org/en-US/docs/MDN/Contribute/Structures/Macros/Commonly-used_macros">Sık kullanılan makrolar</a>&nbsp;linkine bakarak makroların yapabileceği çeşitli şeyleri görebilirsiniz.</li>
 <li>Yereliniz için yerelleştirme&nbsp;hakkında daha fazla bilgi için <a href="https://developer.mozilla.org/en-US/docs/MDN/Contribute/Localize/Localization_projects">Yerelleştirme projeleri sayfası</a>na bakabilirsiniz.</li>
</ul>

