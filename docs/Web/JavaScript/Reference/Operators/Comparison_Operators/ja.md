---
version: prototype1
revision_id: 1031556
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

<p>JavaScript には、厳密に比較する方法と、型変換した結果で比較する方法の 2 通りがあります。厳密な比較 (例えば <code>===</code>) では、オペランドが同じ型である場合に限り真になります。より一般的に使用される抽象的な比較 (例えば <code>==</code>) では、比較する前にオペランドを同じ型に変換します。抽象的な関係演算子 (例えば <code>&lt;=</code>) では比較する前に、始めにオペランドをプリミティブな値に変換し、さらに同じ型に変換します。</p>

<p>文字列は、Unicode の値を用い、標準の辞書に基づいて比較されます。</p>

<p>比較の機能は以下のとおりです:</p>

<ul>
 <li>2 つの文字列は、文字の順序が同一で、長さが等しく、かつ対応する位置の文字が等しいとき、厳密に等しくなります。</li>
 <li>2 つの数値は、数字的に等しいとき (数字の値が等しいとき)、厳密に等しくなります。<a href="/ja/docs/Web/JavaScript/Reference/Global_Objects/NaN" title="NaN">NaN</a> は、どんなものとも (Nan とさえも) 等しくなりません。プラスゼロとマイナスゼロはそれぞれに対し等しくなります。</li>
 <li>2 つの論理オペランドは、両者が <code>true</code> あるいは両者が <code>false</code> の時、厳密に等しくなります。</li>
 <li>2 つの別個のオブジェクトは、厳密な比較でも抽象的な比較でも等しくなりません。</li>
 <li>オブジェクトを比較する式は、それらが同じオブジェクトを参照しているとき、厳密に等しくなります。</li>
 <li>Null と Undefined の型は、それら自身と厳密に等しく、またお互いが抽象的に等しくなります。</li>
</ul>

<h2 id="Equality_operators" name="Equality_operators">等価演算子</h2>

<h3 id="Equality_()" name="Equality_()"><a name="Equality">等しい (==)</a></h3>

<p>等価演算子は 2 つのオペランドが<strong>同じ型ではないならば</strong>、オペランドを変換し、そして厳密な比較を適用します。もし<strong>両方のオペランドがオブジェクトならば</strong> JavaScript は、オペランドがメモリ内の同じオブジェクトを参照するときに等しくなる、内部参照を比較します。</p>

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

  0   == undefined // false
null  == undefined // true
</pre>

<h3 id="Inequality_(!)" name="Inequality_(!)"><a name="Inequality">等しくない (!=)</a></h3>

<p>不等価演算子は、もしオペランド同士が等しくないならば真を返します。もし 2 つのオペランドが<strong>同じ型ではないならば</strong>、JavaScript は適切な型にオペランドを変換して比較しようと試みます。もし<strong>両方のオペランドがオブジェクトならば</strong> JavaScript は、オペランドがメモリ内の異なるオブジェクトを参照するときに等しくならない、内部参照を比較します。</p>

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

<p>厳密等価演算子はオペランド同士が、<strong>型を変換することなく</strong> (上に示した通り) 厳密に等しいならば真を返します。</p>

<h4 id="Syntax_3" name="Syntax_3">構文</h4>

<pre class="syntaxbox">
x === y</pre>

<h4 id="Examples_3" name="Examples_3">例</h4>

<pre class="brush: js ">
3 === 3   // true
3 === '3' // false</pre>

<h3 id="Non-identity_strict_inequality_(!)" name="Non-identity_strict_inequality_(!)"><a name="Nonidentity">厳密には等しくない (!==)</a></h3>

<p>厳密不等価演算子は、<strong>オペランド同士が等しくない、型が等しくない、あるいはその両方</strong>ならば真を返します。</p>

<h4 id="Syntax_4" name="Syntax_4">構文</h4>

<pre class="syntaxbox">
x !== y</pre>

<h4 id="Examples_4" name="Examples_4">例</h4>

<pre class="brush: js">
3 !== '3' // true
4 !== 3   // true
</pre>

<h2 id="Relational_operators" name="Relational_operators">関係演算子</h2>

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

<p>大なりイコール演算子は、左オペランドが右オペランドより大きいまたは等しいならば、真を返します。</p>

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

<p>小なりイコール演算子は、左オペランドが右オペランドより小さいまたは等しいならば、真を返します。</p>

<h4 id="Syntax_8" name="Syntax_8">構文</h4>

<pre class="syntaxbox">
 x &lt;= y</pre>

<h4 id="Examples_8" name="Examples_8">例</h4>

<pre class="brush: js">
3 &lt;= 4 // true
</pre>

<h2 id="Using_the_Equality_Operators" name="Using_the_Equality_Operators">等価演算子を使う</h2>

<p>通常の等価演算子 (<code>==</code> と <code>!=</code>) は 2 つのオペランドの比較に <a href="http://www.ecma-international.org/ecma-262/5.1/#sec-11.9.3">Abstract Equality Comparison Algorithm</a> を使用します。オペランドの型が異なる場合は、比較を行う前にそれらを同じ型に変換しようとします。例えば <code>5 == '5'</code> という式では、比較を行う前に右オペランドの文字列を数値に変換します。</p>

<p>厳密等価演算子 (<code>===</code> と <code>!==</code>) は <a href="http://www.ecma-international.org/ecma-262/5.1/#sec-11.9.6">Strict Equality Comparison Algorithm</a> を使用して、同一の型かどうかに関する比較も行います。オペランドの型が異なれば、結果は常に <code>false</code> になりますので、<code>5 !== '5'</code> となります。</p>

<p>オペランドがその値だけでなく特定の型でなければならない場合、あるいはオペランドの正確な型が重要である場合には、厳密等価演算子を使ってください。それ以外では通常の等価演算子を使いますが、その場合は 2 つのオペランドがたとえ同じ型でなくても比較が可能になります。</p>

<p>型の変換が必要とされるとき (すなわち厳密でない比較) は、JavaScript は以下のように文字列、数値、論理値、オブジェクトに変換します。</p>

<ul>
 <li>数値と文字列を比較するとき、文字列は数値に変換されます。JavaScript は文字列の数値リテラルを <code>Number</code> 型の数値に変換しようと試みます。最初に、その文字列の数値リテラルから数学的な値を引き出します。次に、最も近い <code>Number</code> 型の値にこの値を丸めます。</li>
 <li>もしオペランドの片方が <code>Boolean</code> ならば、その論理オペランドは <code>true</code> ならば <code>1</code> に、そして <code>false</code> ならば <code>+0</code> に変換されます。</li>
 <li>オブジェクトを数値または文字列と比較する場合、JavaScript はそのオブジェクトの既定値を返そうとします。演算子はそのオブジェクトを、そのオブジェクトの <code>valueOf</code> や <code>toString</code> といったメソッドを用いて、プリミティブな値か、<code>String</code> か、あるいは <code>Number</code> の値に変換しようとします。そうした変換の試みが失敗したときにはランタイムエラーが生成されます。</li>
 <li>比較対象がプリミティブ値である場合のみ、オブジェクトはプリミティブ値に変換されます。両方のオペランドがオブジェクトであれば、それらはオブジェクトとして比較され、両方が同じオブジェクトを参照する場合にのみ、テストは「真」となります。</li>
</ul>

<div class="note"><strong>注記:</strong> 「文字列オブジェクト」はオブジェクトであり、プリミティブな「文字列」とは異なります。通常は「文字列オブジェクト」を用いることは少ないので、次のコードはあなたの意表をつく結果となるものかもしれません。</div>

<pre class="brush:js">
// 両方のオペランドが文字列型 (すなわちプリミティブな文字列) であるため、true が返ります:
'foo' === 'foo'

var a = new String('foo');
var b = new String('foo');

// false。a と b はオブジェクト型であり、異なるオブジェクト同士の比較となります。
a == b 

// false。a と b はオブジェクト型であり、異なるオブジェクト同士の比較となります。
a === b 

// true。a と 'foo' は異なる型であり、オブジェクト (a) は 
// 文字列 'foo' に変換されて比較されます。
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
   <td>最初期の定義。JavaScript 1.0 で実装。</td>
  </tr>
  <tr>
   <td>{{SpecName('ES3')}}</td>
   <td>{{Spec2('ES3')}}</td>
   <td><code>===</code> および <code>!==</code> 演算子を追加。JavaScript 1.3 で実装。</td>
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
 <li><a href="/ja/docs/Web/JavaScript/Equality_comparisons_and_sameness">等価性の比較とその使いどころ</a></li>
</ul>

