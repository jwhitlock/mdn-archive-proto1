---
version: prototype1
revision_id: 1170085
locale: fa
slug: Mozilla/Add-ons/WebExtensions
tags: "افزونه" "افزونه_فایرفاکس" "برنامه_نویسی" "توسعه"
title: WebExtensions
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: True
needs_localization: True
table_of_contents_depth: 1
based_on: 1143511
---
<div dir="rtl">{{AddonSidebar}}</div>

<div dir="rtl">WebExtensions سیستم توسعه افزونه های مرورگرهای وب سازگار با سایر مرورگرها است. برای توسعه وسعت این سیستم، قابلیت سازگاری با <a class="external-icon external" href="https://developer.chrome.com/extensions">extension API</a> که توسط شرکت گوگل و اوپرا پشتیبانی می شود را دارا می باشد.</div>

<div dir="rtl">افزونه های نوشته شده برای این مرورگرها در بیشتر مواقع در فایرفاکس یا&nbsp;<a href="https://developer.microsoft.com/en-us/microsoft-edge/platform/documentation/extensions/">Microsoft Edge</a> با <a href="https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Porting_from_Google_Chrome">کمی تغییر</a> قابل اجرا هستند. همچنین این API کاملا با&nbsp;<a href="https://developer.mozilla.org/en-US/Firefox/Multiprocess_Firefox">multiprocess Firefox</a> سازگار است.</div>

<p dir="rtl">&nbsp;</p>

<p dir="rtl">ما همچنین قصد داریم این APIها را گسترش دهیم تا نیازهای توسعه دهندگان افزونه ها را مرتفع سازیم. در صورتی که ایده ای دارید ما مشتاقانه منتظر شما هستیم. شما می توانید ما را در<a href="https://mail.mozilla.org/listinfo/dev-addons">dev-addons mailing list</a>&nbsp; یا&nbsp;<a href="irc://irc.mozilla.org/webextensions">#webextensions</a> در&nbsp;<a href="https://wiki.mozilla.org/IRC">IRC</a> دنبال کنید.</p>

<p dir="rtl">&nbsp;</p>

<div class="row topicpage-table" dir="rtl">
<div class="section">
<h3 id="Getting_started">از اینجا شروع کید</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/What_are_WebExtensions">WebExtension چیست ؟</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Your_first_WebExtension">اولین WebExtension شما</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Your_second_WebExtension">دومین WebExtension شما</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Anatomy_of_a_WebExtension">تشریح یک WebExtension</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Examples">نمونه هایی از WebExtensonها</a></li>
</ul>

<h3 id="How_to">چگونه</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Intercept_HTTP_requests">جلوگیری از ترافیک HTTP</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Modify_a_web_page">تغییر محتوای وب</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Add_a_button_to_the_toolbar">اضافه کردن دکمه در منوی ابزار</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Implement_a_settings_page">پیاده سازی صفحه تنظیمات</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Interact_with_the_clipboard">کارکدن با کلیپ بورد</a></li>
 <li>دستکاری کردن برگه های مرورگر</li>
 <li>دسترسی و تغییر لیست علاقه مندی ها</li>
 <li>دسترسی و تغییر کوکی ها</li>
</ul>

<h3 id="Concepts">مفاهیم</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/API">بررسی اجمالی JavaScript API</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/User_interface_components">کامپوننت رابط کاربری</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Content_scripts">Content scripts</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Match_patterns">Match patterns</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Internationalization">بین المللی کردن</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Content_Security_Policy">Content Security Policy</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Native_messaging">Native messaging</a></li>
</ul>

<h3 id="Porting">انتقال</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/Porting_from_Google_Chrome">اتقال افزونه Google Chrome</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">انتقال یک افزونه قدیمی فایرفاکس</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Embedded_WebExtensions">Embedded WebExtensions</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_the_Add-on_SDK">مقایسه به Add-on SDK</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_XUL_XPCOM_extensions">مقایسه با افزونه های XUL/XPCOM</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Chrome_incompatibilities">ناسازگاری ها با Chrome</a></li>
</ul>

<h3 id="Firefox_workflow">نحوه کار فایرفاکس</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/Temporary_Installation_in_Firefox">نصب</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Debugging">اشکال زدایی</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Getting_started_with_web-ext">شروع کار با web-ext</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/web-ext_command_reference">منابع کامند web-ext</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/WebExtensions_and_the_Add-on_ID">WebExtensionها و آی دی Add-on</a></li>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/Publishing_your_WebExtension">انتشار WebExtension شما</a></li>
</ul>
</div>

<div class="section">
<h3 id="Reference">منابع</h3>

<ul>
 <li><a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/API">بررسی اجمالی JavaScript API</a></li>
 <li><a href="/en-US/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">جدول سازگاری مرورگرهای وب برای JavaScript API</a></li>
</ul>

<h4 id="JavaScript_APIs">JavaScript APIs</h4>

<div class="twocolumns">{{ ListSubpages ("/en-US/Add-ons/WebExtensions/API") }}</div>

<h4 id="Manifest_keys">Manifest keys</h4>

<div class="twocolumns">{{ ListSubpages ("/en-US/Add-ons/WebExtensions/manifest.json") }}</div>
</div>
</div>

