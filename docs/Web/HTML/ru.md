---
version: prototype1
revision_id: 1329350
locale: ru
slug: Web/HTML
tags: "HTML" "HTML5" "Landing" "Главная" "Reference" "Руководство" "гипертекст"
title: HTML
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{HTMLSidebar()}}</div>

<p><span class="seoSummary">Язык гипертекстовой разметки (HyperText Markup Language — HTML), основной строительный блок веб-страниц, используется для создания и визуального представления веб-страниц. Он определяет содержание страницы, но не её функциональность.</span></p>

<p>HTML добавляет разметку в обычный текст. Гипертекст содержит ссылки, которыми веб-страницы связываются друг с другом, делая Всемирную паутину тем, чем она является сегодня. Создавая и публикуя веб-страницы в сети Интернет, вы становитесь активным участником Всемирной паутины. HTML поддерживает как&nbsp;изображения, так и другой медиаконтент. С помощью HTML каждый может создать статический, а также динимический сайт. HTML является языком, описывающим структуру и семантику содержимого веб-документа. Контент веб-страницы размечен с помощью тегов, представляющих HTML-элементы. Примерами таких элементов являются {{HTMLElement("img")}}, {{HTMLElement("title")}}, {{HTMLElement("p")}}, {{HTMLElement("div")}}, {{HTMLElement("picture")}}&nbsp;и так далее. Эти элементы формируют строительные блоки для любого веб-сайта.</p>

<p>Статьи, представленные здесь, содержат справочные материалы по веб-разработке.</p>

<section class="cleared" id="sect1">
<ul class="card-grid">
 <li><span>Справочник по HTML</span>

  <p>В нашем <a href="/ru/docs/Web/HTML/Ссылки">подробном справочнике</a> вы найдете всю необходимую информацию по каждому из элементов и атрибутов, составляющих HTML.</p>
 </li>
 <li><span>Руководство по HTML</span>
  <p>Для чтения статей, учебников и примеров посвященных HTML обратитесь к нашему <a href="/ru/docs/Web/Guide/HTML">руководству по HTML для разработчиков</a>.</p>
 </li>
 <li><span>Введение в HTML</span>
  <p>Если вы впервые столкнулись с веб-разработкой, то прочтите наш <a href="/ru/docs/Web/Guide/HTML/Introduction">вводный материал</a> о том, что такое HTML и как его использовать.</p>
 </li>
</ul>

<div class="row topicpage-table">
<div class="section">
<h2 class="Documentation" id="Справочники">Справочники</h2>

<dl>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/Block-level_elements">Блочные элементы</a></dt>
 <dd class="landingPageList">Элементы HTML,&nbsp;как правило, блочные&nbsp;и&nbsp;<a href="/ru/docs/Web/HTML/Строчные_Элементы" title="/ru/docs/HTML/inline_elements">строчные</a>. Блочные элементы обычно&nbsp;занимают всю ширину своего родителя, формально&nbsp;создавая "блок" (отсюда и название).</dd>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/CORS_enabled_image">CORS:&nbsp;Включённые изображения</a></dt>
 <dd class="landingPageList">Спецификации HTML вводят атрибут&nbsp;<code><a href="/ru/docs/Web/HTML/Element/img#attr-crossorigin">crossorigin</a></code>, что, вместе с подходящим&nbsp;<a class="glossaryLink" href="/ru/docs/Glossary/CORS" title="CORS небезопасен, когда страница запрашивает какие-нибудь ресурсы с каких-нибудь ресурсов без ограничений. CORS — это система, которая определяет, блокировать или выполнять эти запросы.">CORS</a> заголовком, позоляет определённым через&nbsp;элемент&nbsp;<code><a href="/ru/docs/Web/HTML/Element/img" title="The HTML Image Element (&lt;img&gt;) represents an image of the document.">&lt;img&gt;</a></code>&nbsp;и загруженным с других источников&nbsp;изображениям, быть использованными&nbsp;в canvas так, как будто они загружаются с текущего источника.</dd>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/CORS_settings_attributes">CORS: Настройки атрибутов</a></dt>
 <dd class="landingPageList">В HTML5&nbsp;у некоторых&nbsp;HTML-элементов, которые предоставляют поддержку <a href="/ru/docs/HTTP/Access_control_CORS">CORS</a>&nbsp;(например,&nbsp;<a href="/ru/docs/Web/HTML/Element/img" title="The HTML Image Element (&lt;img&gt;) represents an image of the document."><code>&lt;img&gt;</code></a> и&nbsp;<a href="/ru/docs/Web/HTML/Element/video" title="The HTML &lt;video&gt; element is used to embed video content. It may contain several video sources, represented using the src attribute or the &lt;source&gt; element; the browser will choose the most suitable one."><code>&lt;video&gt;</code></a>), есть атрибут&nbsp;<code>crossorigin</code>, который позволяет конфигурировать CORS-запросы для полученных элементами&nbsp;данных.</dd>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/Controlling_spell_checking_in_HTML_forms">Контролирование правописания в формах HTML</a></dt>
 <dd class="landingPageList">
 <p class="syntaxbox">Firefox 2 вводит поддержку проверки правописания в полях веб-форм. Пользователь может определять, проверять ли текст или нет,&nbsp;через about:config, проверять ли его везде или только в <a href="https://developer.mozilla.org/ru/docs/Web/HTML/Element/textarea">&lt;textarea&gt;</a>.</p>
 </dd>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/DASH_Adaptive_Streaming_for_HTML_5_Video">DASH: Адаптивная трансляция HTML5 видео</a></dt>
 <dd class="landingPageList">Dynamic Adaptive Streaming over HTTP (DASH) — протокол адаптивной трансляции видео. Он позволяет переключаться между битрейтами без остановки воспроизведения.</dd>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/Focus_management_in_HTML">Управление фокусом в HTML</a></dt>
 <dd class="landingPageList">В черновиках HTML5, DOM-атрибут&nbsp;<code><a href="/en/DOM/document.activeElement" title="en/DOM/document.activeElement">activeElement</a></code>&nbsp;и DOM-метод&nbsp;<code><a href="/en/DOM/document.hasFocus" title="en/DOM/document.hasFocus">hasFocus()</a></code>&nbsp;предоставляют возможность иметь более лучший контроль над интерактивными элементами на странице, зависящей&nbsp;от действий пользователя. Например, они могут быть использованы для составляения статистики: подсчёт количества&nbsp;кликов по ссылкам; времени, сколько активен элемент&nbsp;и т. д. Также они помогают минимизировать количество запросов на сервер, когда используются вместе с технологией AJAX, зависящих от действий пользователя и разметки страницы.</dd>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/Общие_атрибуты">Общие атрибуты</a></dt>
 <dd class="landingPageList">Общие атрибуты могут быть определены на всех&nbsp;<a href="/ru/docs/Web/HTML/Element">HTML-элементах</a>, <em>даже если они не описаны в стандартах</em>.&nbsp;Это значит, что на&nbsp;любых нестандартных элементах могут быть использованы общие атрибуты, даже если документ не стандарта&nbsp;HTML5. Например, браузеры с поддержкой&nbsp;HTML5 спрячут контент, помеченный как&nbsp;<code>&lt;foo hidden&gt;...&lt;foo&gt;</code>, хотя&nbsp;<code>&lt;foo&gt;</code>&nbsp;нестандартный элемент HTML.</dd>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/Attributes">Руководство по атрибутам в HTML</a></dt>
 <dd class="landingPageList">У элементов HTML есть <strong>атрибуты&nbsp;—</strong>&nbsp;это дополнительные значения, которые настраивают элементы или регулируют их поведение различным способом, чтобы соответствовать критериям пользователей.</dd>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/Element">Руководство по элементам в HTML</a></dt>
 <dd class="landingPageList">На этой странице находится список всех <a class="glossaryLink" href="/ru/docs/Glossary/HTML" title="HTML (HyperText Markup Language) — это язык разметки, которые определяет структуру страницы.">HTML</a> <a class="glossaryLink" href="/ru/docs/Glossary/Element" title="Элемент — это часть страницы. В XML и HTML элемент может содержать данные или, возможно, ничего. Обычно элемент состоит из открывающегося тега, атрибутов, содержания и закрывающегося тега.">элементов</a>.</dd>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/Ссылки">Руководство по HTML</a></dt>
 <dd class="landingPageList">HTML - это язык, который описывает структуру и смысловое содержание веб-документа; он состоит из <strong>элементов</strong>, каждый из которых может быть изменён с использованием <strong>атрибутов</strong> этих элементов.</dd>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/Inline_elements">Строчные элементы</a></dt>
 <dd class="landingPageList">HTML-элементы обычно строчные или&nbsp;<a href="/ru/docs/Web/HTML/Block-level_elements">блочные</a>. Строчный элемент занимает только выделенное тегами место, которое определяет этот элемент.</dd>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/Типы_ссылок">Типы ссылок</a></dt>
 <dd class="landingPageList">В HTML&nbsp;типы ссылок определяют отношение между двумя страницами, в которых одни ссылки передают информацию&nbsp;другим, используя&nbsp;<a href="/ru/docs/Web/HTML/Element/a" title="The HTML &lt;a&gt; Element (or the HTML Anchor Element) defines a hyperlink, the named target destination for a hyperlink, or both."><code>&lt;a&gt;</code></a>, <a href="/ru/docs/Web/HTML/Element/area" title="The HTML &lt;area&gt; element defines a hot-spot region on an image, and optionally associates it with a hypertext link. This element is used only within a &lt;map&gt; element."><code>&lt;area&gt;</code></a>&nbsp;или&nbsp;<a href="/ru/docs/Web/HTML/Element/link" title="The HTML Link Element (&lt;link&gt;) specifies relationships between the current document and an external resource. Possible uses for this element include defining a relational framework for navigation. This Element is most used to link to style sheets."><code>&lt;link&gt;</code></a>.</dd>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/Поддерживаемые_медиа_форматы">HTML Audio и Video</a></dt>
 <dd class="landingPageList">Элементы&nbsp;<code><a class="new" href="/ru/docs/Web/HTML/Element/audio" title="Документация об этом ещё не написана; пожалуйста, поспособствуйте её написанию!">&lt;audio&gt;</a></code> и <a href="/ru/docs/Web/HTML/Element/video" title="Для встраивания видео контента в документ используйте элемент HTML &lt;video&gt;. Видео элемент может содержать один или несколько источников видео. Чтобы указать источник видео, необходимо использовать атрибут src или элемент &lt;source&gt;; браузер сам определит наиболее подходящий источник."><code>&lt;video&gt;</code></a>&nbsp;предоставляют поддержку проигрывания аудио и видео без использования плагинов.</dd>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/microformats">Микроформаты</a></dt>
 <dd class="landingPageList"><span class="p-summary"><a class="external external-icon" href="http://microformats.org"><dfn>Микроформаты</dfn></a>&nbsp;(иногда сокращено как&nbsp;<strong>μF</strong>) — это маленькие шаблоны HTML для разметки информации о людях, организациях, мероприятиях, записях в блоге, продуктах, отзывах, описаний, рецептов и т. д.</span>&nbsp;Они просты во встраивании семантики в HTML и легки в предоставлении информации поисковыми системами, агрегаторами и т. д.</dd>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/Optimizing_your_pages_for_speculative_parsing">Оптимизация ваших страниц для ускорения парсинга</a></dt>
 <dd class="landingPageList">Традиционно&nbsp;HTML-парсер в браузерах работает на главной ветке&nbsp;и блокируется после тега <code>&lt;/script&gt;</code>, пока скрипт не загрузится и не выполнится. HTML-парсер в Firefox 4 и новее поддерживает рискованный парсинг вне главной ветки. Он продолжает парсить, пока скрипты загружаются и выполняются. В Firefox 3.5 и 3.6 парсер начинает рискованную загрузку&nbsp;скриптов, стилей и изображений, когда он находит их. Однако,&nbsp;в Firefox 4 и новее HTML-парсер также рискованно&nbsp;загружает алгоритм постройки&nbsp;древа&nbsp;HTML. С одной стороны, когда риск оправдался, нет необходимости в репарсинге части, которая уже была просканирована на скрипты, стили и изображения. С другой стороны, когда риск не оправдался, HTML-парсеру достаётся больше работы.</dd>
 <dt class="landingPageList"><a href="/ru/docs/Web/HTML/Using_the_application_cache">Использование&nbsp;кэша приложений</a></dt>
 <dd class="landingPageList"><a href="/ru/docs/HTML/HTML5" title="HTML/HTML5">HTML5</a> предоставляет механизм <em>кэширования приложения</em>, позволяющий веб-приложениям работать в автономном режиме. Разработчики теперь могут использовать интерфейс <strong>Кэша приложения</strong> (<em>AppCache</em>), сообщая браузеру, какие из ресурсов браузеру следует закэшировать и сделать доступными в режиме оффлайн. Закэшированные приложения загружаются и работают корректно, даже если пользователь обновляет страницу в тот момент, когда он отключен от сети.</dd>
</dl>

<p><span class="alllinks"><a href="/ru/docs/tag/HTML" title="Статьи отмеченные: HTML">Посмотреть всё…</a></span></p>
</div>

<div class="section">
<h2 class="Tools" id="Tools" name="Tools">Руководства и учебные материалы</h2>

<dl>
 <dt><a href="/ru/docs/Web/Guide/HTML">Руководство по HTML для разработчиков</a></dt>
 <dd>Статьи MDN демонстрируют определённые методики, которые вы можете использовать при построении веб-контента при помощи HTML. Там же можно найти учебные и другие материалы, которые будут не менее полезны.</dd>
</dl>
</div>
</div>

<p>{{CommunityBox("Веб-разработки", "dev-tech-layout", "mozilla.dev.tech.layout", "", "Stack Overflow|http://ru.stackoverflow.com/questions/tagged/html|Вопросы по&nbsp;HTML|Посетите Stack Overflow, совместно построенный и поддерживаемый&nbsp;Q&amp;A сайт. Посмотрите ответ на Ваш вопрос, и если его нет, то вы можете задать свой вопрос.")}}</p>
</section>

<div id="obhcommdiv" style="display: none;">inactive</div>

<div id="obhcommdiv" style="display: none;">&nbsp;</div>

<div id="obhcommdiv" style="display: none;">&nbsp;</div>

<div id="obhcommdiv" style="display: none;">&nbsp;</div>

