---
version: prototype1
revision_id: 1341633
locale: ko
slug: Web/JavaScript
tags: "Learn" "Landing" "JavaScript" "l10n:priority"
title: JavaScript
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{JsSidebar}}</div>

<p class="summary"><strong>JavaScript</strong> (JS)는 가벼운 인터프리터형 또는 JIT-컴파일형&nbsp;프로그래밍 언어로, <a href="https://en.wikipedia.org/wiki/First-class_functions" title="https://en.wikipedia.org/wiki/First-class_functions">일급 함수</a>를 지원합니다. 주로 웹 페이지를 위한 스크립팅 언어로 알려졌지만, <a class="external" href="https://nodejs.org/">node.js</a>나 <a href="https://couchdb.apache.org/">Apache CouchDB</a>처럼 <a class="external" href="https://en.wikipedia.org/wiki/JavaScript#Uses_outside_web_pages">많은 비브라우저 환경</a>에서도 사용됩니다. JavaScript는 <a class="mw-redirect" href="https://en.wikipedia.org/wiki/Prototype-based_programming" title="Prototype-based">프로토타입 기반</a>의 다중 패러다임 스크립팅 언어로서, 역동적이고, 객체지향형, 명령형 및 선언형(가령 함수형 프로그래밍) 스타일을 지원합니다. 자세한 내용은 <a href="/ko/docs/Web/JavaScript/About">JavaScript에 대하여</a>를 참고하세요.</p>

<p>이 문서는&nbsp;JavaScript 언어 자체만 다루며 웹 페이지를 비롯한 다른 사용 환경에 대해서는 다루지 않습니다. 웹 페이지의 특정 {{Glossary("API","APIs")}}에 대하여 알고 싶다면 <a href="/ko/docs/Web/API">웹 API</a>와 <a href="/ko/docs/DOM">DOM</a>을 참고하시기 바랍니다.</p>

<p>JavaScript의 표준은 <a href="/ko/docs/Web/JavaScript/언어_리소스">ECMAScript</a>입니다. 2012년 현재, <a href="http://kangax.github.io/compat-table/es5/">최신 브라우저</a>는 모두 ECMAScript 5.1을 전부 지원합니다. 예전 브라우저의 경우는 최소한 ECMAScript 3까지는 지원합니다. 2015년 6월 17일 <a href="http://www.ecma-international.org">ECMA International</a>에서는 공식명 ECMAScript 2015 로 불리는&nbsp;ECMAScript의 6번째 주&nbsp;버전을&nbsp;발표했습니다(보통 ECMAScript 6 혹은 ES6으로&nbsp;불립니다). 그 이후 ECMAScript 표준은 출시가 1년 주기입니다. 이 문서는 최신 초안 버전(현재 <a class="external" href="http://tc39.github.io/ecma262/">ECMAScript 2018</a>)을 언급합니다.</p>

<p>JavaScript를 <a href="http://en.wikipedia.org/wiki/Java_(programming_language)">Java 프로그래밍 언어</a>와 혼동해서는 안 됩니다. "Java"와 "JavaScript" 두 가지 모두 Oracle이 미국 및 기타 국가에 등록한 상표입니다. 하지만, 두 언어는 문법 체계와 사용방법이 전혀 다릅니다.</p>

<div class="column-container">
<div class="column-half">
<h2 id="자습서">자습서</h2>

<p>안내서 및 자습서와 JavaScript로 프로그램 짜는 법 알아보기.</p>

<h3 id="입문">입문</h3>

<dl>
 <dt><a href="/ko/docs/Web/JavaScript/Guide" title="JavaScript Guide">JavaScript 안내서</a></dt>
 <dd>JavaScript에 익숙하지 않다면, 이 안내서는 언어를 차례차례 안내합니다.</dd>
 <dt><a href="/ko/docs/Web/JavaScript/JavaScript_technologies_overview" title="JavaScript technologies overview">JavaScript 기술 개요</a></dt>
 <dd>웹 브라우저 JavaScript 상황 소개.</dd>
 <dt><a href="/ko/docs/Web/JavaScript/Introduction_to_Object-Oriented_JavaScript" title="Introduction to Object Oriented JavaScript">객체 지향 JavaScript 입문</a></dt>
 <dd>JavaScript로 객체 지향 프로그래밍 개념 소개.</dd>
</dl>

<h3 id="중급">중급</h3>

<dl>
 <dt><a href="/ko/docs/A_re-introduction_to_JavaScript" title="A re-introduction to JavaScript">JavaScript 재입문</a></dt>
 <dd>JavaScript에 대해 안다고 <em>생각하는</em> 이들을 위한 개요.</dd>
</dl>

<dl>
 <dt><a href="/ko/docs/Web/JavaScript/Data_structures" title="JavaScript data structures">JavaScript 데이터 구조</a></dt>
 <dd>JavaScript에서 이용가능한 데이터 구조 개요.</dd>
 <dt><a href="/ko/docs/Web/JavaScript/Equality_comparisons_and_sameness" title="Equality comparisons and sameness">같음 비교 및 동일성</a></dt>
 <dd>JavaScript는 세 가지 다른 값 비교 연산을 제공합니다: <code>===</code>를 사용한 엄격한(strict) 같음, <code>==</code>를 사용한 느슨한(loose) 같음 및 {{jsxref("Global_Objects/Object/is", "Object.is()")}} 메서드.</dd>
</dl>

<h3 id="고급">고급</h3>

<dl>
 <dt><a href="/ko/docs/Web/JavaScript/Guide/Inheritance_and_the_prototype_chain" title="Inheritance and the prototype chain">상속 및 프로토타입 체인</a></dt>
 <dd>널리 오해 받고 과소 평가된 프로토타입(원형) 기반 상속의 설명.</dd>
 <dt><a href="/ko/docs/Web/JavaScript/Reference/Strict_mode" title="Strict mode">엄격 모드</a></dt>
 <dd>엄격 모드는 초기화 전에 어떤 변수도 사용할 수 없음을 정의합니다. 이는&nbsp;빠른 성능 및 쉬운 디버깅을 위한 ECMAScript 5의 제한된 변형(variant)입니다.</dd>
 <dt><a href="/ko/docs/Web/JavaScript/Typed_arrays" title="JavaScript typed arrays">JavaScript 형식화된 배열</a></dt>
 <dd>JavaScript 형식화된 배열은 원시(raw) 이진 데이터에 접근하기 위한 메커니즘을 제공합니다.</dd>
 <dt><a href="/ko/docs/Web/JavaScript/Memory_Management">메모리 관리</a></dt>
 <dd>JavaScript에서 메모리 라이프 사이클 및 가비지 컬렉션.</dd>
 <dt><a href="/ko/docs/Web/JavaScript/EventLoop" title="Concurrency model and Event Loop">동시성 모델 및 이벤트 루프</a></dt>
 <dd>JavaScript "이벤트 루프"에 기반을 둔 동시성 모델이 있습니다.</dd>
</dl>
</div>

<div class="column-half">
<h2 id="참고서">참고서</h2>

<p>전체 <a href="/ko/docs/Web/JavaScript/Reference" title="JavaScript reference">JavaScript 참고</a> 문서 훑어보기.</p>

<dl>
 <dt><a href="/ko/docs/Web/JavaScript/Reference/Global_Objects" title="Standard objects">표준 객체</a></dt>
 <dd>{{jsxref("Array")}}, {{jsxref("Boolean")}}, {{jsxref("Date")}}, {{jsxref("Error")}}, {{jsxref("Function")}}, {{jsxref("JSON")}}, {{jsxref("Math")}}, {{jsxref("Number")}}, {{jsxref("Object")}}, {{jsxref("RegExp")}}, {{jsxref("String")}}, {{jsxref("Map")}}, {{jsxref("Set")}}, {{jsxref("WeakMap")}} , {{jsxref("WeakSet")}} 등 표준 내장(built-in) 객체 알아가기.</dd>
 <dt><a href="/ko/docs/Web/JavaScript/Reference/Operators" title="Expressions and operators">식 및 연산자</a></dt>
 <dd>JavaScript 연산자 {{jsxref("Operators/instanceof", "instanceof")}}, {{jsxref("Operators/typeof", "typeof")}}, {{jsxref("Operators/new", "new")}}, {{jsxref("Operators/this", "this")}}의 행동, <a href="/ko/docs/Web/JavaScript/Reference/Operators/연산자_우선순위" title="operator precedence">연산자 우선순위</a> 등에 대해 더 알아보기.</dd>
 <dt><a href="/ko/docs/Web/JavaScript/Reference/Statements" title="Statements and declarations">문 및 선언</a></dt>
 <dd>{{jsxref("Statements/do...while", "do-while")}}, {{jsxref("Statements/for...in", "for-in")}}, {{jsxref("Statements/for...of", "for-of")}}, {{jsxref("Statements/try...catch", "try-catch")}}, {{jsxref("Statements/let", "let")}}, {{jsxref("Statements/var", "var")}}, {{jsxref("Statements/const", "const")}}, {{jsxref("Statements/if...else", "if-else")}}, {{jsxref("Statements/switch", "switch")}} 등의 JavaScript 문 및 키워드 작동 법 배우기.</dd>
 <dt><a href="/ko/docs/Web/JavaScript/Reference/Functions" title="Functions">함수</a></dt>
 <dd>어플리케이션 개발에 JavaScript 함수로 작업하는 법 배우기.</dd>
</dl>

<h2 id="도구_자원" title="Tools &amp; resources">도구 &amp; 자원</h2>

<p><strong>JavaScript</strong> 코드 작성 및 디버깅을 돕는 도구.</p>

<dl>
 <dt><a href="/ko/docs/도구들" title="Firefox Developer Tools">Firefox 개발자 도구</a></dt>
 <dd><a href="/ko/docs/도구들/Scratchpad">Scratchpad</a>, <a href="/ko/docs/도구들/Web_Console">Web Console</a>, <a href="/ko/docs/도구들/Performance">JavaScript Profiler</a>, <a href="/ko/docs/도구들/Debugger">Debugger</a> 등.</dd>
 <dt><a class="external" href="http://www.getfirebug.com/">Firebug</a></dt>
 <dd>어느 웹 페이지에서든 CSS, HTML 및 JavaScript 실시간 편집, 디버그 및 관찰.</dd>
 <dt><a href="/ko/docs/Web/JavaScript/Shells">JavaScript 쉘</a></dt>
 <dd>빠르게 JavaScript 코드 조각(snippet)을 테스트할 수 있는 JavaScript 쉘.</dd>
 <dt><a href="https://togetherjs.com/">TogetherJS</a></dt>
 <dd>간편한 협업(Collaboration).</dd>
 <dt><a href="http://stackoverflow.com/questions/tagged/javascript">Stack Overflow</a></dt>
 <dd>"JavaScript" 태그 달린 Stack Overflow 질문.</dd>
 <dt><a href="/ko/docs/Web/JavaScript/New_in_JavaScript" title="JavaScript versions and release notes">JavaScript 버전 및 출시 노트</a></dt>
 <dd>JavaScript 기능 역사 및 구현 상태 훑어보기.</dd>
 <dt><a href="https://jsfiddle.net/">JSFiddle</a></dt>
 <dd>JavaScript, CSS, HTML 편집 및 실시간 결과 얻기. 외부 자원(resource)을 사용하며&nbsp;온라인으로 팀과 협업하기.</dd>
</dl>
</div>
</div>

<p>{{CommunityBox("JavaScript", "js-engine.internals", "mozilla.dev.tech.js-engine.internals", "js", "ES discuss|http://esdiscuss.org/|esdiscuss.org|ECMAScript standard discussion mailing list||SpiderMonkey|https://wiki.mozilla.org/JavaScript|Project page|Contribute to the JavaScript Engine||Twitter|https://twitter.com/FirefoxNightly|@FirefoxNightly|Firefox Nightly updates on Twitter")}}</p>

