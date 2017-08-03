---
version: prototype1
revision_id: 1282431
locale: zh-CN
slug: Web/JavaScript/Reference/Operators/Comparison_Operators
tags: "严格比较操作符" "比较操作符"
title: 比较操作符
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{jsSidebar("Operators")}}</div>

<p>JavaScript 有两种比较方式：严格比较运算符和转换类型比较运算符。对于严格比较运算符（===）来说，仅当两个操作数的类型相同且值相等为 true，而对于被广泛使用的比较运算符（==）来说，会在进行比较之前，将两个操作数转换成相同的类型。对于关系运算符（比如 &lt;=）来说，会先将操作数转为原始值，使它们类型相同，再进行比较运算。</p>

<p>字符串比较则是使用基于标准字典的 Unicode 值来进行比较的。</p>

<p>比较的特点:</p>

<ul>
 <li>对于两个拥有相同字符顺序，相同长度，并且每个字符的位置都匹配的字符串，应该使用严格比较运算符。</li>
 <li><span style="line-height:1.5">&nbsp;对于两个数值相同的数字应该使用严格比较运算符，NaN和任何值不相等，包括其自身，正数零等于负数零。</span></li>
 <li>对于两个同为true或同为false的布尔操作数，应使用严格比较运算符。</li>
 <li>不要使用严格比较运算符或比较运算符来比较两个不相等的对象。</li>
 <li>当比较一个表达式和一个对象时，仅当两个操作数引用相同的对象（指针指向相同对象）。</li>
 <li>对于Null 和&nbsp;Undefined 类型而言，应使用严格比较运算符比较其自身，使用比较运算符进行互相比较。</li>
</ul>

<h2 id="相等运算符">相等运算符</h2>

<h3 id="相等()">相等(==)</h3>

<p>比较操作符会为两个不同类型的操作数转换类型，然后进行严格比较。当两个操作数都是对象时，JavaScript会比较其内部引用，当且仅当他们的引用指向内存中的相同对象（区域）时才相等，即他们在栈内存中的引用地址相同。</p>

<h4 id="语法">语法</h4>

<pre class="syntaxbox">
x == y
</pre>

<h4 id="例子">例子</h4>

<pre class="brush: js">
 1   ==  1     // true
"1"  ==  1     // true
 1   == '1'    // true
 0   == false  // true
</pre>

<h3 id="不相等_(!)"><a name="Inequality">不相等 (!=)</a></h3>

<p>不等操作符仅当操作数不相等时返回true，如果两操作数不是同一类型，JavaScript会尝试将其转为一个合适的类型，然后进行比较。如果两操作数为对象类型，JavaScript会比较其内部引用地址，仅当他们在内存中引用不同对象时不相等。</p>

<h4 id="语法_2">语法</h4>

<pre class="syntaxbox">
x != y</pre>

<h4 id="例子_2">例子</h4>

<pre class="brush: js">
1 !=   2     // true
1 !=  "1"    // false
1 !=  '1'    // false
1 !=  true   // false
0 !=  false  // false
</pre>

<h3 id="一致严格相等_()"><a name="Identity">一致/严格相等&nbsp;(===)</a></h3>

<p>一致运算符不会进行类型转换，仅当操作数严格相等时返回true</p>

<h4 id="语法_3">语法</h4>

<pre class="syntaxbox">
x === y</pre>

<h4 id="例子_3">例子</h4>

<pre class="brush: js ">
3 === 3   // true
3 === '3' // false
var object1 = {"value":"key"}, object2={"value":"key"};
object1 === object2 //false</pre>

<h3 id="不一致严格不相等_(!)"><a name="Nonidentity">不一致/严格不相等 (!==)</a></h3>

<p>不一致运算符当操作数不相等或不同类型时返回true</p>

<h4 id="语法_4">语法</h4>

<pre class="syntaxbox">
x !== y</pre>

<h4 id="例子_4">例子</h4>

<pre class="brush: js">
3 !== '3' // true
4 !== 3   // true
</pre>

<h2 id="关系运算符">关系运算符</h2>

<h3 id="大于运算符_(&gt;)"><a name="Greater_than_operator">大于运算符&nbsp;(&gt;)</a></h3>

<p>大于运算符仅当左操作数大于右操作数时返回true</p>

<h4 id="语法_5">语法</h4>

<pre class="syntaxbox">
x &gt; y</pre>

<h4 id="例子_5">例子</h4>

<pre class="brush: js">
4 &gt; 3 // true
</pre>

<h3 id="大于等于运算符_(&gt;)"><a name="Greater_than_or_equal_operator">大于等于运算符 (&gt;=)</a></h3>

<p>大于等于运算符当左操作数大于或等于右操作数时返回true</p>

<h4 id="语法_6">语法</h4>

<pre class="syntaxbox">
 x &gt;= y</pre>

<h4 id="例子_6">例子</h4>

<pre class="brush: js">
4 &gt;= 3 // true
3 &gt;= 3 // true
</pre>

<h3 id="小于运算符_(&lt;)"><a name="Less_than_operator">小于运算符 (&lt;)</a></h3>

<p>小于运算符仅当左操作数小于右操作数时返回true</p>

<h4 id="语法_7">语法</h4>

<pre class="syntaxbox">
 x &lt; y</pre>

<h4 id="例子_7">例子</h4>

<pre class="brush: js">
3 &lt; 4 // true
</pre>

<h3 id="小于等于运算符_(&lt;)"><a id="Less_than_or_equal_operator" name="Less_than_or_equal_operator">小于等于运算符 (&lt;=)</a></h3>

<p>小于等于运算符当左操作数小于或等于右操作数时返回true</p>

<h4 id="语法_8">语法</h4>

<pre class="syntaxbox">
 x &lt;= y</pre>

<h4 id="例子_8">例子</h4>

<pre class="brush: js">
3 &lt;= 4 // true
</pre>

<h2 id="使用比较操作符">使用比较操作符</h2>

<p>标准相等操作符(<code>==</code> and <code>!=</code>) 使用&nbsp;<a href="http://www.ecma-international.org/ecma-262/5.1/#sec-11.9.3">Abstract Equality Comparison Algorithm</a> 去比较两个操作数。当两个操作数类型不相等时，会在比较前尝试将其转换为相同类型。&nbsp;e.g., 对于表达式&nbsp;<code>5 == '5'</code>, 在比较前会先将右边字符串类型的操作数 5 转换为数字。</p>

<p>严格相等操作符 (<code>===</code> and <code>!==</code>) 使用 Strict Equality Comparison Algorithm 并尝试对两个相同操作数进行相等比较，如果它们的类型不相等，那么永远会返回false 所以&nbsp;<code>5 !== '5'。</code></p>

<p>当需要明确操作数的类型和值的时候，或者操作数的确切类型非常重要时，应使用严格相等操作符。否则，当你允许操作数在比较前进行类型转换时，可以使用标准相等操作符来比较。</p>

<p>当比较运算涉及类型转换时&nbsp;(i.e., non–strict comparison), JavaScript 会按以下规则对字符串，数字，布尔或对象类型的操作数进行操作:</p>

<ul>
 <li>当比较数字和字符串时，字符串会转换成数字值。&nbsp;JavaScript 尝试将数字字面量转换为数字类型的值。&nbsp;首先, 一个数学上的值会从数字字面量中衍生出来，然后得到被四舍五入后的数字类型的值。</li>
 <li>如果其中一个操作数为布尔类型，那么布尔操作数如果为true，那么会转换为1，如果为false，会转换为整数0，即0。</li>
 <li>如果是一个对象与数字或字符串向比较，JavaScript会尝试返回对象的默认值。操作符会尝试将对象转换为其原始值（一个字符串或数字值）通过方法valueOf和toString。如果尝试转换失败，会产生一个运行时错误。</li>
 <li>注意：当且仅当与原始值比较时，对象会被转换为原始值。当两个操作数均为对象时，它们作为对象进行比较，仅当它们引用相同对象时返回true。</li>
</ul>

<div class="note"><strong>注意:</strong> 字符串对象的类型是对象，不是字符串！字符串对象很少被使用，所以下面的结果也许会让你Duang~Duang~Duang~~~</div>

<pre class="brush:js">
// true as both operands are Type String (i.e. string primitives):
'foo' === 'foo'

var a = new String('foo');
var b = new String('foo');

// false as a and b are Type Object and reference different objects
a == b 

// false as a and b are Type Object and reference different objects
a === b 

// true as a and 'foo' are of different type and, the Object (a) 
// is converted to String 'foo' before comparison
a == 'foo' </pre>

<h2 id="Specifications">Specifications</h2>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="col">Specification</th>
   <th scope="col">Status</th>
   <th scope="col">Comment</th>
  </tr>
  <tr>
   <td>ECMAScript 1st Edition.</td>
   <td>Standard</td>
   <td>Initial definition. Implemented in JavaScript 1.0</td>
  </tr>
  <tr>
   <td>ECMAScript 3rd Edition.</td>
   <td>Standard</td>
   <td>Adds <code>===</code> and <code>!==</code> operators. Implemented in JavaScript 1.3</td>
  </tr>
  <tr>
   <td>{{SpecName('ES5.1', '#sec-11.8', 'Relational Operators')}}<br />
    {{SpecName('ES5.1', '#sec-11.9', 'Equality Operators')}}</td>
   <td>{{Spec2('ES5.1')}}</td>
   <td>Defined in several sections of the specification:&nbsp;<a href="http://www.ecma-international.org/ecma-262/5.1/#sec-11.8">Relational Operators</a>,&nbsp;<a href="http://www.ecma-international.org/ecma-262/5.1/#sec-11.9">Equality Operators</a></td>
  </tr>
  <tr>
   <td>{{SpecName('ES6', '#sec-relational-operators', 'Relational Operators')}}<br />
    {{SpecName('ES6', '#sec-equality-operators', 'Equality Operators')}}</td>
   <td>{{Spec2('ES6')}}</td>
   <td>Defined in several sections of the specification:&nbsp;<a href="http://www.ecma-international.org/ecma-262/6.0/#sec-relational-operators">Relational Operators</a>,&nbsp;<a href="http://www.ecma-international.org/ecma-262/6.0/#sec-equality-operators">Equality Operators</a></td>
  </tr>
  <tr>
   <td>{{SpecName('ESDraft', '#sec-relational-operators')}}</td>
   <td>{{Spec2('ESDraft')}}</td>
   <td>Defined in several sections of the specification:&nbsp;<a href="http://tc39.github.io/ecma262/#sec-relational-operators">Relational Operators</a>,&nbsp;<a href="http://tc39.github.io/ecma262/#sec-equality-operators">Equality Operators</a></td>
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

