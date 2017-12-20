---
version: prototype1
revision_id: 1338876
locale: ru
slug: Mozilla/Add-ons/WebExtensions
tags: "Landing" "Дополнения" "Расширения" "WebExtensions"
title: Расширения браузера
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<p>WebExtensions - это кросс-браузерная система разработки дополнений (для браузеров). В значительной степени эта система совместима с <a class="external-icon external" href="https://developer.chrome.com/extensions">API-расширений</a>, поддерживаемых Google Chrome и Opera. Расширения, написанные для этих браузеров, в большинстве случаев будут работать с Firefox или <a href="https://developer.microsoft.com/en-us/microsoft-edge/platform/documentation/extensions/">Microsoft Edge</a> <a href="/ru/Add-ons/WebExtensions/Porting_from_Google_Chrome">лишь с минимальными изменениями</a>. Эти API также полностью совместимы с <a href="/ru/Firefox/Multiprocess_Firefox">мультипоточным Firefox</a>.</p>

<p>Также мы намерены расширять API для поддержки нужд разработчиков дополнений, поэтому, если у вас есть идеи, то мы их с удовольствием выслушаем. Вы можете связаться с нами через <a href="https://mail.mozilla.org/listinfo/dev-addons">dev-addons mailing list</a> или <a href="irc://irc.mozilla.org/webextensions">#webextensions</a> на <a href="https://wiki.mozilla.org/IRC">IRC</a>.</p>

<div class="row topicpage-table">
<div class="section">
<h3 id="Приступая_к_работе">Приступая к работе</h3>

<ul>
 <li><a href="/ru/Add-ons/WebExtensions/What_are_WebExtensions">Что такое WebExtensions?</a></li>
 <li><a href="/ru/Add-ons/WebExtensions/Your_first_WebExtension">Первое WebExtension</a></li>
 <li><a href="/ru/Add-ons/WebExtensions/Your_second_WebExtension">Второе WebExtension</a></li>
 <li><a href="/ru/Add-ons/WebExtensions/Anatomy_of_a_WebExtension">Анатомия WebExtension</a></li>
 <li><a href="/ru/Add-ons/WebExtensions/Examples">Примеры WebExtensions</a></li>
</ul>

<h3 id="How_to">How to</h3>

<ul>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/Intercept_HTTP_requests">Перехват HTTP-запросов</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/Modify_a_web_page">Изменить веб-страницу</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/Add_a_button_to_the_toolbar">Добавить кнопку на панель инструментов</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/Implement_a_settings_page">Реализация страницы настроек</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/Interact_with_the_clipboard">Работа с буфером обмена</a></li>
 <li>Работа с вкладками браузера</li>
 <li>Доступ и изменение закладок</li>
 <li>Доступ и изменение куки (cookies)</li>
</ul>

<h3 id="Интерфейс_пользователя">Интерфейс пользователя</h3>

<ul>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/user_interface">Введение</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/user_interface/Browser_action">Кнопка на панели инструментов</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/user_interface/Page_actions">Кнопка в адресной строке</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/user_interface/Popups">Всплывающие окна</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/user_interface/Context_menu_items">Контекстное меню</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/user_interface/Sidebars">Боковые панели </a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/user_interface/Options_page">Страница настройки дополнения</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/user_interface/Bundled_web_pages">Дополнительные web-страницы</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/user_interface/Notifications">Уведомления</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/user_interface/Omnibox">Угадывание адреса по мере ввода</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/user_interface/devtools_panels">Панели инструмента разработчика</a></li>
</ul>

<h3 id="Основные_понятия">Основные понятия</h3>

<ul>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/API">Обзор JavaScript API</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/User_interface_components">Компоненты пользовательского интерфейса</a></li>
 <li><a href="/ru/Add-ons/WebExtensions/Content_scripts">Скрипты Content scripts</a></li>
 <li><a href="/ru/Add-ons/WebExtensions/Match_patterns">Match patterns (шаблоны совпадения)</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/Internationalization">Internationalization</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/Content_Security_Policy">Content Security Policy (политика безопасного контента)</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/Native_messaging">Native messaging (нативный обмен сообщениями)</a></li>
</ul>

<h3 id="Адаптация">Адаптация</h3>

<ul>
 <li><a href="/ru/Add-ons/WebExtensions/Porting_from_Google_Chrome">Портирование расширения из Google Chrome</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">Портирование старых дополнений Firefox</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/Embedded_WebExtensions">Embedded WebExtensions</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_the_Add-on_SDK">Сравнение с Add-on SDK</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/Comparison_with_XUL_XPCOM_extensions">Сравнение с XUL/XPCOM-расширениями</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/Chrome_incompatibilities">Несовместимость с Chrome</a></li>
</ul>

<h3 id="Рабочий_процесс_(workflow)_Firefox">Рабочий процесс (workflow) Firefox</h3>

<ul>
 <li><a href="/en-US/Add-ons/WebExtensions/Temporary_Installation_in_Firefox">Установка</a></li>
 <li><a href="/ru/Add-ons/WebExtensions/Debugging">Отладка</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/Getting_started_with_web-ext">Начало работы с инструментом Web-ext</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/web-ext_command_reference">Справочник команд Web-ext</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/WebExtensions_and_the_Add-on_ID">WebExtensions и Add-on ID</a></li>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/Publishing_your_WebExtension">Публикация вашего дополнения WebExtension</a></li>
</ul>
</div>

<div class="section">
<h3 id="Справочники">Справочники</h3>

<ul>
 <li><a href="/ru/docs/Mozilla/Add-ons/WebExtensions/API">Обзор JavaScript API</a></li>
 <li><a href="/ru/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">Таблицы совместимости браузера для JavaScript APIs</a></li>
</ul>

<h4 id="JavaScript_APIs">JavaScript APIs</h4>

<div class="twocolumns">{{ ListSubpages ("/ru/Add-ons/WebExtensions/API") }}</div>

<h4 id="Manifest_keys">Manifest keys</h4>

<div class="twocolumns">{{ ListSubpages ("/ru/Add-ons/WebExtensions/manifest.json") }}</div>
</div>
</div>

