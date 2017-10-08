---
version: prototype1
revision_id: 1316433
locale: uk
slug: Web/JavaScript/Reference/Operators/Оператори_порівняння
tags: "Довідка" "Оператор" "JavaScript"
title: Оператори порівняння
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: a9e46eea3dbc99cdc2b66ac8e6ad971d4b83072b
---
<div>{{jsSidebar("Operators")}}</div>

<p>JavaScript has both strict and type–converting comparisons. A strict comparison (e.g., <code>===</code>) is only true if the operands are of the same type and the contents match. The more commonly-used abstract comparison (e.g. <code>==</code>) converts the operands to the same type before making the comparison. For relational abstract comparisons (e.g., <code>&lt;=</code>), the operands are first converted to primitives, then to the same type, before comparison.</p>

<p>Strings are compared based on standard lexicographical ordering, using Unicode values.</p>

<p>Features of comparisons:</p>

<ul>
 <li>Two strings are strictly equal when they have the same sequence of characters, same length, and same characters in corresponding positions.</li>
 <li>Two numbers are strictly equal when they are numerically equal (have the same number value). <a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects/NaN" title="NaN">NaN</a> is not equal to anything, including NaN. Positive and negative zeros are equal to one another.</li>
 <li>Two Boolean operands are strictly equal if both are <code>true</code> or both are <code>false</code>.</li>
 <li>Two distinct objects are never equal for either strict or abstract comparisons.</li>
 <li>An expression comparing Objects is only true if the operands reference the same Object.</li>
 <li>Null and Undefined Types are strictly equal&nbsp;to themselves and abstractly equal&nbsp;to each other.</li>
</ul>

<h2 id="Equality_operators">Оператори рівності</h2>

<h3 id="Equality_()"><a name="Equality">Equality (==)</a></h3>

<p>The equality operator converts the operands if they are <strong>not of the same type</strong>, then applies strict comparison. If <strong>both operands are objects</strong>, then JavaScript compares internal references which are equal when operands refer to the same object in memory.</p>

<h4 id="Syntax">Syntax</h4>

<pre class="syntaxbox">
x == y
</pre>

<h4 id="Examples">Examples</h4>

<pre class="brush: js">
1    ==  1         // true
'1'  ==  1         // true
1    == '1'        // true
0    == false      // true
0    == null       // false
var object1 = {'value': 'key'}, object2 = {'value': 'key'}; 
object1 == object2 //false
0    == undefined  // false
null == undefined  // true
</pre>

<h3 id="Inequality_(!)"><a name="Inequality">Inequality (!=)</a></h3>

<p>The inequality operator returns true if the operands are not equal. If the two operands are <strong>not of the same type</strong>, JavaScript attempts to convert the operands to an appropriate type for the comparison.&nbsp;If <strong>both operands are&nbsp;objects</strong>, then JavaScript compares internal references which are not equal when operands refer to different objects in memory.</p>

<h4 id="Syntax_2">Syntax</h4>

<pre class="syntaxbox">
x != y</pre>

<h4 id="Examples_2">Examples</h4>

<pre class="brush: js">
1 !=   2     // true
1 !=  '1'    // false
1 !=  "1"    // false
1 !=  true   // false
0 !=  false  // false
</pre>

<h3 id="Identity_strict_equality_()"><a name="Identity">Identity / strict equality (===)</a></h3>

<p>The identity operator returns true if the operands are strictly equal (see above) <strong>with no type conversion</strong>.&nbsp;</p>

<h4 id="Syntax_3">Syntax</h4>

<pre class="syntaxbox">
x === y</pre>

<h4 id="Examples_3">Examples</h4>

<pre class="brush: js ">
3 === 3   // true
3 === '3' // false
var object1 = {'value': 'key'}, object2 = {'value': 'key'};
object1 === object2 //false</pre>

<p>&nbsp;</p>

<h3 id="Non-identity_strict_inequality_(!)"><a name="Nonidentity">Non-identity / strict inequality (!==)</a></h3>

<p>The non-identity operator returns true if the operands <strong>are not equal and/or not of the same type</strong>.</p>

<h4 id="Syntax_4">Syntax</h4>

<pre class="syntaxbox">
x !== y</pre>

<h4 id="Examples_4">Examples</h4>

<pre class="brush: js">
3 !== '3' // true
4 !== 3   // true
</pre>

<h2 id="Relational_operators">Оператори відношення</h2>

<p>Each of these operators will call the&nbsp;<code>valueOf()</code>&nbsp;function on each operand before a comparison is made.</p>

<h3 id="Greater_than_operator_(&gt;)"><a name="Greater_than_operator">Greater than operator (&gt;)</a></h3>

<p>The greater than operator returns true if the left operand is greater than the right operand.</p>

<h4 id="Syntax_5">Syntax</h4>

<pre class="syntaxbox">
x &gt; y</pre>

<h4 id="Examples_5">Examples</h4>

<pre class="brush: js">
4 &gt; 3 // true
</pre>

<h3 id="Greater_than_or_equal_operator_(&gt;)"><a name="Greater_than_or_equal_operator">Greater than or equal operator (&gt;=)</a></h3>

<p>The greater than or equal operator returns true if the left operand is greater than or equal to the right operand.</p>

<h4 id="Syntax_6">Syntax</h4>

<pre class="syntaxbox">
 x &gt;= y</pre>

<h4 id="Examples_6">Examples</h4>

<pre class="brush: js">
4 &gt;= 3 // true
3 &gt;= 3 // true
</pre>

<h3 id="Less_than_operator_(&lt;)"><a name="Less_than_operator">Less than operator (&lt;)</a></h3>

<p>The less than operator returns true if the left operand is less than the right operand.</p>

<h4 id="Syntax_7">Syntax</h4>

<pre class="syntaxbox">
 x &lt; y</pre>

<h4 id="Examples_7">Examples</h4>

<pre class="brush: js">
3 &lt; 4 // true
</pre>

<h3 id="Less_than_or_equal_operator_(&lt;)"><a id="Less_than_or_equal_operator" name="Less_than_or_equal_operator">Less than or equal operator (&lt;=)</a></h3>

<p>The less than or equal operator returns true if the left operand is less than or equal to the right operand.</p>

<h4 id="Syntax_8">Syntax</h4>

<pre class="syntaxbox">
 x &lt;= y</pre>

<h4 id="Examples_8">Examples</h4>

<pre class="brush: js">
3 &lt;= 4 // true
</pre>

<h2 id="Using_the_Equality_Operators">Вжиток операторів порівняння</h2>

<p>The standard equality operators (<code>==</code> and <code>!=</code>) use the <a href="http://www.ecma-international.org/ecma-262/5.1/#sec-11.9.3">Abstract Equality Comparison Algorithm</a> to compare two operands. If the operands are of different types, it will attempt to convert them to the same type before making the comparison, e.g., in the expression <code>5 == '5'</code>, the string on the right is converted to {{jsxref("Number")}} before the comparison is made.</p>

<p>The strict equality operators (<code>===</code> and <code>!==</code>) use the <a href="http://www.ecma-international.org/ecma-262/5.1/#sec-11.9.6">Strict Equality Comparison Algorithm</a> and are intended for performing equality comparisons on operands of the same type. If the operands are of different types, the result is always <code>false</code> so <code>5 !== '5'</code>.</p>

<p>Use strict equality operators if the operands must be of a specific type as well as value or if the exact type of the operands is important. Otherwise, use the standard equality operators, which allow you to compare the identity of two operands even if they are not of the same type.</p>

<p>When type conversion is involved in the comparison (i.e., non–strict comparison), JavaScript converts the types {{jsxref("String")}}, {{jsxref("Number")}}, {{jsxref("Boolean")}}, or {{jsxref("Object")}} operands as follows:</p>

<ul>
 <li>When comparing a number and a string, the string is converted to a number value. JavaScript attempts to convert the string numeric literal to a <code>Number</code> type value. First, a mathematical value is derived from the string numeric literal. Next, this value is rounded to nearest <code>Number</code> type value.</li>
 <li>If one of the operands is <code>Boolean</code>, the Boolean operand is converted to 1 if it is <code>true</code> and +0 if it is <code>false</code>.</li>
 <li>If an object is compared with a number or string, JavaScript attempts to return the default value for the object. Operators attempt to convert the object to a primitive value, a <code>String</code> or <code>Number</code> value, using the <code>valueOf</code> and <code>toString</code> methods of the objects. If this attempt to convert the object fails, a runtime error is generated.</li>
 <li>Note that an object is converted into a primitive if, and only if, its comparand is a primitive. If both operands are objects, they're compared as objects, and the equality test is true only if both refer the same object.</li>
</ul>

<div class="note"><strong>Note:</strong> String objects are Type Object, not String! String objects are rarely used, so the following results might be surprising:</div>

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

<h2 id="Specifications">Специфікації</h2>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="col">Специфікація</th>
   <th scope="col">Статус</th>
   <th scope="col">Коментар</th>
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

<h2 id="Browser_compatibility">Підтримка веб-переглядачами</h2>

<div class="hidden">The compatibility table on this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</div>

<p>{{Compat("javascript.operators.comparison")}}</p>

<h2 id="See_also">Див. також</h2>

<ul>
 <li>{{jsxref("Object.is()")}}</li>
 <li>{{jsxref("Math.sign()")}}</li>
 <li><a href="/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness">Equality comparisons and sameness</a></li>
</ul>

