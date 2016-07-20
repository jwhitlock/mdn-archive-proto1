---
version: prototype1
revision_id: 1087029
locale: ko
slug: Web/JavaScript/Reference/Operators
tags: "JavaScript" "Operators"
title: 식 및 연산자
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{jsSidebar("Operators")}}</div>

<p>이 장은 JavaScript 언어의 모든 연산자(operator), 식(expression) 및 키워드를 문서화합니다.</p>

<h2 id="항목별_식_및_연산자">항목별 식 및 연산자</h2>

<p>알파벳순 목록은 왼쪽 사이드바를 보세요.</p>

<h3 id="기본_식">기본 식</h3>

<p>기본 키워드 및 JavaScript의 일반 식.</p>

<dl>
 <dt>{{jsxref("Operators/this", "this")}}</dt>
 <dd><code>this</code> 키워드는 함수의 실행 컨텍스트(문맥)를 말합니다.</dd>
 <dt>{{jsxref("Operators/function", "function")}}</dt>
 <dd><code>function</code> 키워드는 함수 식을 정의합니다.</dd>
 <dt>{{jsxref("Operators/class", "class")}}</dt>
 <dd><code>class</code> 키워드는 클래스 식을 정의합니다.</dd>
 <dt>{{jsxref("Operators/function*", "function*")}}</dt>
 <dd><code>function*</code> 키워드는 생성기(generator) 함수 식을 정의합니다.</dd>
 <dt>{{jsxref("Operators/yield", "yield")}}</dt>
 <dd>생성기 함수를 일시정지(pause) 및 재개(resume)합니다.</dd>
 <dt>{{jsxref("Operators/yield*", "yield*")}}</dt>
 <dd>다른 생성기 함수 또는 반복가능(iterable) 객체로 위임합니다(delegate).</dd>
 <dt>{{jsxref("Global_Objects/Array", "[]")}}</dt>
 <dd>배열 초기자/리터럴 구문.</dd>
 <dt>{{jsxref("Operators/Object_initializer", "{}")}}</dt>
 <dd>객체 초기자/리터럴 구문.</dd>
 <dt>{{jsxref("Global_Objects/RegExp", "/ab+c/i")}}</dt>
 <dd>정규식 리터럴 구문.</dd>
 <dt>{{jsxref("Operators/Grouping", "( )")}}</dt>
 <dd>그룹화 연산자.</dd>
</dl>

<h3 id="좌변_식">좌변 식</h3>

<p>좌변값은 할당(assignment)의 대상입니다.</p>

<dl>
 <dt>{{jsxref("Operators/Property_accessors", "속성 접근자", "", 1)}}</dt>
 <dd>member 연산자는 객체의 속성(property) 또는 메서드에 액세스를 제공합니다<br />
 (<code>object.property</code> 및 <code>object["property"]</code>).</dd>
 <dt>{{jsxref("Operators/new", "new")}}</dt>
 <dd><code>new</code> 연산자는 생성자의 인스턴스를 만듭니다.</dd>
 <dt><a href="/ko/docs/Web/JavaScript/Reference/Operators/new.target">new.target</a></dt>
 <dd>생성자에서, <code>new.target</code>은 {{jsxref("Operators/new", "new")}}에 의해 호출된 생성자를 말합니다.</dd>
 <dt>{{jsxref("Operators/super", "super")}}</dt>
 <dd><code>super</code> 키워드는 부모 생성자를 호출합니다.</dd>
 <dt>{{jsxref("Operators/Spread_operator", "...obj")}}</dt>
 <dd>전개(spread) 연산자는 식이 여러 인수(함수 호출 용) 또는 여러 요소(배열 리터럴 용)가 예상되는 곳에 확장될 수 있도록 합니다.</dd>
</dl>

<h3 id="증가_및_감소">증가 및 감소</h3>

<p>접미(postfix)/접두(prefix) 증가 및 접미/접두 감소 연산자.</p>

<dl>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "A++", "#Increment")}}</dt>
 <dd>접미 증가 연산자.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "A--", "#Decrement")}}</dt>
 <dd>접미 감소 연산자.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "++A", "#Increment")}}</dt>
 <dd>접두 증가 연산자.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "--A", "#Decrement")}}</dt>
 <dd>접두 감소 연산자.</dd>
</dl>

<h3 id="단항_연산자">단항 연산자</h3>

<p>단항(unary) 연산은 피연산자가 하나뿐인 연산입니다.</p>

<dl>
 <dt>{{jsxref("Operators/delete", "delete")}}</dt>
 <dd><code>delete</code> 연산자는 객체에서 속성을 지웁니다.</dd>
 <dt>{{jsxref("Operators/void", "void")}}</dt>
 <dd><code>void</code> 연산자는 식의 반환값을 버립니다.</dd>
 <dt>{{jsxref("Operators/typeof", "typeof")}}</dt>
 <dd><code>typeof</code> 연산자는 주어진 객체의 형을 결정합니다.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "+", "#Unary_plus")}}</dt>
 <dd>단항 더하기 연산자는 그 피연산자를 숫자형으로 변환합니다.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "-", "#Unary_negation")}}</dt>
 <dd>단항 부정(negation) 연산자는 그 피연산자를 숫자형으로 변환한 뒤 부정합니다.</dd>
 <dt>{{jsxref("Operators/Bitwise_Operators", "~", "#Bitwise_NOT")}}</dt>
 <dd>비트 NOT 연산자.</dd>
 <dt>{{jsxref("Operators/Logical_Operators", "!", "#Logical_NOT")}}</dt>
 <dd>논리 NOT 연산자.</dd>
</dl>

<h3 id="산술_연산자">산술 연산자</h3>

<p>산술 연산자는 피연산자로 숫자 값(리터럴 또는 변수 중 하나)을 취하고 숫자 값 하나를 반환합니다.</p>

<dl>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "+", "#Addition")}}</dt>
 <dd>덧셈 연산자.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "-", "#Subtraction")}}</dt>
 <dd>뺄셈 연산자.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "/", "#Division")}}</dt>
 <dd>나눗셈 연산자.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "*", "#Multiplication")}}</dt>
 <dd>곱셈 연산자.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "%", "#Remainder")}}</dt>
 <dd>나머지 연산자.</dd>
</dl>

<dl>
 <dt>{{experimental_inline}} {{jsxref("Operators/Arithmetic_Operators", "**", "#Exponentiation")}}</dt>
 <dd>지수 연산자.</dd>
</dl>

<h3 id="관계_연산자">관계 연산자</h3>

<p>비교(comparison) 연산자는 피연산자를 비교하여 비교가 참인지 여부에 따라 <code>Boolean</code> 값을 반환합니다.</p>

<dl>
 <dt>{{jsxref("Operators/in", "in")}}</dt>
 <dd><code>in</code> 연산자는 객체가 주어진 속성이 있는지를 결정합니다.</dd>
 <dt>{{jsxref("Operators/instanceof", "instanceof")}}</dt>
 <dd><code>instanceof</code> 연산자는 객체가 다른 객체의 인스턴스인지를 결정합니다.</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "&lt;", "#Less_than_operator")}}</dt>
 <dd>작음 연산자.</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "&gt;", "#Greater_than_operator")}}</dt>
 <dd>큼 연산자.</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "&lt;=", "#Less_than_or_equal_operator")}}</dt>
 <dd>작거나 같음 연산자.</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "&gt;=", "#Greater_than_or_equal_operator")}}</dt>
 <dd>크거나 같음 연산자.</dd>
</dl>

<div class="note">
<p><strong>주의:&nbsp;=&gt;</strong> 는 연산자가 아닙니다, 하지만 <a href="/ko/docs/Web/JavaScript/Reference/Functions/애로우_펑션">화살표 함수</a>를 위한 표기법입니다.</p>
</div>

<h3 id="같음_연산자">같음 연산자</h3>

<p>같음(equality) 연산자 평가 결과는 항상 비교가 참인지 여부에 기반을 둔 <code>Boolean</code> 형입니다.</p>

<dl>
 <dt>{{jsxref("Operators/Comparison_Operators", "==", "#Equality")}}</dt>
 <dd>같음 연산자.</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "!=", "#Inequality")}}</dt>
 <dd>같지 않음 연산자.</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "===", "#Identity")}}</dt>
 <dd>항등(identity) 연산자.</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "!==", "#Nonidentity")}}</dt>
 <dd>비항등 연산자.</dd>
</dl>

<h3 id="비트_시프트_연산자">비트 시프트 연산자</h3>

<p>피연산자의 모든 비트를 이동(shift)하는 연산.</p>

<dl>
 <dt>{{jsxref("Operators/Bitwise_Operators", "&lt;&lt;", "#Left_shift")}}</dt>
 <dd>비트 좌로 시프트 연산자.</dd>
 <dt>{{jsxref("Operators/Bitwise_Operators", "&gt;&gt;", "#Right_shift")}}</dt>
 <dd>비트 우로 시프트 연산자.</dd>
 <dt>{{jsxref("Operators/Bitwise_Operators", "&gt;&gt;&gt;", "#Unsigned_right_shift")}}</dt>
 <dd>비트 부호 없는 우로 시프트 연산자.</dd>
</dl>

<h3 id="이진_비트_연산자">이진 비트 연산자</h3>

<p>비트 연산자는 피연산자를 32비트 집합(0과 1)으로 다루고 표준 JavaScript 숫자 값을 반환합니다.</p>

<dl>
 <dt>{{jsxref("Operators/Bitwise_Operators", "&amp;", "#Bitwise_AND")}}</dt>
 <dd>비트 AND.</dd>
 <dt>{{jsxref("Operators/Bitwise_Operators", "|", "#Bitwise_OR")}}</dt>
 <dd>비트 OR.</dd>
 <dt>{{jsxref("Operators/Bitwise_Operators", "^", "#Bitwise_XOR")}}</dt>
 <dd>비트 XOR.</dd>
</dl>

<h3 id="이진_논리_연산자">이진 논리 연산자</h3>

<p>논리 연산자는 보통 사용될 때 boolean(논리) 값으로 사용되고, boolean 값을 반환합니다.</p>

<dl>
 <dt>{{jsxref("Operators/Logical_Operators", "&amp;&amp;", "#Logical_AND")}}</dt>
 <dd>논리 AND.</dd>
 <dt>{{jsxref("Operators/Logical_Operators", "||", "#Logical_OR")}}</dt>
 <dd>논리 OR.</dd>
</dl>

<h3 id="조건_(3항)_연산자">조건 (3항) 연산자</h3>

<dl>
 <dt>{{jsxref("Operators/Conditional_Operator", "(condition ? ifTrue : ifFalse)")}}</dt>
 <dd>
 <p>조건 연산자는 조건의 논리값에 따라 두 값 중 하나를 반환합니다.</p>
 </dd>
</dl>

<h3 id="할당_연산자">할당 연산자</h3>

<p>할당(assignment) 연산자는 값을 그 우변 피연산자의 값에 따라 좌변 피연산자에 할당합니다.</p>

<dl>
 <dt>{{jsxref("Operators/Assignment_Operators", "=", "#Assignment")}}</dt>
 <dd>할당 연산자.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "*=", "#Multiplication_assignment")}}</dt>
 <dd>곱셈 할당.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "/=", "#Division_assignment")}}</dt>
 <dd>나눗셈 할당.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "%=", "#Remainder_assignment")}}</dt>
 <dd>나머지 할당.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "+=", "#Addition_assignment")}}</dt>
 <dd>덧셈 할당.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "-=", "#Subtraction_assignment")}}</dt>
 <dd>뺄셈 할당</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "&lt;&lt;=", "#Left_shift_assignment")}}</dt>
 <dd>좌로 이동 할당.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "&gt;&gt;=", "#Right_shift_assignment")}}</dt>
 <dd>우로 이동 할당.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "&gt;&gt;&gt;=", "#Unsigned_right_shift_assignment")}}</dt>
 <dd>부호 없는 우로 이동 할당.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "&amp;=", "#Bitwise_AND_assignment")}}</dt>
 <dd>비트 AND 할당.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "^=", "#Bitwise_XOR_assignment")}}</dt>
 <dd>비트 XOR 할당.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "|=", "#Bitwise_OR_assignment")}}</dt>
 <dd>비트 OR 할당.</dd>
 <dt>{{jsxref("Operators/Destructuring_assignment", "[a, b] = [1, 2]")}}<br />
 {{jsxref("Operators/Destructuring_assignment", "{a, b} = {a:1, b:2}")}}</dt>
 <dd>
 <p>해체(destructuring) 할당은 배열 또는 객체의 속성을 배열 또는 객체 리터럴과 비슷해 보이는 구문을 사용하여 변수에 할당할 수 있게 합니다.</p>
 </dd>
</dl>

<h3 id="쉼표_연산자">쉼표 연산자</h3>

<dl>
 <dt>{{jsxref("Operators/Comma_Operator", ",")}}</dt>
 <dd>쉼표 연산자는 여러 식을 단문으로 평가되게 하고 마지막 식의 결과를 반환합니다.</dd>
</dl>

<h3 id="비표준_기능">비표준 기능</h3>

<dl>
 <dt>{{non-standard_inline}} {{jsxref("Operators/Legacy_generator_function", "Legacy generator function", "", 1)}}</dt>
 <dd><code>function</code> 키워드는 식 내부 legacy 생성기 함수를 정의하는데 사용될 수 있습니다. 함수를 legacy 생성기로 만들기 위해서는, 함수 몸통(body)은 적어도 하나의 {{jsxref("Operators/yield", "yield")}} 식을 포함해야 합니다.</dd>
 <dt>{{non-standard_inline}} {{jsxref("Operators/Expression_closures", "Expression closures", "", 1)}}</dt>
 <dd>식 클로저(closure)는 간단한 함수 작성을 위한 단축 구문입니다.</dd>
 <dt>{{non-standard_inline}} {{jsxref("Operators/Array_comprehensions", "[for (x of y) x]")}}</dt>
 <dd>배열 내포(comprehension).</dd>
 <dt>{{non-standard_inline}} {{jsxref("Operators/Generator_comprehensions", "(for (x of y) y)")}}</dt>
 <dd>생성기 내포.</dd>
</dl>

<h2 id="스펙">스펙</h2>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="col">스펙</th>
   <th scope="col">상태</th>
   <th scope="col">설명</th>
  </tr>
  <tr>
   <td>{{SpecName('ES1', '#sec-11', 'Expressions')}}</td>
   <td>{{Spec2('ES1')}}</td>
   <td>초기 정의</td>
  </tr>
  <tr>
   <td>{{SpecName('ES5.1', '#sec-11', 'Expressions')}}</td>
   <td>{{Spec2('ES5.1')}}</td>
   <td>&nbsp;</td>
  </tr>
  <tr>
   <td>{{SpecName('ES6', '#sec-ecmascript-language-expressions', 'ECMAScript Language: Expressions')}}</td>
   <td>{{Spec2('ES6')}}</td>
   <td>신규: 전개 연산자, 해체 할당, <code>super</code> 키워드.</td>
  </tr>
  <tr>
   <td>{{SpecName('ESDraft', '#sec-ecmascript-language-expressions', 'ECMAScript Language: Expressions')}}</td>
   <td>{{Spec2('ESDraft')}}</td>
   <td>&nbsp;</td>
  </tr>
 </tbody>
</table>

<h2 id="참조">참조</h2>

<ul>
 <li><a href="/ko/docs/Web/JavaScript/Reference/Operators/연산자_우선순위">연산자 우선순위</a></li>
</ul>

