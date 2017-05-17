---
version: prototype1
revision_id: 1245231
locale: bn-BD
slug: Mozilla/Add-ons
tags: "Add-ons" "TopicStub" "NeedsTranslation"
title: অ্যাড-অনস
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<div class="summary"><span style="color:#000000">মোজিলা অ্যাপ্লিকেশান গুলোর পরিবর্তন এবং পরিবর্ধন&nbsp;</span></div>

<p>অ্যাড-অন,&nbsp;<a href="https://developer.mozilla.org/en-US/docs/Mozilla/Gecko">গেকো</a> ভিত্তিক অ্যাপ্লিকেশান&nbsp;যেমন: ফায়ারফক্স, সীমাঙ্কী এবং থান্ডারবার্ড এ&nbsp;নতুন কার্যকারিতা যোগ করে। মূলত দুই ধরণের অ্যাড-অন আছে:&nbsp;<a href="https://developer.mozilla.org/en-US/Add-ons#Extensions">এক্সটেনশন</a>, অ্যাপ্লিকেশানে নতুন ধরণের ফিচার যুক্ত করে, আর&nbsp;<a href="https://developer.mozilla.org/en-US/Add-ons#Themes">থিম</a> অ্যাপ্লিকেশানের ইউজার ইন্টারফেস পরিবর্তন করে।&nbsp;</p>

<p>এক্সটেনশন এবং থিম উভয়ের জন্যই মোজিলা&nbsp;<a href="https://addons.mozilla.org/">addons.mozilla.org</a>&nbsp;তে একটি রিপোজিটরি পরিচালনা করে যা এএমও &nbsp;নামে পরিচিত। আপনি যখন <a href="https://developer.mozilla.org/en-US/Add-ons/Submitting_an_add-on_to_AMO">এএমও&nbsp;তে অ্যাড-অন জমা দেন</a>&nbsp;, তখন সেগুলোকে পর্যালোচনা করা হয় তারপর সেগুলো পর্যালোচনাতে উত্তীর্ণ হলে ব্যাবহারকারির কাছে পৌঁছে।<span style="font-family:helvetica">আপনাকে এএমও তে অ্যাড-অন জমা দিতে হবেনা, কিন্তু আপনি যদি দেন, তাহলে ব্যাবহারকারিরা আত্মবিশ্বাসী হতে পারেন যে, সেগুলো রিভিও (পর্যালোচনা) করা হয়েছে । এবং আপনি দরকারি অ্যাড-অন এর উৎস হিসেবে এএমও এর দৃশ্যমানতা এর সুবিধা নিতে পারেন।&nbsp;</span></p>

<p><span style="font-family:helvetica">যেসকল অ্যাপ্লিকেশান অ্যাড-অন কে হোস্ট করে অ্যাড-অন তাদের আচরণকে প্রবলভাবে প্রভাবিত করতে পারে। আমরা এক ঝাঁক দিকনির্দেশনা তৈরি করেছি যাতে ব্যাবরহারকারিদের ভাল অভিজ্ঞতা দিতে পারি । সকল ধরণের অ্যাড-অনের জন্যই এই দিকনির্দেশনা প্রযোজ্য, তা&nbsp;</span><a class="external" href="https://addons.mozilla.org/" style="text-decoration: none; ">addons.mozilla.org</a><span style="font-family:helvetica">&nbsp; তে হোস্ট করা হোক বা অন্য কোথাও হোস্ট করা হোক। </span></p>

<hr />
<h2 id="এক্সটেনশন">এক্সটেনশন&nbsp;</h2>

<p>এক্সটেনশন ফায়ারফক্স এবং থান্ডার-বার্ড এর মত মোজিলা অ্যাপ্লিকেশান গুলোতে নতুন কার্যকারিতা যোগ করে। এরা ব্রাউজারে নতুন ফিচার যুক্ত করতে পারে, যেমন: বিভিন্ন উপায়ে ট্যাবগুলোকে পরিচালনা করা। এবং তারা বিশেষ বিশেষ ওয়েবসাইটের&nbsp;ব্যাবহারযোগ্যতা অথবা নিরাপত্তা বাড়াতে&nbsp;ওয়েব কনটেন্টের পরিবর্তন করতে সক্ষম।&nbsp;</p>

<p>এক্সটেনশন তৈরি করতে আপনি তিনটি ভিন্ন ভিন্ন কৌশল ব্যাবহার করতে পারেন: অ্যাড-অন এসডিকে ভিত্তিক এক্সটেনশন, ম্যানুয়ালী বুটস্ত্র্যাপড রিস্টার্ট বিহীন এক্সটেনশন এবং ওভারলে এক্সটেনশন। &nbsp;</p>

<ul class="card-grid">
 <li><span><a href="https://developer.mozilla.org/en-US/Add-ons/SDK">অ্যাড-অন এসডিকে এক্সটেনশন</a>&nbsp;</span><br />
  এক গুচ্ছ হাই-লেভেল জাভাস্ক্রিপ্ট এপিআই দ্বারা রিস্টার্টবিহীন এক্সটেনশন ডেভেলপ করুন।&nbsp;</li>
 <li><a href="https://developer.mozilla.org/en-US/Add-ons/Bootstrapped_extensions">রিস্টার্টবিহীন এক্সটেনশন&nbsp;</a><br />
  এমন এক্সটেনশন ডেভেলপ করুন যাতে ব্রাউজার রিস্টার্টের প্রয়োজন না হয়। &nbsp;</li>
 <li><a href="https://developer.mozilla.org/en-US/Add-ons/Overlay_Extensions">ওভারলে এক্সটেনশন</a>&nbsp;<br />
  এক্সইউএল ওভার লে দ্বারা গতানুগতিক এক্সটেনশন ডেভেলপ করুন। &nbsp;</li>
</ul>

<p>আপনি যদি পারেন তবে, অ্যাড-অন এসডিকে &nbsp;ব্যাবহার করা সমীচীন হবে, যা রি স্টার্ট বিহীন মেকানিজম ব্যাবহার করে কিন্তু নির্দিষ্ট কিছু কাজকে সহজ করে এবং তারপর নিজেকে পরিষ্কার করে। যদি অ্যাড-অন এসডিকে আপনার প্রয়োজনের তুলনায় পর্যাপ্ত না হয় তবে, এর পরিবর্তে ম্যানুয়াল রি স্টার্ট বিহীন এক্সটেনশন ইমপ্লিমেন্ট করতে পারেন। বর্তমানে অধিকাংশ ক্ষেত্রে ওভারলে এক্সটেনশন অপ্রচলিত , যদিও এখনো এগুলোর প্রাচুর্য রয়েছে।&nbsp;</p>

<p>কোন কৌশল অবলম্বন করবেন এ সম্পর্কে আরও জানতে পড়ুন তাদের <a href="https://developer.mozilla.org/en-US/Add-ons/Comparing_Extension_Toolchains">তুলনা</a>।&nbsp;</p>

<div class="column-container">
<div class="column-half">
<h2 id="ভাল_চর্চা">ভাল চর্চা&nbsp;</h2>

<dl>
 <dd>আপনি যেভাবেই এক্সটেনশন ডেভেলপ করুন না কেন, আপনাকে কিছু দিক নির্দেশ মেনে চলতে হবে, যাতে ব্যাবহারকারিরা একটা ভাল অভিজ্ঞতা পান।&nbsp;</dd>
 <dt><a href="https://developer.mozilla.org/en-US/Add-ons/Performance_best_practices_in_extensions">পারফরমেন্স&nbsp;</a></dt>
 <dd>নিশ্চিত করা যে আপনার এক্সটেনশন দ্রুত, প্রতিক্রিয়াশীল এবং মেমরি এফিসিয়েন্ট।&nbsp;</dd>
 <dt><a href="https://developer.mozilla.org/en-US/Add-ons/Security_best_practices_in_extensions">নিরাপত্তা&nbsp;</a></dt>
 <dd>নিশ্চিত করা যে আপনার এক্সটেনশন ইউজারকে ক্ষতিকারক ওয়েবসাইটে &nbsp;প্রবেশ করাবে না।&nbsp;</dd>
 <dt><a href="https://developer.mozilla.org/en-US/Add-ons/Extension_etiquette">ভদ্রতা&nbsp;</a></dt>
 <dd>নিশ্চিত করা যে আপনার এক্সটেনশন অপর এক্সটেনশনের সাথে ভালো ভাবে কাজ করতে পারে কিনা।&nbsp;</dd>
</dl>
</div>

<div class="column-half">
<h3 id="নির্দিষ্ট-অ্যাপ্লিকেশান">নির্দিষ্ট-অ্যাপ্লিকেশান</h3>

<p>অধিকাংশ ডকুমেন্টেশান ধরে নেয় যে আপনি ফায়ারফক্স ডেক্সটপের জন্য অ্যাড-অন ডেভেলপ করছেন। আপনি যদি গেকো ভিত্তিক অন্য অ্যাপ্লিকেশান এর জন্য ডেভেলপ করতে চান, তাহলে আপনাকে তাদের মধ্যে মুখ্য পার্থক্য গুলো জানতে হবে।&nbsp;</p>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/Add-ons/Thunderbird">থান্ডারবার্ড&nbsp;</a></dt>
 <dd>থান্ডার বার্ড মেইল ক্লায়েন্ট এর জন্য এক্সটেনশন ডেভেলপ করা। &nbsp;</dd>
 <dt><a href="https://developer.mozilla.org/en-US/Add-ons/Firefox_for_Android">ফায়ারফক্স এন্ড্রয়েড</a></dt>
 <dd>ফায়ারফক্স এন্ড্রয়েডের জন্য এক্সটেনশন ডেভেলপ করা।&nbsp;</dd>
 <dt><a href="https://developer.mozilla.org/en-US/Add-ons/SeaMonkey_2">সীমাঙ্কী</a></dt>
 <dd><a href="http://www.seamonkey-project.org/">সীমাঙ্কী</a>&nbsp;সফটওয়্যার সুইটের জন্য এক্সটেনশন ডেভেলপ করা।&nbsp;</dd>
</dl>
</div>
</div>

<hr />
<h2 id="থিম"><a name="Themes">থিম&nbsp;</a></h2>

<p>থিম হল অ্যাড-অন যারা অ্যাপ্লিকেশানের ইউজার ইন্টারফেস পরিবর্তন করে। দুই ধরণের থিম আছে: লাইটওয়েট এবং সম্পূর্ণ থিম।&nbsp;</p>

<div class="column-container">
<div class="column-half">
<p><a href="https://addons.mozilla.org/en-US/developers/docs/themes">লাইটওয়েট থিম</a> গুলো সম্পূর্ণ থিমের চেয়ে সহজে ইমপ্লিমেন্ট করা যায়, কিন্তু খুব সীমিত পরিবর্তন প্রদান করে। &nbsp; &nbsp;</p>
</div>

<div class="column-half">
<p><a href="https://developer.mozilla.org/en-US/docs/Themes">সম্পূর্ণ থিম</a> দ্বারা অ্যাপ্লিকেশান ইউআই তে গভীর পরিবর্তন আনা যায়। সম্পূর্ণ থিমের ডকুমেন্টেশান গুলো অনেক পুরনো, কিন্তু সম্ভাব্য আপডেটের জন্য এখানে লিঙ্ক দেয়া হবে। &nbsp;</p>
</div>
</div>

<hr />
<h2 id="অন্যান্য_ধরণের_অ্যাড-অন">অন্যান্য ধরণের অ্যাড-অন</h2>

<p><a href="https://developer.mozilla.org/en-US/docs/Creating_OpenSearch_plugins_for_Firefox">সার্চইঞ্জিন প্লাগইন</a> হল সরল এবং খুব নির্দিষ্ট ধরণের অ্যাড-অন: তারা ব্রাউজারের সার্চবারে নতুন সার্চইঞ্জিন যুক্ত করে ।&nbsp;</p>

<p>যেসকল কন্টেন্টকে অ্যাপ্লিকেশান স্বাভাবিক ভাবে সাপোর্ট করেনা তাদের বোঝার জন্য <a href="https://developer.mozilla.org/en-US/docs/Plugins">প্লাগইনের</a> সাহায্য দরকার হয়। আমরা এসকল প্লাগ ইনের গভীরতা বাড়াতে কাজ করছি, কেননা এদের স্থায়িত্ব, পারফরমেন্স এবং নিরাপত্তার সমস্যাপূর্ণ ইতিহাস রয়েছে। &nbsp;</p>

<hr />
<p>{{CommunityBox("extension development", "dev-extensions", "mozilla.dev.extensions", "extdev","Add-ons forums|https://forums.mozilla.org/addons/viewforum.php?f=3|discussion and support|Visit the add-ons forums||AMO|https://addons.mozilla.org/en-US/firefox/|addons.mozilla.org|Visit addons.mozilla.org")}}</p>

<h2 id="Subnav">সাবন্যাভ</h2>

<ol>
 <li><a href="/en-US/User:wbamberg/Add-ons/Overlay_Extensions" title="Overlay extensions">Overlay extensions</a></li>
 <li><a href="/en-US/docs/Extensions/Bootstrapped_extensions" title="Restartless extensions">Restartless extensions</a></li>
 <li><a href="https://addons.mozilla.org/en-US/developers/docs/sdk/latest/dev-guide/index.html">Add-on SDK</a>{{AddonSDKSubnav}}</li>
 <li><a href="#">Extension good practices</a>
  <ol>
   <li><a href="/en-US/Add-ons/Performance_best_practices_in_extensions" title="Performance">Performance</a></li>
   <li><a href="/en-US/Add-ons/Security_best_practices_in_extensions" title="Security">Security</a></li>
   <li><a href="/en-US/Add-ons/Extension_etiquette" title="Etiquette">Etiquette</a></li>
  </ol>
 </li>
 <li><a href="#">Themes</a>
  <ol>
   <li><a href="https://addons.mozilla.org/en-US/developers/docs/themes" title="Lightweight themes">Lightweight themes</a></li>
   <li><a href="/en-US/docs/Themes" title="Complete themes">Complete themes</a></li>
  </ol>
 </li>
 <li><a href="#">Publishing add-ons</a>
  <ol>
   <li><a href="https://addons.mozilla.org/" title="addons.mozilla.org">addons.mozilla.org</a></li>
   <li><a href="/en-US/docs/Mozilla/Add-ons/Add-on_guidelines">Add-on guidelines</a></li>
  </ol>
 </li>
</ol>

<div id="__if72ru4sdfsdfrkjahiuyi_once" style="display:none;">&nbsp;</div>

<div id="__hggasdgjhsagd_once" style="display:none;">&nbsp;</div>

