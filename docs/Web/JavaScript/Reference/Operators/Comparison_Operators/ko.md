---
version: prototype1
revision_id: 1340441
locale: ko
slug: Web/JavaScript/Reference/Operators/Comparison_Operators
tags: 
title: Comparison operators
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: True
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{jsSidebar("Operators")}}</div>

<p>자바스크립트는 strict 비교나, type-converting 비교가 가능하다. strict 비교 (e.g., <code>===</code>) 는 피연산자들이 같은 타입과 값&nbsp;가질때&nbsp;&nbsp;참이다. 더 일반적으로 사용되는 abstract(type-converting)비교 (e.g. <code>==</code>) 는 피연선자를 비교하기 전 먼저 같은 타입으로 바꾼다. 관계 abstract 비교 (e.g., <code>&lt;=</code>), 에서는,비교하기 전에 피연자는 가장 먼저 primitive들로 바꾸고, 같은 타입으로 바꾼다.</p>

<p>문자열은 유니코드 값을 사용해 표준 사서편집 (lexicographical) 상 순서에 따른다.</p>

<p>비교 연산의 특징:</p>

<ul>
 <li>두 문자열의&nbsp;strictly equal은 두 문자열의 문자가 같은 순서를 가지고, 같은 길이를 가지고, 대응하는 위치의 문자가 같을&nbsp;때 를 말한다</li>
 <li>두 숫자의 strictly equal은 두 수가 숫자적으로 같을 때(값이 같을 때)를 말한다.. <a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects/NaN" title="NaN">NaN</a>은 NaN을 포함하여 어떤것과도 같지 않다, 음의 0, 양의 0는 같다.</li>
 <li>두 부울 피연산자의 strictly equal은 둘다 참이거나 둘다 거짓인 경우를 말한다.</li>
 <li>서로 다른 두 객체는 strict비교든 abstract비교든 같지 않다.</li>
 <li>객체를 비교하는 표현은 오직 피연산자가 같은 객체를 참조한 경우만 참이다.</li>
 <li>NULL과 Undefined Type은 자기 자신과 strict equal이고 서로간엔 abstract equal이 적용된다.</li>
</ul>

<h2 id="일치연산자(Equality_operators)">일치연산자(Equality operators)</h2>

<h3 id="동등연산자_()"><a name="Equality">동등연산자 (==)</a></h3>

<p>동등연산자는 만약 피연산자들이 서로 다르면 같은 타입으로 바꾼다, 그다음 strict 비교를 적용한다. 만약 두 피연산자 둘 다 객체라면, 자바스크립트가 메모리의 같은 객체를 참조 할 때 내부 내용을 비교하며, 두 피연자가 메모리의 같은 객체를 가리킨다면 두 객체를 같다고 한다.&nbsp;</p>

<h4 id="Syntax">Syntax</h4>

<pre class="syntaxbox">
x == y
</pre>

<h4 id="Examples">Examples</h4>

<pre class="brush: js">
  1   ==  1        // true
 "1"  ==  1        // true
  1   == '1'       // true
  0   == false     // true
  0   == null      // false

  0   == undefined // false
null  == undefined // true
</pre>

<h3 id="부등_연산자(Inequality_Operator)_(!)"><a name="Inequality">부등 연산자(Inequality Operator)&nbsp;(!=)</a></h3>

<p>부등연산자는 피연산자들이 같지 않는다면 참을 반환한다. 만약 두 피연자가 같은 타입이 아니라면, 자라바스크립트가 두 피연산자를 비교하기에 적당한 타입으로 바꾼다.만약 두 피연자가 객체라면, 자바스크립트가 내부 내용을 비교하며, 메모리의 다른&nbsp;객체를 참조 할 때 다르다고 하며 참을 반환한다..</p>

<h4 id="Syntax_2">Syntax</h4>

<pre class="syntaxbox">
x != y</pre>

<h4 id="Examples_2">Examples</h4>

<pre class="brush: js">
1 !=   2     // true
1 !=  "1"    // false
1 !=  '1'    // false
1 !=  true   // false
0 !=  false  // false
</pre>

<h3 id="일치연산자(Identity_strict_equality)_()"><a name="Identity">일치연산자(Identity / strict equality) (===)</a></h3>

<p>일치연산자는 피연산자들이 타입 변환 없이 strictly equal일 때를 말한다.</p>

<h4 id="Syntax_3">Syntax</h4>

<pre class="syntaxbox">
x === y</pre>

<h4 id="Examples_3">Examples</h4>

<pre class="brush: js ">
3 === 3   // true
3 === '3' // false</pre>

<h3 id="불일치_연산자(Non-identity_strict_inequality)_(!)"><a name="Nonidentity">불일치 연산자(Non-identity / strict inequality) (!==)</a></h3>

<p>불일치연산자는 같은 타입에서 값이 다르거나 다른 타입인 경우 참을 반환한다.</p>

<h4 id="Syntax_4">Syntax</h4>

<pre class="syntaxbox">
x !== y</pre>

<h4 id="Examples_4">Examples</h4>

<pre class="brush: js">
3 !== '3' // true
4 !== 3   // true
</pre>

<h2 id="관계연산자(Relational_operators)">관계연산자(Relational operators)</h2>

<h3 id="크다_연산자(Greater_than_operator_(&gt;))"><a name="Greater_than_operator">크다&nbsp;연산자(Greater than operator (&gt;))</a></h3>

<p>크다 연산자는 만일 왼쪽 피연산자가 오른쪽 피연산자보다 클 경우 참으로 반환한다.</p>

<h4 id="Syntax_5">Syntax</h4>

<pre class="syntaxbox">
x &gt; y</pre>

<h4 id="Examples_5">Examples</h4>

<pre class="brush: js">
4 &gt; 3 // true
</pre>

<h3 id="크거나_동일한_연산자(Greater_than_or_equal_operator_(&gt;))"><a name="Greater_than_or_equal_operator">크거나 동일한 연산자(Greater than or equal operator (&gt;=))</a></h3>

<p>크거나 동일한 연산자는 만일 왼쪽 피연산자가 오른쪽 피연산자보다 크거나 동일할 경우 참으로 반환한다.</p>

<h4 id="Syntax_6">Syntax</h4>

<pre class="syntaxbox">
 x &gt;= y</pre>

<h4 id="Examples_6">Examples</h4>

<pre class="brush: js">
4 &gt;= 3 // true
3 &gt;= 3 // true
</pre>

<h3 id="작다_연산자(Less_than_operator_(&lt;))"><a name="Less_than_operator">작다 연산자(Less than operator (&lt;))</a></h3>

<p>작다 연산자는 왼쪽 피연산자가 오른쪽 피연산자보다 작을 경우에 참을 반환한다.</p>

<h4 id="Syntax_7">Syntax</h4>

<pre class="syntaxbox">
 x &lt; y</pre>

<h4 id="Examples_7">Examples</h4>

<pre class="brush: js">
3 &lt; 4 // true</pre>

<h3 id="작거나_같은_연산자(Less_than_or_equal_operator_(&lt;))"><a id="Less_than_or_equal_operator" name="Less_than_or_equal_operator">작거나 동일한&nbsp;연산자(Less than or equal&nbsp;operator (&lt;=))</a></h3>

<p>작거나 동일한 연산자는 왼쪽 피연산자가 오른쪽 피연산자보다 작거나 동일할 경우에 참을 반환한다.</p>

<h4 id="Syntax_8">Syntax</h4>

<pre class="syntaxbox">
 x &lt;= y</pre>

<h4 id="Examples_8">Examples</h4>

<pre class="brush: js">
3 &lt;= 4 // true
</pre>

<h2 id="일치연산자들_사용(Using_the_Equality_Operators)">일치연산자들 사용(Using the Equality Operators)</h2>

<p>표준적인 일치연산자 (<code>==</code> and <code>!=</code>) 들은&nbsp;두 피연산자들을 비교하기 위해 Abstruct Equlity Comparison Algorithm를 사용한다.&nbsp;만일 피연산자들이 다른 타입이라면, 비교하기 전에 같은 타입과 e.g. 및 비교되기 전에 바꿔진 올바른 string과 5=='5'표현내부안에서 피연산자들을 같은 타입으로 바꿀 것이다.</p>

<p>strict 동등 연산은 (<code>===</code> and <code>!==</code>) &nbsp;<a href="http://www.ecma-international.org/ecma-262/5.1/#sec-11.9.6">Strict Equality Comparison Algorithm</a>을 사용하고 피연산자들이 같은 타입일 때 동등 비교를 하도록 되어있다. 만약 피연산자들이 다른 타입이라면 결과는 항상 거짓이다. 따라서 5 !== '5</p>

<p><br />
 strict 동등 연산은 피연산자가 확실히 특정 값과 타입을 가져야 하거나 피연산자의 정확한 타입이 중요할 때 사용된다. 그렇지 않으면, 피연산자들의 타입이 달라서 사용 할 수 있는 표준 동등 연산자를 사용한다.</p>

<p>타입 변환이 비교하기 위해 먼저 사용 되어야 할 때(non-strict 비교할 때) (i.e., non–strict comparison), 자바스크립트는&nbsp;{{jsxref("String")}}, {{jsxref("Number")}}, {{jsxref("Boolean")}}, or {{jsxref("Object")}} 과 같은 타입의 피연산자를 다음과&nbsp;같이 바꾼다</p>

<ul>
 <li>숫자와 문자열을 비교할 때, 문자열은 숫자값으로 바꿔진다. 자바스크립트는 문자열의 수치적 리터럴을 숫자 타입으로 바꾼다. 첫번째로 수학적 값은 문자열의 수치적 리터럴로부터 유도되어진다. 다음으로, 이 수학적 값은 가장 가까운 숫자 타입 값으로 반올림한다.</li>
 <li>만약 숫자타입 값중 하나가 부울타입이라면, 부울 피연산자는 참일 때 1, 거짓일 때 0이 된다.</li>
 <li>만약 객체가 숫자나 문자열과 비교된다면, 자바스크립트는 객체에 default 값을 반환한다. 연산자는 객체를 객체의 valueOF나 ToString을 이용한 primitive값으로 바꾼다.(문자열이나 숫자로)<br />
  만약 이런 객체의 변환이 실패한다면, 런타임 에러가 생겨난다.</li>
 <li>객체는 그것과 대응할 피연산자가 primitive일때에만 객체가 primitive로의&nbsp;변환하는 것이 끝이라는 것을&nbsp;주의하라.만약 두 피연산자가 객체라면, 그것들은 객체로서 비교되어질 것이다, 그리고 동등연산은 그 피연산자들이 같은 객체를 지명하고 있을 때만 참이 된다.</li>
</ul>

<div class="note"><strong>Note:</strong> String objects는 객체 타입이지 문자열 타입이 아니다!! &nbsp;String objects는 잘 쓰이지 않기때문에 다음&nbsp;결과는 놀랄만할 것이다.&nbsp;</div>

<pre class="brush:js">
// true as both operands are type String (i.e. string primitives):
'foo' === 'foo'

var a = new String('foo');
var b = new String('foo');

// false as a and b are type Object and reference different objects
a == b 

// false as a and b are type Object and reference different objects
a === b 

// true as a and 'foo' are of different type and, the Object (a) 
// is converted to String 'foo' before comparison
a == 'foo'</pre>

<h2 id="Specifications">Specifications</h2>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="col">Specification</th>
   <th scope="col">Status</th>
   <th scope="col">Comment</th>
  </tr>
  <tr>
   <td>{{SpecName('ES1')}}</td>
   <td>{{Spec2('ES1')}}</td>
   <td>Initial definition. Implemented in JavaScript 1.0</td>
  </tr>
  <tr>
   <td>{{SpecName('ES3')}}</td>
   <td>{{Spec2('ES3')}}</td>
   <td>Adds <code>===</code> and <code>!==</code> operators. Implemented in JavaScript 1.3</td>
  </tr>
  <tr>
   <td>{{SpecName('ES5.1', '#sec-11.8')}}</td>
   <td>{{Spec2('ES5.1')}}</td>
   <td>Defined in several sections of the specification: <a href="http://www.ecma-international.org/ecma-262/5.1/#sec-11.8">Relational Operators</a>, <a href="http://www.ecma-international.org/ecma-262/5.1/#sec-11.9">Equality Operators</a></td>
  </tr>
  <tr>
   <td>{{SpecName('ES6', '#sec-relational-operators')}}</td>
   <td>{{Spec2('ES6')}}</td>
   <td>Defined in several sections of the specification: <a href="http://www.ecma-international.org/ecma-262/6.0/#sec-relational-operators">Relational Operators</a>, <a href="http://www.ecma-international.org/ecma-262/6.0/#sec-equality-operators">Equality Operators</a></td>
  </tr>
  <tr>
   <td>{{SpecName('ESDraft', '#sec-relational-operators')}}</td>
   <td>{{Spec2('ESDraft')}}</td>
   <td>Defined in several sections of the specification: <a href="http://tc39.github.io/ecma262/#sec-relational-operators">Relational Operators</a>, <a href="http://tc39.github.io/ecma262/#sec-equality-operators">Equality Operators</a></td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<p>{{CompatibilityTable}}</p>

<div id="compat-desktop">
<table class="compat-table">
 <tbody>
  <tr>
   <th>Feature</th>
   <th>Chrome</th>
   <th>Firefox (Gecko)</th>
   <th>Internet Explorer</th>
   <th>Opera</th>
   <th>Safari</th>
  </tr>
  <tr>
   <td>Basic support</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
  </tr>
 </tbody>
</table>
</div>

<div id="compat-mobile">
<table class="compat-table">
 <tbody>
  <tr>
   <th>Feature</th>
   <th>Android</th>
   <th>Chrome for Android</th>
   <th>Firefox Mobile (Gecko)</th>
   <th>IE Mobile</th>
   <th>Opera Mobile</th>
   <th>Safari Mobile</th>
  </tr>
  <tr>
   <td>Basic support</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
  </tr>
 </tbody>
</table>
</div>

<h2 id="See_also">See also</h2>

<ul>
 <li>{{jsxref("Object.is()")}}</li>
 <li><a href="/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness">Equality comparisons and sameness</a></li>
</ul>

