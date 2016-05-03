---
version: prototype1
revision_id: 1050348
locale: ja
slug: Web/JavaScript/Reference/Operators
tags: "JavaScript" "Operators"
title: 式と演算子
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{jsSidebar("Operators")}}</div>

<p>この章では、JavaScript 言語のすべての演算子、式、キーワードについて文書化しています。</p>

<h2 id="Expressions_and_operators_by_category" name="Expressions_and_operators_by_category">式と演算子 (カテゴリ別)</h2>

<p>アルファベット順リストは左側のサイドバーをご覧ください。</p>

<h3 id="Primary_expressions" name="Primary_expressions">基本式</h3>

<p>JavaScript の基本的なキーワードと一般的な式です。</p>

<dl>
 <dt>{{jsxref("Operators/this", "this")}}</dt>
 <dd><code>this</code> キーワードは関数の実行コンテキストを参照します。</dd>
 <dt>{{jsxref("Operators/function", "function")}}</dt>
 <dd><code>function</code> キーワードは関数式を定義します。</dd>
 <dt>{{jsxref("Operators/class", "class")}}</dt>
 <dd><code>class</code> キーワードはクラス式を定義します。</dd>
 <dt>{{jsxref("Operators/function*", "function*")}}</dt>
 <dd><code>function*</code> キーワードはジェネレータ関数式を定義します。</dd>
 <dt>{{jsxref("Operators/yield", "yield")}}</dt>
 <dd>ジェネレータ関数の一時停止と再開を行います。</dd>
 <dt>{{jsxref("Operators/yield*", "yield*")}}</dt>
 <dd>別のジェネレータ関数または反復可能オブジェクトを代行します。</dd>
 <dt>{{jsxref("Global_Objects/Array", "[]")}}</dt>
 <dd>配列初期化子またはリテラル構文です。</dd>
 <dt>{{jsxref("Operators/Object_initializer", "{}")}}</dt>
 <dd>オブジェクト初期化子またはリテラル構文です。</dd>
 <dt>{{jsxref("Global_Objects/RegExp", "/ab+c/i")}}</dt>
 <dd>正規表現式のリテラル構文です。</dd>
 <dt>{{jsxref("Operators/Grouping", "( )")}}</dt>
 <dd>グループ化演算子です。</dd>
</dl>

<h3 id="Left-hand-side_expressions" name="Left-hand-side_expressions">左辺式</h3>

<p>左辺値は、代入の対象になります。</p>

<dl>
 <dt>{{jsxref("Operators/Property_accessors", "プロパティアクセス演算子", "", 1)}}</dt>
 <dd>プロパティアクセス演算子はオブジェクトのプロパティやメソッドへのアクセスを提供します<br>
 (<code>object.property</code> や <code>object["property"]</code>)。</dd>
 <dt>{{jsxref("Operators/new", "new")}}</dt>
 <dd><code>new</code> 演算子はコンストラクタのインスタンスを作成します。</dd>
 <dt><a href="/docs/Web/JavaScript/Reference/Operators/new.target">new.target</a></dt>
 <dd>コンストラクタ内で <code>new.target</code> を使うことで、{{jsxref("Operators/new", "new")}} によって呼び出されるコンストラクタを参照できます。</dd>
 <dt>{{jsxref("Operators/super", "super")}}</dt>
 <dd><code>super</code> キーワードは親コンストラクタを呼び出します。</dd>
 <dt>{{jsxref("Operators/Spread_operator", "...obj")}}</dt>
 <dd>展開演算子 (スプレッド演算子) は、式を複数の引数または複数の要素に展開して、それぞれ関数呼び出しまたは配列リテラルに渡します。</dd>
</dl>

<h3 id="Increment_and_decrement" name="Increment_and_decrement">インクリメントとデクリメント</h3>

<p>接尾/接頭辞のインクリメント演算子と接尾/接頭辞のデクリメント演算子です。</p>

<dl>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "A++", "#Increment")}}</dt>
 <dd>接尾辞インクリメント演算子。</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "A--", "#Decrement")}}</dt>
 <dd>接尾辞デクリメント演算子。</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "++A", "#Increment")}}</dt>
 <dd>接頭辞インクリメント演算子。</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "--A", "#Decrement")}}</dt>
 <dd>接頭辞デクリメント演算子。</dd>
</dl>

<h3 id="Unary_operators" name="Unary_operators">単項演算子</h3>

<p>単項演算は、1 個のオペランドによる演算です。</p>

<dl>
 <dt>{{jsxref("Operators/delete", "delete")}}</dt>
 <dd><code>delete</code> 演算子は、オブジェクトからプロパティを削除します。</dd>
 <dt>{{jsxref("Operators/void", "void")}}</dt>
 <dd><code>void</code> 演算子は、式の戻り値を破棄します。</dd>
 <dt>{{jsxref("Operators/typeof", "typeof")}}</dt>
 <dd><code>typeof</code> 演算子は、与えられたオブジェクトの型を判別します。</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "+", "#Unary_plus")}}</dt>
 <dd>単項正値演算子は、そのオペランドを Number 型に変換します。</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "-", "#Unary_negation")}}</dt>
 <dd>単項負値演算子は、そのオペランドを Number 型に変換して正負を反転します。</dd>
 <dt>{{jsxref("Operators/Bitwise_Operators", "~", "#Bitwise_NOT")}}</dt>
 <dd>ビット否定演算子です。</dd>
 <dt>{{jsxref("Operators/Logical_Operators", "!", "#Logical_NOT")}}</dt>
 <dd>論理否定演算子です。</dd>
</dl>

<h3 id="Arithmetic_operators" name="Arithmetic_operators">算術演算子</h3>

<p>算術演算子は、数値 (リテラルまたは値) をオペランドとして取り、1 個の数値を返します。</p>

<dl>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "+", "#Addition")}}</dt>
 <dd>加算演算子です。</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "-", "#Subtraction")}}</dt>
 <dd>減算演算子です。</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "/", "#Division")}}</dt>
 <dd>除算演算子です。</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "*", "#Multiplication")}}</dt>
 <dd>乗算演算子です。</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "%", "#Remainder")}}</dt>
 <dd>剰余演算子です。</dd>
</dl>

<dl>
 <dt>{{experimental_inline}} {{jsxref("Operators/Arithmetic_Operators", "**", "#Exponentiation")}}</dt>
 <dd>べき乗演算子です。</dd>
</dl>

<h3 id="Relational_operators" name="Relational_operators">関係演算子</h3>

<p>比較演算子は、そのオペランドを比較し、その比較が真かどうかに基づいて <code>Boolean</code> 値を返します。</p>

<dl>
 <dt>{{jsxref("Operators/in", "in")}}</dt>
 <dd><code>in</code> 演算子は、与えられたプロパティをオブジェクトが持っているかどうかを判別します。</dd>
 <dt>{{jsxref("Operators/instanceof", "instanceof")}}</dt>
 <dd><code>instanceof</code> 演算子は、オブジェクトが別のオブジェクトのインスタンスかどうかを判別します。</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "&lt;", "#Less_than_operator")}}</dt>
 <dd>小なり演算子です。</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "&gt;", "#Greater_than_operator")}}</dt>
 <dd>大なり演算子です。</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "&lt;=", "#Less_than_or_equal_operator")}}</dt>
 <dd>以下演算子です。</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "&gt;=", "#Greater_than_or_equal_operator")}}</dt>
 <dd>以上演算子です。</dd>
</dl>

<div class="note">
<p><strong>注記: =></strong> は演算子ではなく、<a href="/docs/Web/JavaScript/Reference/Functions/Arrow_functions">アロー関数</a> のためのノーテーションです。</p>
</div>

<h3 id="Equality_operators" name="Equality_operators">等値演算子</h3>

<p>等値演算子の評価結果は常に、比較が真かどうかに基づいて <code>Boolean</code> 型の値になります。</p>

<dl>
 <dt>{{jsxref("Operators/Comparison_Operators", "==", "#Equality")}}</dt>
 <dd>等値演算子です。</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "!=", "#Inequality")}}</dt>
 <dd>不等値演算子です。</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "===", "#Identity")}}</dt>
 <dd>同値演算子です。</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "!==", "#Nonidentity")}}</dt>
 <dd>非同値演算子です。</dd>
</dl>

<h3 id="Bitwise_shift_operators" name="Bitwise_shift_operators">ビットシフト演算子</h3>

<p>オペランドのすべてのビットをシフト演算します。</p>

<dl>
 <dt>{{jsxref("Operators/Bitwise_Operators", "&lt;&lt;", "#Left_shift")}}</dt>
 <dd>ビット左シフト演算子です。</dd>
 <dt>{{jsxref("Operators/Bitwise_Operators", "&gt;&gt;", "#Right_shift")}}</dt>
 <dd>ビット右シフト演算子です。</dd>
 <dt>{{jsxref("Operators/Bitwise_Operators", "&gt;&gt;&gt;", "#Unsigned_right_shift")}}</dt>
 <dd>ビット符号なし右シフト演算子です。</dd>
</dl>

<h3 id="Binary_bitwise_operators" name="Binary_bitwise_operators">バイナリビット演算子</h3>

<p>ビット演算子は、そのオペランドを 32 ビット (0 と 1) の並びとして扱い、標準の JavaScript 数値を返します。</p>

<dl>
 <dt>{{jsxref("Operators/Bitwise_Operators", "&amp;", "#Bitwise_AND")}}</dt>
 <dd>ビット論理積 (AND) です。</dd>
 <dt>{{jsxref("Operators/Bitwise_Operators", "|", "#Bitwise_OR")}}</dt>
 <dd>ビット論理和 (OR) です。</dd>
 <dt>{{jsxref("Operators/Bitwise_Operators", "^", "#Bitwise_XOR")}}</dt>
 <dd>ビット排他的論理和 (XOR) です。</dd>
</dl>

<h3 id="Binary_logical_operators" name="Binary_logical_operators">バイナリ論理演算子</h3>

<p>論理演算には、一般的に (論理) 真偽値が使用され、それが置かれた時に真偽値を返します。</p>

<dl>
 <dt>{{jsxref("Operators/Logical_Operators", "&amp;&amp;", "#Logical_AND")}}</dt>
 <dd>論理積 (AND) です。</dd>
 <dt>{{jsxref("Operators/Logical_Operators", "||", "#Logical_OR")}}</dt>
 <dd>論理和 (OR) です。</dd>
</dl>

<h3 id="Conditional_(ternary)_operator" name="Conditional_(ternary)_operator">条件 (三項) 演算子</h3>

<dl>
 <dt>{{jsxref("Operators/Conditional_Operator", "(condition ? ifTrue : ifFalse)")}}</dt>
 <dd>
 <p>この条件演算子は、条件の論理値を基に、2 つの値のいずれか一方を返します。</p>
 </dd>
</dl>

<h3 id="Assignment_operators" name="Assignment_operators">代入演算子</h3>

<p>代入演算子は、右辺のオペランドに基づいて、値を左辺のオペランドに代入します。</p>

<dl>
 <dt>{{jsxref("Operators/Assignment_Operators", "=", "#Assignment")}}</dt>
 <dd>代入演算子です。</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "*=", "#Multiplication_assignment")}}</dt>
 <dd>乗算値を代入します。</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "/=", "#Division_assignment")}}</dt>
 <dd>除算値を代入します。</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "%=", "#Remainder_assignment")}}</dt>
 <dd>剰余値を代入します。</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "+=", "#Addition_assignment")}}</dt>
 <dd>加算値を代入します。</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "-=", "#Subtraction_assignment")}}</dt>
 <dd>減算値を代入します。</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "&lt;&lt;=", "#Left_shift_assignment")}}</dt>
 <dd>左シフトした値を代入します。</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "&gt;&gt;=", "#Right_shift_assignment")}}</dt>
 <dd>右シフトした値を代入します。</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "&gt;&gt;&gt;=", "#Unsigned_right_shift_assignment")}}</dt>
 <dd>符号なしの右シフトした値を代入します。</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "&amp;=", "#Bitwise_AND_assignment")}}</dt>
 <dd>ビット論理積 (AND) の値を代入します。</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "^=", "#Bitwise_XOR_assignment")}}</dt>
 <dd>ビット排他的論理和 (XOR) の値を代入します。</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "|=", "#Bitwise_OR_assignment")}}</dt>
 <dd>ビット論理和 (OR) の値を代入します。</dd>
 <dt>{{jsxref("Operators/Destructuring_assignment", "[a, b] = [1, 2]")}}<br />
 {{jsxref("Operators/Destructuring_assignment", "{a, b} = {a:1, b:2}")}}</dt>
 <dd>
 <p>分割代入は、配列やオブジェクトのプロパティを、配列やオブジェクトリテラルに似た構文を使用して変数に代入します。</p>
 </dd>
</dl>

<h3 id="Comma_operator" name="Comma_operator">カンマ演算子</h3>

<dl>
 <dt>{{jsxref("Operators/Comma_Operator", ",")}}</dt>
 <dd>カンマ演算子は、複数の式を単一の文で評価し、その最後の式の結果を返します。</dd>
</dl>

<h3 id="Non-standard_features" name="Non-standard_features">非標準の機能</h3>

<dl>
 <dt>{{non-standard_inline}} {{jsxref("Operators/Legacy_generator_function", "レガシージェネレータ関数", "", 1)}}</dt>
 <dd><code>function</code> キーワードは、式の内部でレガシージェネレータ関数の定義に使用されます。関数をレガシージェネレータにするには、関数本体に少なくとも 1 個の {{jsxref("Operators/yield", "yield")}} 式を含めてください。</dd>
 <dt>{{non-standard_inline}} {{jsxref("Operators/Expression_closures", "式クロージャ", "", 1)}}</dt>
 <dd>式クロージャ構文は、単純な関数を書くための省略記法です。</dd>
 <dt>{{non-standard_inline}} {{jsxref("Operators/Array_comprehensions", "[for (x of y) x]")}}</dt>
 <dd>配列内包表記です。</dd>
 <dt>{{non-standard_inline}} {{jsxref("Operators/Generator_comprehensions", "(for (x of y) y)")}}</dt>
 <dd>ジェネレータ内包表記です。</dd>
</dl>

<h2 id="Specifications" name="Specifications">仕様</h2>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="col">仕様書</th>
   <th scope="col">状況</th>
   <th scope="col">コメント</th>
  </tr>
  <tr>
   <td>{{SpecName('ES1', '#sec-11', 'Expressions')}}</td>
   <td>{{Spec2('ES1')}}</td>
   <td>初期定義。</td>
  </tr>
  <tr>
   <td>{{SpecName('ES5.1', '#sec-11', 'Expressions')}}</td>
   <td>{{Spec2('ES5.1')}}</td>
   <td> </td>
  </tr>
  <tr>
   <td>{{SpecName('ES6', '#sec-ecmascript-language-expressions', 'ECMAScript Language: Expressions')}}</td>
   <td>{{Spec2('ES6')}}</td>
   <td>新仕様: 展開演算子、分割代入、<code>super</code> キーワード、配列内包表記、ジェネレータ内包表記</td>
  </tr>
  <tr>
   <td>{{SpecName('ESDraft', '#sec-ecmascript-language-expressions', 'ECMAScript Language: Expressions')}}</td>
   <td>{{Spec2('ESDraft')}}</td>
   <td> </td>
  </tr>
 </tbody>
</table>

<h2 id="See_also" name="See_also">関連項目</h2>

<ul>
 <li><a href="/docs/Web/JavaScript/Reference/Operators/Operator_Precedence">演算子の優先順位</a></li>
</ul>

