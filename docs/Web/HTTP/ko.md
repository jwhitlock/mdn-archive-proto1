---
version: prototype1
revision_id: 1318267
locale: ko
slug: Web/HTTP
tags: "HTTP" "Headers" "TopicStub" "NeedsTranslation"
title: HTTP
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{ HTTPSidebar }}</div>

<p class="summary"><strong><dfn>하이퍼텍스트 트랜스퍼 프로토콜(HTTP)는 HTML과 같은, 하이퍼미디어 문서 전송을 위한 </dfn></strong><a class="external" href="http://en.wikipedia.org/wiki/Application_Layer">응용-계층</a><strong><dfn>&nbsp;프로토콜입니다. HTTP는 웹 브라우저와 웹 서버 사이의 통신을 위해 설계되었지만&nbsp;다른 목적을 위해서도 사용될 수 있습니다.</dfn></strong>&nbsp;이 프로토콜은 연결을 열고, 요청을 보낸 뒤&nbsp;응답을 받을 때까지 대기하는 클라이언트를 이용하는 고전적인&nbsp;<a class="external" href="https://en.wikipedia.org/wiki/Client%E2%80%93server_model">클라이언트-서버 모델</a>을 따릅니다. 또한&nbsp;&nbsp;<a class="external" href="http://en.wikipedia.org/wiki/Stateless_protocol">상태없는 프로토콜</a>로, 이는&nbsp;두 개의 요청 사이에 어떤 데이터(상태)도 서버가 유지하지 않는다는 것을 의미합니다. 종종 TCP / IP 계층을 기반으로 하지만,&nbsp;모든 안정적인&nbsp;&nbsp;<a class="external" href="http://en.wikipedia.org/wiki/Transport_Layer">전송 계층</a>에서 사용할 수 있습니다.&nbsp;UDP처럼 메시지를 묵시적으로 손실하지 않는 프로토콜입니다.</p>

<div class="column-container">
<div class="column-half">
<h2 id="튜토리얼">튜토리얼</h2>

<p>HTTP 사용법을 가이드와 튜토리얼로 배워보세요.</p>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Overview">HTTP 개요</a></dt>
 <dd>클라이언트-서버 프로토콜의 기본&nbsp;기능(그것으로 무엇을 할 수 있는지 그리고 의도된 사용법은 무엇인지)을 소개합니다.</dd>
 <dt><a href="/en-US/docs/Mozilla/HTTP_cache">HTTP 캐시</a></dt>
 <dd>캐싱은 웹 사이트의 좋은 성능을&nbsp;위한 중요한 도구입니다. 이 글은 서로 다른 종류의 캐시를 제시하고 그것들을 구성하고 제어하기 위해 HTTP 헤더을 사용하는 방법에 대해 설명합니다.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Cookies">HTTP 쿠키</a></dt>
 <dd>쿠키가 동작하는 방식은&nbsp;<a class="external" href="http://tools.ietf.org/html/rfc6265">RFC 6265</a>에 정의되어 있습니다. HTTP 요청 수신 시, 서버는 응답과 함께&nbsp;<code>Set-Cookie</code>&nbsp;헤더를 전송할 수 있습니다.&nbsp;그 후에, 클라이언트는&nbsp;<code>Cookie</code> HTTP 헤더의 형식 내에서 동일한 서버에 대한 모든 요청을 이용해&nbsp;쿠키 값을 반환하게 됩니다. 추가적으로,&nbsp;&nbsp;파기 지연을 지정할 수 있습니다. 또한 쿠키는 특정 도메인과 경로에 한정될 수도 있습니다.</dd>
 <dt><a href="/en-US/docs/HTTP/Access_control_CORS">HTTP 접근 제어&nbsp;(CORS)</a></dt>
 <dd><strong>크로스-사이트 HTTP 요청</strong>이란 요청을 일으키는 리소스의 도메인이 아닌 <strong>다른 도메인</strong>의 리소스에 대한 HTTP 요청을 말합니다.&nbsp;HTML 웹 페이지와 같이,&nbsp;도메인&nbsp;A (<code>http://domaina.example/</code>)로부터 로드되는 리소스가 이미지처럼&nbsp;<code>img</code> 엘리먼트&nbsp;(<code>http://domainb.foo/image.jpg</code>)를 사용해 도메인&nbsp;B (http://domainb.foo/)에 있는 이미지 리소스에 대해 요청하는 것을 예로 들 수 있습니다. 이런 일은 오늘 날의 웹에서 매우 흔한 일입니다&nbsp;— 페이지들이&nbsp;CSS 스타일, 이미지 그리고 스크립트와 다른 리소스들을 포함하여, 크로스-사이트 측면에서 많은 리소스들을 로드하는 상황&nbsp;말이죠.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Basics_of_HTTP/Evolution_of_HTTP">HTTP의 진화</a></dt>
 <dd>초기 버전부터 현대의 HTTP/2 그리고 그 이후까지&nbsp;HTTP에서 일어났던 변화에 대한 간략한 설명</dd>
 <dt><a href="https://wiki.mozilla.org/Security/Guidelines/Web_Security">Mozilla 웹 보안 가이드라인</a></dt>
 <dd>사이트 운영 조직이 안전한 웹 응용프로그램을 만들도록 돕는 팁 모음입니다.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Messages">HTTP 메시지</a></dt>
 <dd>HTTP/1.x 그리고 HTTP/2 메시지의 서로 다른 종류의 타입과 구조에 대해 설명합니다.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Session">전형적인 HTTP 세션</a></dt>
 <dd>보통의 HTTP 세션의 흐름을 보여주고 설명합니다.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Connection_management_in_HTTP_1.x">HTTP/1.x에서의 연결 관리</a></dt>
 <dd>HTTP/1.x에서 사용 가능한 세 가지 연결 관리 모델,&nbsp;그들의 강점 그리고&nbsp;약점에 대해&nbsp;설명합니다.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="레퍼런스">레퍼런스</h2>

<p>상세한&nbsp;HTTP 레퍼런스 문서를&nbsp;살펴보시기 바랍니다.</p>

<dl>
 <dt><a href="/en-US/docs/Web/HTTP/Headers">HTTP 헤더</a></dt>
 <dd>HTTP 메시지 헤더는 서버 혹은 클라이언트의 리소스 또는&nbsp;동작을 정확하게 설명하는 용도로 사용됩니다. 'X-' 접두사를 사용해 커스텀 헤더를 추가할 수도 있습니다; 원래의&nbsp;내용이&nbsp;<a class="external" href="http://tools.ietf.org/html/rfc4229">RFC 4229</a>에&nbsp;정의되었던&nbsp;<a class="external" href="http://www.iana.org/assignments/message-headers/perm-headers.html">IANA 레지스트리</a>에 그 외의&nbsp;헤더들이 나와&nbsp;있습니다.&nbsp;IANA는 <a class="external" href="http://www.iana.org/assignments/message-headers/prov-headers.html">새롭게 제안된 HTTP 메시지 헤더의 레지스트리</a>도 관리하고 있습니다.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Methods">HTTP 요청 메서드</a></dt>
 <dd>HTTP로 실행될 수 있는 다른 동작({{HTTPMethod("GET")}}, {{HTTPMethod("POST")}})도 있지만,&nbsp;{{HTTPMethod("OPTIONS")}}, {{HTTPMethod("DELETE")}} 혹은&nbsp;{{HTTPMethod("TRACE")}}와 같은 일반적이지는 않은 요청들도 있습니다.</dd>
 <dt><a href="/en-US/docs/Web/HTTP/Response_codes">HTTP 상태 응답 코드</a></dt>
 <dd>HTTP 응답 코드는 특정 HTTP 요청이 성공적으로 완료되었는지를 가리킵니다. 응답은 다섯 가지 계층 내에서 그룹화됩니다: 정보가 있는 응답, 성공적인 응답, 리디렉션, 클라이언트 오류 그리고 서버 오류.</dd>
</dl>

<h2 id="도구와_리소스">도구와&nbsp;리소스</h2>

<p>당신의 HTTP 연결을 사용하고 디버깅하기 위한 유용한 도구들</p>

<dl>
 <dt><a href="/en-US/docs/Tools">파이어폭스 개발자 도구</a></dt>
 <dd><a href="/en-US/docs/Tools/Network_Monitor">네트워크 모니터</a></dd>
 <dt><a href="https://observatory.mozilla.org/">Mozilla Observatory</a></dt>
 <dd>
 <p>개발자, 시스템 관리자와 보안 전문가들이 사이트를 안전하고 견고하게 설정하도록 돕기 위해 설계된 프로젝트입니다.</p>
 </dd>
 <dt><a href="https://redbot.org/">레드봇</a></dt>
 <dd>캐시와 관련된 헤더를 체크하기 위한 도구</dd>
 <dt><a href="http://www.html5rocks.com/ru/tutorials/internals/howbrowserswork/">브라우저 동작 방식</a></dt>
 <dd>HTTP 프로토콜을 통한 브라우저 내부와 요청 흐름에 관한 매우 포괄적인 글입니다.&nbsp;어느 웹 개발자든지 반드시 읽어야 하는 글입니다.</dd>
</dl>
</div>
</div>

