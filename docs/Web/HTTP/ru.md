---
version: prototype1
revision_id: 1148064
locale: ru
slug: Web/HTTP
tags: "HTTP" "Web" "Reference" "l10n:priority"
title: HTTP
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>{{ HTTPSidebar }}</p>

<p class="summary">Протокол передачи гипер текста (&nbsp;<dfn>Hypertext Transfer Protocol -&nbsp;HTTP)</dfn>&nbsp;это <a href="https://ru.wikipedia.org/wiki/%D0%9F%D1%80%D0%BE%D1%82%D0%BE%D0%BA%D0%BE%D0%BB%D1%8B_%D0%BF%D1%80%D0%B8%D0%BA%D0%BB%D0%B0%D0%B4%D0%BD%D0%BE%D0%B3%D0%BE_%D1%83%D1%80%D0%BE%D0%B2%D0%BD%D1%8F">прикладной протокол</a> для передачи гипертекстовых документов, таких как HTML. Он создан для общения между веб-браузерами и веб-серверами, хотя в принципе HTTP может использоваться и для других целей. Протокол следует классической <a href="https://ru.wikipedia.org/wiki/%D0%9A%D0%BB%D0%B8%D0%B5%D0%BD%D1%82-%D1%81%D0%B5%D1%80%D0%B2%D0%B5%D1%80">клиент-серверной модели</a>, когда клиент открывает соединение, инициирует запрос, а затем ждет ответа. HTTP - это&nbsp;<a href="http://en.wikipedia.org/wiki/Stateless_protocol" title="http://en.wikipedia.org/wiki/Stateless_protocol">stateless-протокол</a>, то есть сервер не сохраняет никаких данных (состояние) между парами запросов-ответов. Несмотря на то, что HTTP основан на TCP/IP , он так же может использовать любой <a href="http://en.wikipedia.org/wiki/Transport_Layer">транспорт</a>, который не теряет молча сообщения (то есть обязан знать дошло ли сообщение до адресата).&nbsp;</p>

<div class="column-container">
<div class="column-half">
<h2 class="Documentation" id="Documentation" name="Documentation">Учебники</h2>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Overview">Обзор HTTP</a></dt>
 <dd>Основные свойства клиент-серверного протокола: что можно сделать и для чего он предназначен</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Basics_of_HTTP/Evolution_of_HTTP">Эволюция HTTP</a></dt>
 <dd>Краткое описание изменений, произошедших в HTTP, начиная с самых ранних версий, заканчивая новой HTTP/2 и далее.</dd>
 <dt><a href="https://wiki.mozilla.org/Security/Guidelines/Web_Security">Принципы вэб-безопасности Mozilla</a></dt>
 <dd>Сборник советов для помощи в разработке защищённых вэб-приложений.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Messages">HTTP-сообщения (HTTP Messages)</a></dt>
 <dd>Описывает тип и структуру разных видов сообщений HTTP/1.x и HTTP/2.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Session">Обычный сеанс HTTP</a></dt>
 <dd>Показывает и описывает течение обычногое сеанса HTTP</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Connection_management_in_HTTP_1.x">Управление подключениями в HTTP/1.x</a></dt>
 <dd>Описывает три модели управления подключыениями доступными в HTTP/1.x, их сильные и слабые стороны</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Caching">HTTP-кэширование (HTTP Cache)</a></dt>
 <dd>Кэширование это важнейший инструмент для повышения производительности веб-сайтов. Эта статья представляет разные виды кэша, и как можно использовать HTTP-заголовки для конфигурации и управления кэшированием.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Cookies">HTTP куки (HTTP cookies)</a></dt>
 <dd>Как работают куки можно почитать в <a href="https://tools.ietf.org/html/rfc6265">RFC 6265</a>. В момент получения HTTP-запроса , сервер может послать "Set-Cookie"-заголовок в ответе. После этого, значение куки посылается клиентом с каждым запросом к этому серверу. Делается это в форме <code>Cookie HTTP header</code>. Дополнительно, можно указать истечение срока куки, а так же ограничения для специфического домена или пути.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Access_control_CORS">Контроль доступа (совместное использование ресурсов между разными источниками, HTTP access control (CORS))</a></dt>
 <dd><strong>Межсайтовые HTTP-запросы</strong> (кросс-сайтовые) - это HTTP-запросы к ресурсам, находящимся домене <strong>отличающимся </strong>от того, с которого производится запрос. Например, HTML-страница, загружаемая с домена А (<code>http://domaina.example</code>), запрашивает изображение с домена Б (<code>http://domainb.foo</code>), используя тег&nbsp;<code>img</code> (<code>http://domainb.foo/image.jpg</code>). &nbsp;Это происходит постоянно в мире веба: страницы загружают различные ресурсы в кроссайтовой манере, включая стили (CSS) , изображения, скрипты и другие ресурсы. CORS позволяет разработчикам сайтов контролировать межсайтовые запросы.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Controlling_DNS_prefetching">Контроль предварительной загрузки DNS (Controlling DNS prefetching)</a></dt>
 <dd>Firefox как и большинство других браузеров выполняет <strong>предварительную загрузку DNS (DNS&nbsp;prefetching)</strong>. Это действие, когда брайзеры превентивно выполняют разрешение доменных имён (получают имена доменов) для ссылок, по которым пользователь может перейти, а также для ссылок на ресурсы, такие как картинки, CSS,&nbsp; JavaScript. Эта предварительная загрузка выполняется в фоновом режиме, так что вполне вероятно, что к моменту обращения к объектам в документе, DNS уже получен. Это уменьшает задержки, когда, например, пользователь кликает на ссылку.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="Справочники">Справочники</h2>

<dl>
 <dt><a href="/en-US/docs/HTTP/Headers" title="/en-US/docs/HTTP/Headers">HTTP заголовки (HTTP headers)</a></dt>
 <dd>Заголовки HTTP сообщения используются для точного описания загружаемого ресурса или поведения сервера или клиента. Пользовательские заголовки можно добавить используя&nbsp;'<code>X-</code>' префикс; другие перечислены в &nbsp;<a class="external" href="http://www.iana.org/assignments/message-headers/perm-headers.html" title="http://www.iana.org/assignments/message-headers/perm-headers.html">IANA registry</a>, содержание которого в свою очередь определено в&nbsp;<a class="external" href="http://tools.ietf.org/html/rfc4229" title="http://tools.ietf.org/html/rfc4229">RFC 4229</a>. IANA так же поддерживает&nbsp;<a class="external" href="http://www.iana.org/assignments/message-headers/prov-headers.html" title="http://www.iana.org/assignments/message-headers/prov-headers.html">регистр предложенных новых HTTP заголовков</a>.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Methods">Методы HTTP запроса</a></dt>
 <dd>Различные операции, которые выполняются с HTTP:
 <ul>
  <li>{{HTTPMethod("GET")}}</li>
  <li>{{HTTPMethod("POST")}}</li>
  <li>{{HTTPMethod("OPTIONS")}}</li>
  <li>{{HTTPMethod("DELETE")}}</li>
  <li>{{HTTPMethod("TRACE")}}</li>
  <li>{{HTTPMethod("PATCH")}}</li>
  <li>другие</li>
 </ul>
 <span style="display:none">&nbsp;</span><span style="display:none"> </span></dd>
 <dt><a href="/en-US/docs/Web/HTTP/Status">Коды ответа (HTTP response codes)</a></dt>
 <dd>Коды ответа HTTP указывают на результат выполнения определенного&nbsp;HTTP запроса. Ответы сгруппированы в пять категорий: информационные ответы, удачные ответы, перенаправления, ошибки клиента, и ошибки сервера.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Headers/Content-Security-Policy">Директивы CSP</a></dt>
 <dd>{{HTTPHeader("Content-Security-Policy")}}-поля заголовков ответа позволяют администраторам веб-сайтов констролировать источники ресурсов, которые браузер пользователя может загрузить на данную веб-страницу. За некоторым исключением, эти политики связаны с указанием сервера-источника и адресов доступа (обращения) скриптов.</dd>
</dl>
</div>
</div>

<h2 id="Инструменты_и_ресурсы">Инструменты и ресурсы</h2>

<dl>
 <dt><a href="/ru/docs/Tools">Firefox Developer Tools</a></dt>
 <dd><a href="/ru/docs/Tools/Network_Monitor">Network monitor</a></dd>
 <dt><a href="https://observatory.mozilla.org/">Mozilla Observatory</a></dt>
 <dd>Проект, созданный в помощь разработчикам, системным администраторам и специалистам по безопасности для создания безопасных и надёжных сайтов.</dd>
 <dt><a href="https://redbot.org/">RedBot</a></dt>
 <dd>Инструмент для проверки кэширования заголовков</dd>
 <dt><a href="http://www.html5rocks.com/ru/tutorials/internals/howbrowserswork/">Принципы работы современных веб-браузеров</a></dt>
 <dd>Комплексная статья по внутренностям браузеров и потоку запросов через протокол HTTP. Это нужно понимать всем разработчикам.</dd>
</dl>

<h2 class="Community" id="Community" name="Community">См. также</h2>

<ul>
 <li><a href="/En/Controlling_DNS_prefetching" title="En/Controlling DNS prefetching">Controlling DNS&nbsp;prefetching</a></li>
 <li><a href="/en/HTTP_Pipelining_FAQ" title="https://developer.mozilla.org/en/HTTP_Pipelining_FAQ">HTTP pipelining FAQ</a></li>
 <li><a href="/en/Web_Development/HTTP_cookies" title="HTTP cookies">HTTP cookies</a></li>
 <li><a href="/en-US/docs/HTTP/Headers" title="/en-US/docs/HTTP/Headers">HTTP Headers</a></li>
 <li><a href="/en-US/docs/HTTP/Basic_access_authentication" title="/en-US/docs/HTTP/Basic_access_authentication">Basic access authentication</a></li>
 <li><a href="/en-US/docs/HTTP/Access_control_CORS" title="/en-US/docs/HTTP/Access_control_CORS">HTTP access control (CORS)</a></li>
</ul>

<p>{{ languages( { "ja": "ja/HTTP"} ) }}</p>

