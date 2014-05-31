---
version: prototype1
revision_id: 608241
locale: pl
slug: Web/JavaScript/Dokumentacja_języka_JavaScript_1.5/Operatory/Operatory_porównania
tags: "Operator" "JavaScript"
title: Operatory porównania
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>
{{ Dopracuj() }}
</p>
<h3 name="Podsumowanie"> Podsumowanie </h3>
<table class="fullwidth-table">
<tbody><tr>
<td class="header" colspan="2">Operatory</td>
</tr>
<tr>
<td>Zaimplementowano w:</td>
<td>JavaScript 1.0
<p>JavaScript 1.3: Dodano operatory <code>===</code> i <code>!==</code>.
</p><p>JavaScript 1.4: Wycofano <code>==</code> porównanie dla dwóch obiektów <code>JSObject</code>. Zastosowano metodę <code>JSObject.equals</code>.
</p>
</td>
</tr>
<tr>
<td>Wersje ECMA:</td>
<td>ECMA-262 zawiera wszystkie operatory porównania oprócz <code>===</code> i <code>!==</code>.
<p>ECMA-262 edycja 3 dodano <code>===</code> i <code>!==</code>.
</p>
</td>
</tr>
</tbody></table>
<p>Operandy posiadają wartość liczbową lub łańcucha znaków. Łańcuchy znaków są porównywane w oparciu o zasady pisowni, używają wartości Unicode. </p><p>Jako rezultat porównania zwracana jest wartość logiczna.
</p>
<ul><li> Dwa łańcuchy są równe kiedy kiedy posiadają taką sama sekwencję znaków, taką samą długość, i takie same znaki w zgodnych pozycjach.
</li><li> Dwie liczby są równe kiedy ich wartości liczbowe (posiadają liczbę o takiej samej wartości). NaN jest różne dla wszystkich, włączając NaN. Dodatnie i ujemne zera są równe.
</li><li> Dwa obiekty są równe jeżeli odnoszą się do tego samego obiektu .
</li><li> Dwa operandy Boolean są równe jeżeli oba zwracają <code>true</code> lub <code>false</code>.
</li><li> Null and Undefined types are <code>==</code> (lecz nie <code>===</code>).
</li></ul>
<p>Następująca tabela opisuje operatory porównania:
</p>
<table class="fullwidth-table">
<tbody><tr>
<th>Operator</th>
<th>Opis</th>
<th>Przykłady zwracające prawdę (true)<sup>1</sup></th>
</tr>
<tr>
<td>Równy (<code>==</code>)</td>
<td>Zwraca true jeżeli operandy są równe. Jeżeli operandy nie są tego samego typu, JavaScript próbuje przekształcić operandy na odpowiedni dla porównania typ.</td>
<td>
<p><code>3 == var1<br>
"3" == var1<br>
3 == '3'<br></code>
</p>
</td>
</tr>
<tr>
<td>Różny (<code>!=</code>)</td>
<td>Zwraca true jeżeli operandy są różne. Jeżeli dwa operandy nie są tego samego typu, JavaScript próbuje przekształcić operandy na odpowiedni dla porównania typ.</td>
<td>
<p><code>var1 != 4<br>
var1 != "3"</code>
</p>
</td>
</tr>
<tr>
<td>Identyczny (<code>===</code>)</td>
<td>Zwraca true jeżeli operandy są równe i tego samego typu.</td>
<td>
<p><code>3 === var1</code>
</p>
</td>
</tr>
<tr>
<td>Nieidentyczny (<code>!==</code>)</td>
<td>Zwraca true jeżeli operandy nie są równe i/lub nie są tego samego typu.</td>
<td>
<p><code>var1 !== 3<br>
3 !== '3'</code>
</p>
</td>
</tr>
<tr>
<td>Większy niż (<code>&gt;</code>)</td>
<td>Zwraca true jeżeli lewy operand jest większy od prawego operandu.</td>
<td>
<p><code>var2 &gt; var1</code>
</p>
</td>
</tr>
<tr>
<td>Większy - równy (<code>&gt;=</code>)</td>
<td>Zwraca true jeżeli lewy operand jest większy lub równy prawemu operandowi.</td>
<td>
<p><code>var2 &gt;= var1<br>
var1 &gt;= 3</code>
</p>
</td>
</tr>
<tr>
<td>Mniejszy niż (<code>&lt;</code>)</td>
<td>Zwraca true, jeśli lewy operand jest mniejszy, niż prawy. </td>
<td>
<p><code>var1 &lt; var2</code>
</p>
</td>
</tr>
<tr>
<td>Mniejszy - równy (<code>&lt;=</code>)</td>
<td>Zwraca true jeżeli lewy operand jest mniejszy lub równy prawemu operandowi.</td>
<td>
<p><code>var1 &lt;= var2<br>
var2 &lt;= 5</code>
</p>
</td>
</tr>
</tbody></table>
<p><small><sup>1</sup> Te przykłady zakładają, że <code>var1</code> będzie przydzielona wartość 3 i <code>var2</code> będzie miała przydzieloną wartość 4.</small>
</p>
<h3 name="U.C5.BCywanie_operator.C3.B3w_por.C3.B3wnania"> Używanie operatorów porównania </h3>
<p>Standardowe operatory(<code>==</code> i <code>!=</code>) porównują dwa operandy bez względu na ich typ. Operatory porównania identyczności(<code>===</code> i <code>!==</code>) dokonują porównania równości na operandach tego samego typu. Operatorów identyczności używamy jeżeli operandy muszą być określonego typu jak również wartości lub jeśli dokładny typ operandów jest ważny. W przeciwnym razie, używamy standardowych operatorów porównania, które pozwalają na porównać identyczność dwóch operandów nawet jeżeli nie są takiego samego typu.
</p><p>Kiedy potrzebna jest konwersja, JavaScript następująco przekształca operand Number, Boolean lub Object.
</p>
<ul><li> Kiedy porównujemy liczbę i łańcuch, łańcuch jest zmieniany na wartość liczbową. JavaScript próbuje przekształcić łańcuch literalny cyfr na wartość typu <code>Number</code>. Najpierw, matematyczna wartość jest wyprowadzana z łańcucha cyfrowego literału. Następnie, ta wartość jest zaokrąglana do najbliższej wartości typu <code>Number</code>.
</li><li> If one of the operands is <code>Boolean</code>, the Boolean operand is converted to 1 if it is <code>true</code> and +0 if it is <code>false</code>.
</li><li> If an object is compared with a number or string, JavaScript attempts to return the default value for the object. Operators attempt to convert the object to a primitive value, a <code>String</code> or <code>Number</code> value, using the <code>valueOf</code> and <code>toString</code> methods of the objects. If this attempt to convert the object fails, a runtime error is generated.
</li></ul>
<p>You cannot use the standard equality operator (<code>==</code>) to compare instances of <code>JSObject</code>. Use the <code>JSObject.equals</code> method for such comparisons.
</p>
<h3 name="Kompatybilno.C5.9B.C4.87_wsteczna"> Kompatybilność wsteczna </h3>
<p>Zachowanie standardowych operatorów porównania (<code>==</code> i <code>!=</code>) zależy od wersji JavaScript.
</p>
<h4 name="JavaScript_1.3_i_wersje_wcze.C5.9Bniejsze"> JavaScript 1.3 i wersje wcześniejsze </h4>
<p>You can use either the standard equality operator (<code>==</code>) or <code>JSObject.equals</code> to compare instances of <code>JSObject</code>.
</p>
<h4 name="JavaScript_1.2"> JavaScript 1.2 </h4>
<p>The standard equality operators (<code>==</code> and <code>!=</code>) do not perform a type conversion before the comparison is made. Operatory identyczności (<code>===</code> i <code>!==</code>) są niedostępne.
</p>
<h4 name="JavaScript_1.1_i_wersje_wcze.C5.9Bniejsze"> JavaScript 1.1 i wersje wcześniejsze </h4>
<p>The standard equality operators (<code>==</code> and <code>!=</code>) perform a type conversion before the comparison is made.Operatory identyczności (<code>===</code> i <code>!==</code>) są niedostępne.
</p>{{ languages( { "en": "en/Core_JavaScript_1.5_Reference/Operators/Comparison_Operators", "fr": "fr/R\u00e9f\u00e9rence_de_JavaScript_1.5_Core/Op\u00e9rateurs/Op\u00e9rateurs_de_comparaison" } ) }}

