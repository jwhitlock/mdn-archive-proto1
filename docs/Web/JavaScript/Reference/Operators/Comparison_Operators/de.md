---
version: prototype1
revision_id: 891259
locale: de
slug: Web/JavaScript/Reference/Operators/Vergleichsoperatoren
tags: "JavaScript" "Vergleichsoperator"
title: Vergleichsoperatoren
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{jsSidebar("Operators")}}</div>

<p>JavaScript kennt sowohl den strikten als auch nicht-strikten&nbsp;Vergleich. Ein strikter Vergleich (z.B. ===) ist nur wahr bei Operanden gleichen Typs. Der häufiger verwendete nicht-strikter&nbsp;Vergleich (z.B. ==) wandelt die Operanden in den gleichen Typen um, bevor sie verglichen werden.&nbsp;Bei relationalen&nbsp;Vergleichsoperatoren&nbsp;(z.B. &lt;=) werden die Operanden vor dem Vergleich zuerst in elementare&nbsp;Datentypen konvertiert und&nbsp;dann in gleiche&nbsp;Typen umgewandelt.</p>

<p>Zeichenketten werden entsprechend der&nbsp;lexikographischen Ordnung verglichen, basierend auf den Unicode.</p>

<p>Merkmale von Vergleichen:</p>

<ul>
 <li>Zwei Zeichenketten sind strikt&nbsp;gleich, wenn sie die gleiche Abfolge von Zeichen, die gleiche Länge und die gleichen Zeichen in übereinstimmenden Positionen haben.</li>
 <li>Zwei Zahlen sind strikt gleich, wenn sie numerisch gleich sind (den gleichen Zahlwert haben). <a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects/NaN" title="NaN">NaN</a>&nbsp;ist mit nichts gleich, auch nicht mit sich selbst.&nbsp;Positive und&nbsp;negative Nullen&nbsp;sind strikt gleich.</li>
 <li>Zwei Boolesche Operanden sind exakt gleich wenn beide <code>true</code>&nbsp;oder beide&nbsp;<code>false</code> sind.</li>
 <li>Zwei unterschiedliche&nbsp;Objekte sind niemals gleich, weder in&nbsp;strikten noch&nbsp;nicht-strikten&nbsp;Vergleichen.</li>
 <li>Ein Ausdruck, der Objekte vergleicht, gilt als&nbsp;wahr (<code>true</code>), wenn die Operanden auf das gleiche Objekt zeigen.</li>
 <li>Die Typen <code>Null</code> und <code>undefined</code> sind sich gegenüber strikt gleich und gegenseitig nicht-strikt gleich.</li>
</ul>

<h2 id="Gleichheitsoperatoren">Gleichheitsoperatoren</h2>

<h3 id="Gleichheit_()"><a name="Equality">Gleichheit (==)</a></h3>

<p>Der Gleichheitsoperator vergleicht zwei Operanden.&nbsp;Sind die Operanden <strong>nicht gleichen Typs</strong> werden sie zuerst umgewandelt. Sind&nbsp;<strong>beide Operanden Objekte</strong>, vergleicht JavaScript die Referenzen;&nbsp;Referenzen gelten als gleich, wenn sie auf das gleiche Objekt im Speicher&nbsp;zeigen.</p>

<h4 id="Syntax">Syntax</h4>

<pre class="syntaxbox">
x == y
</pre>

<h4 id="Beispiele">Beispiele</h4>

<pre class="brush: js">
 1   ==  1     // true
"1"  ==  1     // true
 1   == '1'    // true
 0   == false  // true
</pre>

<h3 id="Ungleichheit_(!)"><a name="Inequality">Ungleichheit (!=)</a></h3>

<p>Der Ungleichheitsoperator gibt wahr zurück, wenn die Operanden nicht gleich sind. Wenn die beiden Operanden <strong>nicht vom gleichen Typ </strong>sind, versucht JavaScript die Operanden in einen passenden Typ für den Vergleich umzuwandeln. Wenn <strong>beide&nbsp;Operanden Objekte sind</strong>, vergleicht JavaScript die Referenzen;&nbsp;Referenzen sind ungleich, wenn sie&nbsp;auf verschiedene Objekte im Speicher verweisen.</p>

<p>Syntax</p>

<pre class="syntaxbox">
x != y</pre>

<h4 id="Beispiele_2">Beispiele</h4>

<pre class="brush: js">
1 !=   2     // true
1 !=  "1"    // false
1 !=  '1'    // false
1 !=  true   // false
0 !=  false  // false
</pre>

<h3 id="Identität_strikte_Gleichheit_()"><a name="Identity">Identität&nbsp;/ strikte Gleichheit&nbsp;(===)</a></h3>

<p>Der Identitätsoperator gibt wahr zurück, wenn die Operanden strikt gleich sind (siehe oben). Insbesondere werden die Operanden vor dem Vergleich nicht konvertiert.</p>

<h4 id="Syntax_2">Syntax</h4>

<pre class="syntaxbox">
x === y</pre>

<h4 id="Beispiele_3">Beispiele</h4>

<pre class="brush: js ">
3 === 3   // true
3 === '3' // false</pre>

<h3 id="Strikte_Ungleichheit_(!)"><a name="Nonidentity">Strikte Ungleichheit (!==)</a></h3>

<p>Der strikte Ungleichheitsoperator gibt wahr zurück, wenn die Operanden<strong>&nbsp;nicht vom gleichen Typ sind bzw. ungleich sind</strong>.</p>

<h4 id="Syntax_3">Syntax</h4>

<pre class="syntaxbox">
x !== y</pre>

<h4 id="Beispiele_4">Beispiele</h4>

<pre class="brush: js">
3 !== '3' // true
4 !== 3   // true
</pre>

<h2 id="Relationale_Operatoren">Relationale Operatoren</h2>

<h3 id="Operator_größer_als_(&gt;)"><a name="Greater_than_operator">Operator größer als&nbsp;(&gt;)</a></h3>

<p>Der Größer-als-Operator gibt wahr zurück, wenn der linke Operand größer als der rechte Operand ist.</p>

<h4 id="Syntax_4">Syntax</h4>

<pre class="syntaxbox">
x &gt; y</pre>

<h4 id="Beispiele_5">Beispiele</h4>

<pre class="brush: js">
4 &gt; 3 // true
</pre>

<h3 id="Operator_größer_oder_gleich_(&gt;)"><a name="Greater_than_or_equal_operator">Operator größer oder gleich (&gt;=)</a></h3>

<p>Der Operator größer-oder-gleich gibt wahr zurück, wenn der linke Operand größer als oder gleich dem rechten Operanden ist.</p>

<h4 id="Syntax_5">Syntax</h4>

<pre class="syntaxbox">
 x &gt;= y</pre>

<h4 id="Beispiele_6">Beispiele</h4>

<pre class="brush: js">
4 &gt;= 3 // true
3 &gt;= 3 // true
</pre>

<h3 id="Operator_kleiner_als_(&lt;)"><a name="Less_than_operator">Operator kleiner als (&lt;)</a></h3>

<p>Der Kleiner-als-Operator gibt wahr zurück, wenn der linke Operand kleiner als der rechte Operand ist.</p>

<h4 id="Syntax_6">Syntax</h4>

<pre class="syntaxbox">
 x &lt; y</pre>

<h4 id="Beispiele_7">Beispiele</h4>

<pre class="brush: js">
3 &lt; 4 // true
</pre>

<h3 id="Operator_kleiner_oder_gleich_(&lt;)"><a id="Less_than_or_equal_operator" name="Less_than_or_equal_operator">Operator kleiner oder gleich (&lt;=)</a></h3>

<p>Der Kleiner-oder-gleich-Operator gibt wahr zurück, wenn der linke Operand kleiner oder gleich dem rechten Operanden ist.</p>

<h4 id="Syntax_7">Syntax</h4>

<pre class="syntaxbox">
 x &lt;= y</pre>

<h4 id="Beispiele_8">Beispiele</h4>

<pre class="brush: js">
3 &lt;= 4 // true
</pre>

<h2 id="Die_Gleichheitsoperatoren_anwenden">Die Gleichheitsoperatoren anwenden</h2>

<p>Die Standard-Gleichheitsoperatoren (<code>==</code>&nbsp;und <code>!=</code>) benutzen den <a href="http://www.ecma-international.org/ecma-262/5.1/#sec-11.9.3">Abstract Equality Comparison Algorithm</a>,&nbsp;um zwei Operanden zu vergleichen. Sind die Operanden unterschiedlichen&nbsp;Typs, wird vor dem Vergleich zuerst versucht&nbsp;sie in gleiche&nbsp;Typen umzuwandeln;&nbsp;z.B. wird&nbsp;beim Ausdruck&nbsp;<code>5 == '5'</code>&nbsp; das Zeichen auf der rechten Seite in eine Zahl konvertiert.</p>

<p>Die strikten Gleichheitsoperatoren&nbsp;(<code>===</code>&nbsp;und <code>!==</code>) benutzen den Strict Equality Comparison Algorithm und sind dafür gedacht, Operanden des gleichen Typs zu vergleichen. &nbsp;Wenn die Operanden von unterschiedlichen&nbsp;Typen sind, ist das&nbsp;Ergebnis immer unwahr (<code>false</code>);&nbsp;somit ist&nbsp;<code>5!=='5'</code>&nbsp;wahr.</p>

<p>Strikte Gleichheitsoperatoren sollten verwendet werden, wenn die Operanden sowohl&nbsp;einen&nbsp;bestimmten Typen als auch&nbsp;Wert haben sollen. Ansonsten benutzt man die nicht-strikten Gleichheitsoperatoren, die es einem erlauben Operanden unterschiedlicher Typen&nbsp;zu vergleichen.</p>

<p>Wenn beim Vergleich eine Typkonvertierung vorgenommen wird&nbsp;(z.B. beim nicht-strikten Vergleich), konvertiert&nbsp;JavaScript die Operanden vom Typ&nbsp;String, Number, Boolean oder&nbsp;Objekt wie folgt:</p>

<ul>
 <li>Wenn eine Zahl und eine Zeichenkette verglichen werden, wird die Zeichenkette zu einem Zahlenwert umgewandelt.&nbsp;JavaScript versucht das numerische&nbsp;Zeichenliteral in einen Wert des Typs&nbsp;<code>Number</code>&nbsp;zu wandeln. Zuerst&nbsp;wird der mathematische&nbsp;Wert des numerischen Zeichenliterals ermittelt. Danach wird der Wert auf den nächsten Wert des Typs&nbsp;<code>Number</code>&nbsp;gerundet.</li>
 <li>Wenn einer der Operanden ein Boolescher Typ ist, wird der Operand zur&nbsp;1 konveriert wenn er <code>wahr</code> ist und zur&nbsp;+0 wenn <code>unwahr</code>.</li>
 <li>Wenn ein Objekt mit einer Zahl oder einer Zeichenkette verglichen wird, &nbsp;versucht&nbsp;JavaScript den Defaultwert für das Objekt zurückzugeben.&nbsp;Operatoren&nbsp;versuchen das Objekt in einen elementaren&nbsp;Wert (<code>String</code> oder&nbsp;<code>Number)</code>&nbsp;umzuwandeln, indem sie die&nbsp;<code>valueOf</code>&nbsp;und <code>toString</code>&nbsp;Methoden der Objekte benutzen. Kann ein Objekt nicht umgewandelt werden, wird ein Laufzeitfehler erzeugt.</li>
 <li>Ein Objekt wird nur dann in einen elementaren Datentypen umgewandelt, wenn sein Vergleichsoperand ein elementarer Datentyp ist. Sind beide Operanden Objekte, werden sie als Objekte verglichen und der Gleichheitstest liefert nur dann wahr, wenn beide auf&nbsp;das&nbsp;gleiche Objekt zeigen.</li>
</ul>

<div class="note"><strong>Hinweis:</strong>&nbsp;Der Type einer Zeichenkette&nbsp;ist <code>Object</code>&nbsp;und nicht <code>String</code>! Zeichenkettenobjekte werden kaum benutzt, daher sind die folgenden Ergebnisse möglicherweise überraschend:</div>

<pre class="brush:js">
// true, da beide Zeichenkettenliterale sind (i.e. string primitives)
'foo' === 'foo'

var a = new String('foo');
var b = new String('foo');

// false, da a und b auf verschiedene Objekte zeigen 
a == b 

// false, da a und b auf verschiedene Objekte zeigen
a === b 

// true, da a und 'foo' verschiedene Typen sind, das Objekt (a) 
// wird vor dem Vergleich zum String 'foo' umgewandelt
a == 'foo' </pre>

<h2 id="Spezifikationen">Spezifikationen</h2>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="col">Spezifikation</th>
   <th scope="col">Status</th>
   <th scope="col">Kommentar</th>
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
   <td>&nbsp;</td>
  </tr>
  <tr>
   <td>{{SpecName('ES6', '#sec-relational-operators', 'Relational Operators')}}<br />
    {{SpecName('ES6', '#sec-equality-operators', 'Equality Operators')}}</td>
   <td>{{Spec2('ES6')}}</td>
   <td>&nbsp;</td>
  </tr>
 </tbody>
</table>

<h2 id="Browserkompatibilität">Browserkompatibilität</h2>

<p>{{CompatibilityTable}}</p>

<div id="compat-desktop">
<table class="compat-table">
 <tbody>
  <tr>
   <th>Merkmal</th>
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
   <th>Merkmal</th>
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

<h2 id="Siehe_auch">Siehe auch</h2>

<ul>
 <li>{{jsxref("Object.is()")}}</li>
 <li><a href="/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness">Equality comparisons and sameness</a></li>
</ul>

