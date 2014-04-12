---
version: prototype1
revision_id: 549681
locale: fa
slug: Mozilla/Add-ons
tags: "Add-ons" "TopicStub" "NeedsTranslation"
title: افزونه‌ها
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div class="summary" dir="rtl">
 تغییر و توسعه برنامه‌های موزیلا</div>
<p dir="rtl"><span class="seoSummary">افزونه‌ها قابلیت‌های جدیدی به برنامه‌های مبتنی بر <a href="/en-US/docs/Mozilla/Gecko">Gecko</a> مانند فایرفاکس، سی‌مانکی و تاندربیرد اضافه می‌کنند.</span><strong> </strong>دو نوع اصلی از افزونه‌ها وجود دارد: <a href="#Extensions">الحاقی‌ها</a> که قابلیت‌های جدیدی به برنامه اضافه می‌کنند، <a href="#Themes">تم‌ها</a> که رابط کاربری برنامه را تغییر می‌دهند.</p>
<p dir="rtl">برای هر دو نوع الحاقی‌ها و تم‌ها، موزیلا یک مخزن در <a href="https://addons.mozilla.org/">addons.mozilla.org</a> راه‌اندازی کرده‌است، که به عنوان AMO شناخته می‌شود. وقتی شما <a href="/en-US/Add-ons/Submitting_an_add-on_to_AMO">افزونه‌ها را به AMO ارسال می‌کنید</a> افزونه‌ها بازبینی شده، و افزونه‌ها بعد از گذراندن مرحله بازبینی برای کاربران قابل دسترس خواهند بود. شما مجبور نیستید که افزونه‌ها را به AMO ارسال کنید، اما اگر این‌کار را انجام دهید، کاربران اطمینان پیدا می‌کنند که در عمل افزونه‌ها بازبینی شده‌، و شما به عنوان یک منبع مفید افزونه‌ها از دید AMO سود خواهید برد.</p>
<p dir="rtl">افرونه‌ها تاثیر زیادی بر برنامه‌هایی که آن‌ها را میزبانی می‌کنند می‌گذارند. ما برای اطمینان از فراهم کردن یک تجربه خوب برای کاربران باید <a href="/en-US/docs/Mozilla/Add-ons/Add-on_guidelines">مجموعه‌ای از راهنمایی‌ها</a> را توسعه دهیم. این راهنمایی‌ها بر روی تمام انواع افزونه‌ها اعمال می‌شود، چه آن‌ها در <a href="https://addons.mozilla.org/">addons.mozilla.org</a> میزبانی بشوند یا نشوند.</p>
<hr />
<h2 dir="rtl" id=".D8.A7.D9.84.D8.AD.D8.A7.D9.82.DB.8C.E2.80.8C.D9.87.D8.A7"><a name="Extensions">الحاقی‌ها</a></h2>
<p dir="rtl">الحاقی‌ها قابلیت جدیدی به برنامه‌های موزیلا مانند فایرفاکس و تاندربیرد اضافه می‌کنند. الحاقی‌ها ویژگی‌های جدیدی به مرورگر، مانند روش متفاوتی برای مدیریت تب‌ها اضافه می‌کنند، و آن‌ها می توانند محتوای وب را به‌منظور استفاده از وب‌سایت‌ها یا امنیت وب‌سایت‌های خاص بهبود بخشند.</p>
<p dir="rtl">سه تکنیک مختلف وجود دارد که شما می‌توانید برای ساختن الحاقی‌ها استفاده کنید: الحاقی‌های افزودنی مبتنی بر SDK، الحاقی‌های خود راه‌انداز بدون نیاز به راه‌اندازی مجدد، الحاقی‌های روی هم قرار داده شده.</p>
<ul class="card-grid">
 <li dir="rtl"><span><a href="https://developer.mozilla.org/en-US/Add-ons/SDK">الحاقی‌های افزودنی مبتنی بر SDK</a></span><br />
  توسعه الحاقی‌های بدون نیاز به راه اندازی مجدد از یک‌سری از API های جاوا اسکریپت‌ سطح بالا استفاده می‌کند.</li>
 <li dir="rtl"><span><a href="/en-US/Add-ons/Bootstrapped_extensions">الحاقی‌های بدون نیاز به راه اندازی مجدد</a></span><br />
  توسعه الحاقی‌هایی که نیاز به راه اندازی مجدد مرورگر ندارند.</li>
 <li dir="rtl"><a href="/en-US/Add-ons/Overlay_Extensions"><span>الحاقی‌های روی هم قرار داده شده</span></a><br />
  توسعه الحاقی‌های قدیمی که از XML روی هم قرار گرفته شده استفاده می‌کنند.</li>
</ul>
<p dir="rtl">اگر امکان دارد، توصیه می‌شود تا از افزونه SDK استفاده کنید، که از مکانیزم توسعه بدون نیاز به راه اندازی مجدد استفاده می‌کند ولی وظایف خاص را ساده کرده و بعد از اجرا پاک‌سازی را انجام می‌دهد . اگر افزونه SDK مناسب نیازهای شما نیست، به‌جای آن یک الحاقی بدون نیاز به راه اندازی مجدد را توسعه دهید. درحال حاضر الحاقی‌های روی هم قرار گرفته منسوخ شده‌اند، اگر چه خیلی از آن‌ها که بسیار مورد علاقه هستند هنوز وجود دارند.</p>
<p dir="rtl">برای اطلاعات بیشتر در مورد انتخاب تکنیک مناسب برای استفاده، این <a href="/en-US/Add-ons/Comparing_Extension_Toolchains">مقایسه</a> را بخوانید.</p>
<div class="column-container">
 <div class="column-half">
  <h3 dir="rtl" id=".D8.AA.D9.85.D8.B1.DB.8C.D9.86.E2.80.8C.D9.87.D8.A7.DB.8C_.D9.85.D9.81.DB.8C.D8.AF">تمرین‌های مفید</h3>
  <p dir="rtl">مهم نیست که شما چطور یک الحاق را توسعه می‌دهید، راهنمایی‌های زیادی وجود دارد که می توانید دنبال کنید و مطمئن شوید که الحاقی شما تا آنجایی که امکان دارد تجربه خوبی برای کاربران مهیا کرده‌است یا نه.</p>
  <dl>
   <dt dir="rtl">
    <a href="/en-US/Add-ons/Performance_best_practices_in_extensions">کارائی</a></dt>
   <dd dir="rtl">
    اطمینان از این‌که الحاقی شما سریع، جواب‌گو و از نظرحافظه کارآمد است.</dd>
   <dt dir="rtl">
    <a href="/en-US/Add-ons/Security_best_practices_in_extensions">امنیت</a></dt>
   <dd dir="rtl">
    اطمینان از این‌که الحاقی شما کاربر را در معرض وب سایت‌های بداندیش قرار نمی‌دهد.</dd>
   <dt dir="rtl">
    <a href="/en-US/Add-ons/Extension_etiquette">رسوم</a></dt>
   <dd dir="rtl">
    اطمینان از این‌که الحاقی شما به درستی با دیگر الحاقی‌ها کار می‌کند.</dd>
  </dl>
 </div>
 <div class="column-half">
  <h3 dir="rtl" id=".D8.A8.D8.B1.D9.86.D8.A7.D9.85.D9.87_.D8.AE.D8.A7.D8.B5">برنامه ویژه</h3>
  <p dir="rtl">اغلب مستندات فرض می‌کنند که توسعه شما برای میزکار فایرفاکس است. اگر شما بعضی دیگر برنامه‌های مبتنی بر Gecko را توسعه می‌دهید، تفاوت‌های اصلی وجود دارد که شما باید در مورد آن بدانید.</p>
  <dl>
   <dt dir="rtl">
    <a href="/en-US/Add-ons/Thunderbird">تاندربیرد</a></dt>
   <dd dir="rtl">
    توسعه الحاقی‌ها برای سرویس گیرنده پست الکترونیک تاندربیرد.</dd>
   <dt dir="rtl">
    <a href="/en-US/Add-ons/Firefox_for_Android">فایرفاکس برای اندروید</a></dt>
   <dd dir="rtl">
    توسعه الحاقی‌ها برای فایرفاکس برای اندروید.</dd>
   <dt dir="rtl">
    <a href="/en-US/Add-ons/SeaMonkey_2">سی‌مانکی</a></dt>
   <dd dir="rtl">
    توسعه الحاقی‌ها برای مجموعه برنامه <a href="http://www.seamonkey-project.org/">سی‌مانکی</a>.</dd>
  </dl>
 </div>
</div>
<hr />
<h2 dir="rtl" id=".D8.AA.D9.85.E2.80.8C.D9.87.D8.A7"><a name="Themes">تم‌ها</a></h2>
<p dir="rtl">تم‌ها افزونه‌هایی هستند که رابط کاربری برنامه را سفارشی می‌کنند. دو نوع تم وجود دارد: تم‌های سبک وزن و تم‌های کامل.</p>
<div class="column-container">
 <div class="column-half">
  <p dir="rtl"><a href="https://addons.mozilla.org/en-US/developers/docs/themes">تم‌های سبک وزن</a> از تم‌های کامل برای پیاده سازی ساده‌تر هستند، اما سفارشی سازی محدودی را فراهم می‌کنند.</p>
 </div>
 <div class="column-half" dir="rtl">
  <p>با <a href="/en-US/docs/Themes">تم‌های کامل</a> می توانید تغییرات بیشتری به ظاهر برنامه بدهید. مستندات برای تم‌های کامل به‌روز نیستند، اما به عنوان پایه‌ای برای مستندات به‌روز شده به اینجا لینک شده است.</p>
 </div>
</div>
<hr />
<h2 dir="rtl" id=".D8.A7.D9.86.D9.88.D8.A7.D8.B9_.D8.AF.DB.8C.DA.AF.D8.B1_.D8.A7.D9.81.D8.B2.D9.88.D9.86.D9.87.E2.80.8C.D9.87.D8.A7">انواع دیگر افزونه‌ها</h2>
<p dir="rtl"><a href="/en-US/docs/Creating_OpenSearch_plugins_for_Firefox">متصّل شونده‌های موتور جستجو</a> نوع ساده و خیلی خاص از افزونه هستند: آن‌ها موتور‌های جستجوی جدید را به نوار جستجوی مرورگر اضافه می کنند.</p>
<p dir="rtl"><strong><a href="/en-US/docs/Plugins">متصّل شونده‌ها</a> </strong>به برنامه‌ها در فهمیدن محتوایی که به‌صورت محلی پشتیبانی نمی‌شوند کمک می‌کنند. ما به مرور رمان پشتیبانی از این‌گونه متصّل شونده‌ها را بدخواهیم دانست، آن‌هایی که تاریخچه‌ای در مورد قابلیت پایداری، کارایی، و مشکلات امنیتی دارند.</p>
<hr />
<p style="text-align: right;">{{CommunityBox("extension development", "dev-extensions", "mozilla.dev.extensions", "extdev","Add-ons forums|https://forums.mozilla.org/addons/viewforum.php?f=3|discussion and support|Visit the add-ons forums||AMO|https://addons.mozilla.org/en-US/firefox/|addons.mozilla.org|Visit addons.mozilla.org")}}</p>
<h2 id="Subnav" style="text-align: right;">Subnav</h2>
<ol>
 <li style="text-align: right;"><a href="/en-US/Add-ons/Overlay_Extensions" title="Overlay extensions">Overlay extensions</a></li>
 <li style="text-align: right;"><a href="/en-US/Add-ons/Bootstrapped_extensions" title="Restartless extensions">Restartless extensions</a></li>
 <li style="text-align: right;"><a href="/en-US/Add-ons/SDK">Add-on SDK</a>{{AddonSDKSubnav}}</li>
 <li style="text-align: right;"><a href="#">Extension good practices</a>
  <ol>
   <li><a href="/en-US/Add-ons/Performance_best_practices_in_extensions" title="Performance">Performance</a></li>
   <li><a href="/en-US/Add-ons/Security_best_practices_in_extensions" title="Security">Security</a></li>
   <li><a href="/en-US/Add-ons/Extension_etiquette" title="Etiquette">Etiquette</a></li>
  </ol>
 </li>
 <li style="text-align: right;"><a href="#">Themes</a>
  <ol>
   <li><a href="https://addons.mozilla.org/en-US/developers/docs/themes" title="Lightweight themes">Lightweight themes</a></li>
   <li><a href="/en-US/docs/Themes" title="Complete themes">Complete themes</a></li>
  </ol>
 </li>
 <li style="text-align: right;"><a href="#">Publishing add-ons</a>
  <ol>
   <li><a href="https://addons.mozilla.org/" title="addons.mozilla.org">addons.mozilla.org</a></li>
   <li><a href="/en-US/docs/Mozilla/Add-ons/Add-on_guidelines">Add-on guidelines</a></li>
  </ol>
 </li>
</ol>

