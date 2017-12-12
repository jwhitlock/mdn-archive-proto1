---
version: prototype1
revision_id: 1336207
locale: ka
slug: Mozilla/Add-ons
tags: "გამოქვეყნება" "გაფართოება" "გაფართოებები" "დამატებები" "ენის პაკეტი" "თემები" "ლექსიკონი" "საძიებო სისტემები" "Add-ons" "Landing" "Mozilla" "TopicStub" "Extension" "Extensions" "NeedsTranslation"
title: დამატებები
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<div>&nbsp;</div>

<p><span class="seoSummary">დამატებები, საშუალებას აძლევს შემმუშავებლებს, გააფართოვონ და შეცვალონ Firefox-ის შესაძლებლობები. მათი შექმნა შეიძლება ვებდაპროგრამების ტექნოლოგიებით </span>- JavaScript, HTML და CSS - ასევე, ზოგიერთი JavaScript API-ების დახმარებითაც. დამატებების მეშვეობით შესაძლებელია:</p>

<ul>
 <li>ცალკეული ვებსაიტების იერსახის და შიგთავსის შეცვლა</li>
 <li>Firefox-ის სამომხმარებლო გარემოს გადაკეთება</li>
 <li>Firefox-ისთვის ახალი შესაძლებლობების დამატება</li>
</ul>

<p>რამდენიმე სახის დამატება არსებობს, მაგრამ ყველაზე გავრცელებულია გაფართოებები.</p>

<h2 id="Developing_extensions">გაფართოებების შემუშავება</h2>

<p>Firefox გაფართოებების შესაქმნელად წარსულში, ხელსაწყოთა რამდენიმე ნაკრები არსებობდა, თუმცა 2017 წლის ნოემბრის ბოლოდან, მათი შექმნა, მხოლოდ<a href="https://developer.mozilla.org/en-US/Add-ons/WebExtensions"> WebExtensions API-ების</a> გამოყენებითაა დაშვებული. ხელსაწყოთა სხვა ნაკრებები, როგორიცაა Overlay, Bootstrapped და დამატებების SDK, მოძველებულ ტექნოლოგიებადაა მიჩნეული და ამოღებულია.<br />
 <br />
 თუ, ახალი გაფართოების შექმნა გსურთ, გამოიყენეთ <a href="https://developer.mozilla.org/en-US/Add-ons/WebExtensions">WebExtensions API-ები</a>.</p>

<p>WebExtensions API-ებით შექმნილი Firefox გაფართოებები, ყველა ბრაუზერთანაა თავსებადი. უმეტეს შემთხვევაში, მათი გაშვება თავისუფლად შეიძლება Chrome, Edge-სა და Opera-ში, მცირე ცვლილებების შედეგად. ასევე, სრულად თავსებადია Firefox-ის მრავალპროცესიან ვერსიასთანაც.<br />
 <br />
 <a href="https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">იხილეთ, Firefox-სა და სხვა ბრაუზერებში, ამჟამად მხარდაჭერილი API-ები</a>. ჩვენ ვაგრძელებთ მუშაობას, ახალი API-ების დასამატებლად, შემმუშავებელთა საჭიროებების შესაბამისად.<br />
 <br />
 WebExtensions API-ების უმეტესობა, ასევე ხელმისაწვდომია Firefox Android-ზეც.</p>

<h3 id="Migrate_an_existing_extension">არსებული გაფართოებების გადაკეთება</h3>

<p>თუ, გაქვთ ძველი გაფართოები, რომელიც შექმნილია XUL overlay, bootstrapped, ან დამატებების SDK-ს საშუალებით, მათი გადმოტანაც შეგიძლიათ WebExtension API-ებზე. იხილეთ, <a href="/en-US/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">გადმოტანის შესახებ მასალა MDN-ზე.</a></p>

<p>ვრცლად, მხარდაჭერილი ტექნოლოგიების შესახებ, იხილეთ <a href="/en-US/docs/">wiki გვერდზე.</a></p>

<h2 id="Publishing_add-ons">დამატებების გამოქვეყნება</h2>

<p><a href="https://addons.mozilla.org">Addons.mozilla.org</a>, ცნობილი როგორც "AMO," არის Mozilla-ს ოფიციალური საიტი შემმუშავებლებისთვის, დამატებების განსათავსებლად და მომხმარებლებისთვის, მათ მოსაძიებლად. დამატების AMO საიტზე ატვირთვით, თქვენ შეგიძლიათ გახდეთ ჩვენი შემქმნელებისა და მომხმარებლების დიდი ერთობის წევრი და მარტივად გაუზიაროთ თქვენი ნამუშევარი ხალხს.</p>

<p>თქვენ არ ხართ ვალდებული AMO-ზე განათავსოთ თქვენი დამატება, მაგრამ აუცილებელია, რომ Mozilla-მ დაამოწმოს, წინააღმდეგ შემთხვევაში, მომხმარებლები ვერ შეძლებენ მის დაყენებას.</p>

<p>დამატების გამოქვეყნებისა და მიმოხილვის შესახებ, ვრცლად იხილეთ <a href="https://developer.mozilla.org/en-US/Add-ons/Distribution">დამოწმებისა და გავრცელების საკითხები</a>.</p>

<h2 id="Other_types_of_add-ons">სხვა სახის დამატებები</h2>

<p>გარდა გაფართოებებისა, ასევე არსებობს სხვა დამატებებიც, რომელიც საშუალებას აძლევს მომხმარებლებს, უკეთ მოირგონ Firefox. მათ შორისაა:</p>

<ul>
 <li><a href="https://developer.mozilla.org/Add-ons/Themes/Background">მსუბუქი თემებით</a> შესაძლებელია Firefox იერსახის მცირე ცვლილება.</li>
 <li><a href="/en-US/Add-ons/Firefox_for_Android">მობილურის დამატებები</a> განკუთვნილია Firefox Android ვერსიისთვის. გასათვალისწინებელია, რომ ჩვენ ვგეგმავთ ამ API-ების ტექნოლოგიების ამოღებას. მომავალში, WebExtensions API-ები სრულად იქნება მხარდაჭერილი Firefox Android-ზეც.</li>
 <li><a href="/en-US/docs/Creating_OpenSearch_plugins_for_Firefox">საძიებო სისტემის მოდული</a> ამატებს საძიებო საიტს, ბრაუზერის ძიების ველში.</li>
 <li><a href="/en-US/docs/Mozilla/Creating_a_spell_check_dictionary_add-on">ლექსიკონებით</a> შესაძლებელია მართლწერის შემოწმება, სხვადასხვა ენებზე.</li>
 <li><a href="https://support.mozilla.org/kb/use-firefox-interface-other-languages-language-pack">ენის პაკეტები</a> საშუალებას იძლევა, Firefox-ის იერსახე ხელმისაწვდომი გახდეს სხვადასხვა ენაზე.</li>
</ul>

<hr />
<h2 id="Contact_us">დაგვიკავშირდით</h2>

<p>ქვემოთ მოცემული ბმულები შეგიძლიათ გამოიყენოთ დახმარების მისაღებად, სიახლეების შესატყობად, დამატებების შესახებ და გამოხმაურებისთვის.</p>

<h3 id="Add-ons_forum">დამატებების ფორუმი</h3>

<p>ისარგებლეთ <a href="https://discourse.mozilla.org/c/add-ons">დამატებების ფორუმით</a>, შემუშავების შესახებ, ნებისმიერი საკითხის განსახილველად და დახმარების მისაღებად.</p>

<h3 id="Mailing_lists">ელფოსტების სია</h3>

<p>გამოიყენეთ <strong>dev-addons</strong> მისამართები, დამატებების შესამუშავებელი გარემოს, WebExtension სისტემისა და AMO საიტის შესახებ სასაუბროდ:</p>

<ul>
 <li><a href="https://mail.mozilla.org/listinfo/dev-addons">dev-addons სია</a></li>
 <li><a href="https://mail.mozilla.org/pipermail/dev-addons/">dev-addons არქივი</a></li>
</ul>

<p>გამოიყენეთ <strong>webextensions-support</strong> მისამართები, დამატებების WebExtensions-ზე გადმოტანის და გადაკეთების შესახებ სასაუბროდ:</p>

<ul>
 <li><a href="https://mail.mozilla.org/listinfo/webextensions-support">webextensions-support სია</a></li>
 <li><a href="https://mail.mozilla.org/pipermail/webextensions-support/">webextensions-support არქივი</a></li>
</ul>

<h3 id="IRC">IRC</h3>

<p>თუ IRC-ს გამოყენება უფრო მოგწონთ, შეგიძლიათ იხილოთ:</p>

<ul>
 <li><a href="irc://irc.mozilla.org/addons">#addons</a> (დამატებების შესახებ)</li>
 <li><a href="irc://irc.mozilla.org/extdev">#extdev</a> (დამატებების შემუშავების შესახებ, ზოგადი საუბრებისთვის)</li>
 <li><a href="irc://irc.mozilla.org/webextensions">#webextensions</a> (WebExtensions API-სთან დაკავშირებით, ცალკეული საკითხების განსახილველად )</li>
</ul>

<h3 id="Report_problems">მოხსენება ხარვეზების შესახებ</h3>

<h4 id="Security_vulnerabilities">უსაფრთხოების სისუსტეები</h4>

<p>თუ რომელიმე დამატებაში აღმოაჩენთ უსაფრთხოებისთვის შეუთავსებელ მოწყვლადობას, მიუხედავად იმისა, Mozilla-ს საიტზეა თუ არა განთავსებული, გვაცნობეთ და ჩვენ, შემმუშავებელთან ერთად, აუცილებლად ვიზრუნებთ მის გამოსწორებაზე. გთხოვთ, მოგვახსენოთ <a href="http://www.mozilla.org/projects/security/security-bugs-policy.html">ანონიმურად </a><a href="https://bugzilla.mozilla.org/enter_bug.cgi?product=addons.mozilla.org&amp;component=Add-on%20Security&amp;maketemplate=Add-on%20Security%20Bug&amp;bit-23=1&amp;rep_platform=All&amp;op_sys=All">Bugzilla-ში</a>, ან მოგვწერეთ ელფოსტაზე <a href="mailto:amo-admins@mozilla.org">amo-admins@mozilla.org</a>.</p>

<h4 id="Bugs_on_addons.mozilla.org_(AMO)">ხარვეზები addons.mozilla.org (AMO) საიტზე</h4>

<p>თუ საიტზე რამე შეცდომას იპოვით, სიამოვნებით გამოვასწორებთ. გთხოვთ, <a href="https://github.com/mozilla/addons/issues/new">მოგვახსენოთ</a> და დაურთოთ რაც შეიძლება ვრცელი აღწერა.</p>

