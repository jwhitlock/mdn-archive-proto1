---
version: prototype1
revision_id: 1151868
locale: ja
slug: Web/JavaScript/Reference/Operators/Comparison_Operators
tags: "Operator" "JavaScript"
title: 比較演算子
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{jsSidebar("Operators")}}</div>

<p>JavaScript の比較には、厳密な (strict) ものと、型変換を伴うものがあります。厳密な比較 (例えば <code>===</code>) では、オペランドが同じ型で、かつ内容が一致しているときだけ真になります。より一般的に使われる抽象的な (abstract) 比較 (例えば <code>==</code>) では、比較の前にオペランドを同じ型に変換します。抽象的な関係比較&nbsp;(例えば <code>&lt;=</code>) では、比較の前に、まずオペランドをプリミティブな値に変換し、さらに同じ型に変換します。</p>

<p>文字列は、Unicode の値を使って、標準の辞書式順に基づいて比較されます。</p>

<p>比較の機能は以下のとおりです:</p>

<ul>
 <li>2 つの文字列が厳密に等しくなるのは、字の順序が等しく、長さが等しく、対応する位置の文字が等しいときです。</li>
 <li>2 つの数字が厳密に等しくなるのは、数値的に等しいとき (数字の値が等しいとき) です。<a href="/ja/docs/Web/JavaScript/Reference/Global_Objects/NaN" title="NaN">NaN</a> は、どんなものとも (Nan とさえも) 等しくなりません。プラスゼロとマイナスゼロは互いと等しくなります。</li>
 <li>2 つの論理オペランドが厳密に等しくなるのは、どちらも&nbsp;<code>true</code>&nbsp;か、どちらも&nbsp;<code>false</code> のときです。</li>
 <li>2 つの異なるオブジェクトは、厳密な比較でも抽象的な比較でも等しくなりません。</li>
 <li>オブジェクト比較が等しくなるのは、オペランドが同じオブジェクトを参照しているときだけです。</li>
 <li>Null と Undefined 型は、自分自身と厳密に等しく、また互いに抽象的に等しくなります。</li>
</ul>

<h2 id="Equality_operators" name="Equality_operators">等価演算子</h2>

<h3 id="Equality_()" name="Equality_()"><a name="Equality">等しい (==)</a></h3>

<p>等価演算子は、2 つのオペランドが<strong>同じ型でないならば</strong>オペランドを変換して、それから厳密な比較を行います。<strong>両方のオペランドがオブジェクトならば、</strong>JavaScript は内部参照を比較するので、オペランドがメモリ内の同じオブジェクトを参照するときに等しくなります。</p>

<h4 id="Syntax" name="Syntax">構文</h4>

<pre class="syntaxbox">
x == y
</pre>

<h4 id="Examples" name="Examples">例</h4>

<pre class="brush: js">
&nbsp; 1   ==  1        // true
 "1"  ==  1        // true
  1   == '1'       // true
  0   == false     // true
  0   == null      // false
var object1 = {"value":"key"}, object2={"value":"key"};
object1 == object2 // false

  0   == undefined // false
null  == undefined // true
</pre>

<h3 id="Inequality_(!)" name="Inequality_(!)"><a name="Inequality">等しくない (!=)</a></h3>

<p>不等価演算子は、オペランド同士が等しくないならば真を返します。2 つのオペランドが<strong>同じ型でないならば</strong>、JavaScript は適切な型にオペランドを変換して比較しようとします。<strong>両方のオペランドがオブジェクトならば</strong>、JavaScript は内部参照を比較するので、オペランドがメモリ内の異なるオブジェクトを参照するときには等しくなりません。</p>

<h4 id="Syntax_2" name="Syntax_2">構文</h4>

<pre class="syntaxbox">
x != y</pre>

<h4 id="Examples_2" name="Examples_2">例</h4>

<pre class="brush: js">
1 !=   2     // true
1 !=  "1"    // false
1 !=  '1'    // false
1 !=  true   // false
0 !=  false  // false
</pre>

<h3 id="Identity_strict_equality_()" name="Identity_strict_equality_()"><a name="Identity">厳密に等しい (===)</a></h3>

<p>厳密等価演算子はオペランド同士が、<strong>型を変換せずに、</strong>&nbsp;(上に示した通り) 厳密に等しければ真を返します。</p>

<h4 id="Syntax_3" name="Syntax_3">構文</h4>

<pre class="syntaxbox">
x === y</pre>

<h4 id="Examples_3" name="Examples_3">例</h4>

<pre class="brush: js ">
3 === 3   // true
3 === '3' // false
var object1 = {"value":"key"}, object2={"value":"key"};
object1 === object2 // false
</pre>

<h3 id="Non-identity_strict_inequality_(!)" name="Non-identity_strict_inequality_(!)"><a name="Nonidentity">厳密には等しくない (!==)</a></h3>

<p>厳密不等価演算子は、<strong>オペランド同士が等しくないか、型が等しくない、あるいはその両方</strong>ならば真を返します。</p>

<h4 id="Syntax_4" name="Syntax_4">構文</h4>

<pre class="syntaxbox">
x !== y</pre>

<h4 id="Examples_4" name="Examples_4">例</h4>

<pre class="brush: js">
3 !== '3' // true
4 !== 3   // true
</pre>

<h2 id="Relational_operators" name="Relational_operators">関係演算子</h2>

<p>関係演算子は、比較の前に、各オペランドに対して <code>valueOf()</code> 関数を呼ぶ。</p>

<h3 id="Greater_than_operator_(&gt;)" name="Greater_than_operator_(&gt;)"><a name="Greater_than_operator">より大きい (&gt;)</a></h3>

<p>大なり演算子は、左オペランドが右オペランドより大きいならば、真を返します。</p>

<h4 id="Syntax_5" name="Syntax_5">構文</h4>

<pre class="syntaxbox">
x &gt; y</pre>

<h4 id="Examples_5" name="Examples_5">例</h4>

<pre class="brush: js">
4 &gt; 3 // true
</pre>

<h3 id="Greater_than_or_equal_operator_(&gt;)" name="Greater_than_or_equal_operator_(&gt;)"><a name="Greater_than_or_equal_operator">より大きいまたは等しい (以上) (&gt;=)</a></h3>

<p>大なりイコール演算子は、左オペランドが右オペランドより大きいか等しいならば、真を返します。</p>

<h4 id="Syntax_6" name="Syntax_6">構文</h4>

<pre class="syntaxbox">
 x &gt;= y</pre>

<h4 id="Examples_6" name="Examples_6">例</h4>

<pre class="brush: js">
4 &gt;= 3 // true
3 &gt;= 3 // true
</pre>

<h3 id="Less_than_operator_(&lt;)" name="Less_than_operator_(&lt;)"><a name="Less_than_operator">より小さい (&lt;)</a></h3>

<p>小なり演算子は、左オペランドが右オペランドより小さいならば、真を返します。</p>

<h4 id="Syntax_7" name="Syntax_7">構文</h4>

<pre class="syntaxbox">
 x &lt; y</pre>

<h4 id="Examples_7" name="Examples_7">例</h4>

<pre class="brush: js">
3 &lt; 4 // true
</pre>

<h3 id="Less_than_or_equal_operator_(&lt;)" name="Less_than_or_equal_operator_(&lt;)"><a id="Less_than_or_equal_operator" name="Less_than_or_equal_operator">より小さいまたは等しい (以下) (&lt;=)</a></h3>

<p>小なりイコール演算子は、左オペランドが右オペランドより小さいか等しいならば、真を返します。</p>

<h4 id="Syntax_8" name="Syntax_8">構文</h4>

<pre class="syntaxbox">
 x &lt;= y</pre>

<h4 id="Examples_8" name="Examples_8">例</h4>

<pre class="brush: js">
3 &lt;= 4 // true
</pre>

<h2 id="Using_the_Equality_Operators" name="Using_the_Equality_Operators">等価演算子を使う</h2>

<p>標準的な等価演算子 (<code>==</code> と <code>!=</code>) は 2 つのオペランドの比較に <a href="http://www.ecma-international.org/ecma-262/5.1/#sec-11.9.3">Abstract Equality Comparison Algorithm</a> を使用します。オペランドの型が異なる場合は、比較を行う前にそれらを同じ型に変換しようとします。例えば <code>5 == '5'</code> という式では、比較を行う前に右オペランドの文字列を数値に変換します。</p>

<p>厳密等価演算子 (<code>===</code> と <code>!==</code>) は <a href="http://www.ecma-international.org/ecma-262/5.1/#sec-11.9.6">Strict Equality Comparison Algorithm</a> を使用して、同一の型かどうかに関する比較も行います。オペランドの型が異なれば、結果は常に <code>false</code> になりますので、<code>5 !== '5'</code> となります。</p>

<p>厳密等価演算子を使うのは、オペランドが特定の型の特定の値でなければならない場合、言い換えればオペランドの正確な型が重要な場合です。それ以外では、2 つのオペランドが同じ型でなくても比較が可能になる、標準的な等価演算子を使えます。</p>

<p>比較に型の変換が関わるとき (つまり厳密でない比較のとき)、JavaScript は以下のように {{jsxref("String")}}, {{jsxref("Number")}}, {{jsxref("Boolean")}}, &nbsp;{{jsxref("Object")}} 型のオペランドを変換します。</p>

<ul>
 <li>数値と文字列を比較するとき、文字列は数値に変換されます。JavaScript は文字列の数値リテラルを <code>Number</code> 型の値に変換しようとします。まず、文字列の数値リテラルから数学的な値を引き出します。次に、その値を最も近い <code>Number</code> 型に丸めます。</li>
 <li>もしオペランドの片方が <code>Boolean</code> ならば、<code>Boolean</code> オペランドが&nbsp;<code>true</code> の場合 <code>1</code> に、<code>false&nbsp;</code>の場合 <code>+0</code> に変換されます。</li>
 <li>オブジェクトを数値または文字列と比較すると、JavaScript はそのオブジェクトのデフォルト値を返そうとします。演算子は、オブジェクトの&nbsp;<code>valueOf</code> や <code>toString</code> といったメソッドを用いて、プリミティブな値、<code>String</code> か&nbsp;<code>Number</code> の値に変換しようとします。変換に失敗したら、ランタイムエラーを生成します。</li>
 <li>オブジェクトがプリミティブ値に変換されるのは、比較対象がプリミティブ値であるときだけです。両方のオペランドがオブジェクトなら、オブジェクトとして比較され、両方が同じオブジェクトを参照するときだけ真となります。</li>
</ul>

<div class="note"><strong>注記:</strong>&nbsp;文字列オブジェクトはオブジェクトであり、文字列ではありません！　文字列オブジェクトはほとんど使わないので、次の結果は驚くことがあるかもしれません：</div>

<pre class="brush:js">
// 両方のオペランドが文字列型 (すなわちプリミティブな文字列) なので、true:
'foo' === 'foo'

var a = new String('foo');
var b = new String('foo');

// a と b はオブジェクト型で、異なるオブジェクトを参照しているので、false
a == b 

// a と b はオブジェクト型で、異なるオブジェクトを参照しているので、false 

// a と 'foo' は異なる型で、比較前にオブジェクト (a) は 
// 文字列 'foo' に変換されるので、真
a == 'foo'</pre>

<h2 id="Specifications" name="Specifications">仕様</h2>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="col">仕様書</th>
   <th scope="col">策定状況</th>
   <th scope="col">コメント</th>
  </tr>
  <tr>
   <td>{{SpecName('ES1')}}</td>
   <td>{{Spec2('ES1')}}</td>
   <td>最初の定義。JavaScript 1.0 で実装。</td>
  </tr>
  <tr>
   <td>{{SpecName('ES3')}}</td>
   <td>{{Spec2('ES3')}}</td>
   <td><code>===</code>&nbsp;と<code>!==</code> 演算子を追加。JavaScript 1.3 で実装。</td>
  </tr>
  <tr>
   <td>{{SpecName('ES5.1', '#sec-11.8')}}</td>
   <td>{{Spec2('ES5.1')}}</td>
   <td>仕様書内のいくつかのセクションで定義: <a href="http://www.ecma-international.org/ecma-262/5.1/#sec-11.8">Relational Operators</a>, <a href="http://www.ecma-international.org/ecma-262/5.1/#sec-11.9">Equality Operators</a></td>
  </tr>
  <tr>
   <td>{{SpecName('ES6', '#sec-relational-operators')}}</td>
   <td>{{Spec2('ES6')}}</td>
   <td>仕様書内のいくつかのセクションで定義: <a href="http://www.ecma-international.org/ecma-262/6.0/#sec-relational-operators">Relational Operators</a>, <a href="http://www.ecma-international.org/ecma-262/6.0/#sec-equality-operators">Equality Operators</a></td>
  </tr>
  <tr>
   <td>{{SpecName('ESDraft', '#sec-relational-operators')}}</td>
   <td>{{Spec2('ESDraft')}}</td>
   <td>仕様書内のいくつかのセクションで定義: <a href="http://tc39.github.io/ecma262/#sec-relational-operators">Relational Operators</a>, <a href="http://tc39.github.io/ecma262/#sec-equality-operators">Equality Operators</a></td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility" name="Browser_compatibility">ブラウザ実装状況</h2>

<div>{{CompatibilityTable}}</div>

<div id="compat-desktop">
<table class="compat-table">
 <tbody>
  <tr>
   <th>機能</th>
   <th>Chrome</th>
   <th>Firefox (Gecko)</th>
   <th>Internet Explorer</th>
   <th>Opera</th>
   <th>Safari</th>
  </tr>
  <tr>
   <td>基本サポート</td>
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
   <th>機能</th>
   <th>Android</th>
   <th>Chrome for Android</th>
   <th>Firefox Mobile (Gecko)</th>
   <th>IE Mobile</th>
   <th>Opera Mobile</th>
   <th>Safari Mobile</th>
  </tr>
  <tr>
   <td>基本サポート</td>
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

<h2 id="See_also" name="See_also">関連情報</h2>

<ul>
 <li>{{jsxref("Object.is()")}}</li>
 <li>{{jsxref("Math.sign()")}}</li>
 <li><a href="/ja/docs/Web/JavaScript/Equality_comparisons_and_sameness">等価性の比較とその使いどころ</a></li>
</ul>

