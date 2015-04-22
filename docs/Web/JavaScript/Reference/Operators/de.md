---
version: prototype1
revision_id: 790304
locale: de
slug: Web/JavaScript/Reference/Operators
tags: "JavaScript" "Operators"
title: Ausdrücke und Operatoren
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{jsSidebar("Operators")}}</div>

<p>Dieses Kapitel behandelt alle JavaScript-Sprachoperatoren, Ausdrücke und Schlüsselwörter.</p>

<h2 id="Ausdr.C3.BCcke_und_Operatoren_geordnet_nach_Kategorie">Ausdrücke und Operatoren geordnet nach Kategorie</h2>

<p>Die alphabetische Sortierung finden Sie in der linken Seitenspalte.</p>

<h3 id="Grundlegende_Ausdr.C3.BCcke">Grundlegende Ausdrücke</h3>

<p>Elementare Schlüsselwörter und allgemeine Ausdrücke in JavaScript.</p>

<dl>
 <dt>{{jsxref("Operators/this", "this")}}</dt>
 <dd>Das&nbsp;<code>this</code>&nbsp;Schlüsselwort bezieht sich auf den Ausführungskontext einer Funktion.</dd>
 <dt>{{jsxref("Operators/function", "function")}}</dt>
 <dd>Der&nbsp;<code>function</code>&nbsp;Schlüsselbegriff definiert einen Funktionsausdruck.</dd>
 <dt>{{jsxref("Global_Objects/Array", "[]")}}</dt>
 <dd>Array-Initialisierungs- bzw. Literal-Syntax.</dd>
 <dt>{{jsxref("Operators/Object_initializer", "{}")}}</dt>
 <dd>Objekt-Initialisierungs- bzw. Literal-Syntax.</dd>
 <dt>{{jsxref("Global_Objects/RegExp", "/ab+c/i")}}</dt>
 <dd>Literal-Syntax für reguläre Ausdrücke.</dd>
 <dt>{{experimental_inline()}} {{jsxref("Operators/Array_comprehensions", "[for (x of y) x]")}}</dt>
 <dd>Array Comprehensions.</dd>
 <dt>{{experimental_inline()}} {{jsxref("Operators/Generator_comprehensions", "(for (x of y) y)")}}</dt>
 <dd>Generator Comprehensions.</dd>
 <dt>{{jsxref("Operators/Grouping", "( )")}}</dt>
 <dd>Gruppierungs-Operator.</dd>
</dl>

<h3 id="Linke-Seite-Ausdr.C3.BCcke">Linke-Seite-Ausdrücke</h3>

<p>Werte auf der linken Seite sind das Ziel einer Zuweisung.</p>

<dl>
 <dt>{{jsxref("Operators/Property_accessors", "Property accessors", "", 1)}}</dt>
 <dd>Member-Operatoren ermöglichen den Zugriff auf eine Objektvariable oder eine Methode eines Objekts.<br />
 (<code>object.property</code> and <code>object["property"]</code>).</dd>
 <dt>{{jsxref("Operators/new", "new")}}</dt>
 <dd>Der&nbsp;<code>new</code>&nbsp;Operator erzeugt eine Instanz über einen Konstruktor.</dd>
 <dt>{{experimental_inline()}} {{jsxref("Operators/super", "super")}}</dt>
 <dd>Das&nbsp;<code>super</code>&nbsp;Schlüsselwort ruft den Eltern-Konstruktur auf.</dd>
 <dt>{{experimental_inline()}} {{jsxref("Operators/Spread_operator", "...obj")}}</dt>
 <dd>Der Spread-Operator ermöglicht es einem Ausdruck in Situationen erweitert zu werden, &nbsp;wo mehrfache Argumente (für Funktionsaufrufe) oder mehrfache Elemente (für Array-Literale) erwartet werden.</dd>
</dl>

<h3 id="Inkrement_und_Dekrement">Inkrement und Dekrement</h3>

<p>Postfix/Prefix-Inkrement- und Postfix/Prefix-Dekrement-Operatoren.</p>

<dl>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "A++", "#Increment")}}</dt>
 <dd>Postfix-Inkrement-Operator.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "A--", "#Decrement")}}</dt>
 <dd>Postfix-Dekrement-Operator.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "++A", "#Increment")}}</dt>
 <dd>Prefix-Inkrement-Operator.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "--A", "#Decrement")}}</dt>
 <dd>Prefix-Dekrement-Operator.</dd>
</dl>

<h3 id="Un.C3.A4re_Operatoren">Unäre Operatoren</h3>

<p>Ein unärer Vorgang (Operation/Programmablauf) ist ein Vorgang mit nur einem Operand.</p>

<dl>
 <dt>{{jsxref("Operators/delete", "delete")}}</dt>
 <dd>Der&nbsp;<code>delete</code>&nbsp;Operator entfernt eine Objektvariable aus einem Objekt.</dd>
 <dt>{{jsxref("Operators/void", "void")}}</dt>
 <dd>Der&nbsp;<code>void</code>&nbsp;Operator verwirft den Rückgabewert eines Ausdrucks.</dd>
 <dt>{{jsxref("Operators/typeof", "typeof")}}</dt>
 <dd>Der&nbsp;<code>typeof</code>&nbsp;Operator ermittelt den Typ des angegebenen Objekts.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "+", "#Unary_plus")}}</dt>
 <dd>Der unäre Plus-Operator wandelt seinen Operand in einen Number-Typ um.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "-", "#Unary_negation")}}</dt>
 <dd>Der unäre Negations-Operator wandelt seinen Operand in einen NumberTyp um und negiert ihn.</dd>
 <dt>{{jsxref("Operators/Bitwise_Operators", "~", "#Bitwise_NOT")}}</dt>
 <dd>Bitwise NOT Operator.</dd>
 <dt>{{jsxref("Operators/Logical_Operators", "!", "#Logical_NOT")}}</dt>
 <dd>Logischer NOT Operator.</dd>
</dl>

<h3 id="Arithmetische_Operatoren">Arithmetische Operatoren</h3>

<p>Arithmetische Operatoren nehmen numerische Werte (entwender Literale oder Variablen) als ihre Operanden und geben genau einen numerischen Wert zurück.</p>

<dl>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "+", "#Addition")}}</dt>
 <dd>Additions-Operator.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "-", "#Subtraction")}}</dt>
 <dd>Subtraktions-Operator.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "/", "#Division")}}</dt>
 <dd>Divisions-Operator.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "*", "#Multiplication")}}</dt>
 <dd>Multiplikations-Operator.</dd>
 <dt>{{jsxref("Operators/Arithmetic_Operators", "%", "#Remainder")}}</dt>
 <dd>Rest (Remainder)-Operator.</dd>
</dl>

<h3 id="Vergleichsoperatoren">Vergleichsoperatoren</h3>

<p>Ein Vergleichsoperator vergleicht seine Operanden und gibt einen <code>Booleschen</code>&nbsp;Wert zurück, basierend darauf, ob der Wahrheitswert des Vergleichs <code>wahr</code> (true) ist.</p>

<dl>
 <dt>{{jsxref("Operators/in", "in")}}</dt>
 <dd>Der&nbsp;<code>in</code>&nbsp;Operator ermittelt ob ein Objekt die gegebene Objektvariable enthält.</dd>
 <dt>{{jsxref("Operators/instanceof", "instanceof")}}</dt>
 <dd>Der&nbsp;<code>instanceof</code>&nbsp;Operator ermittelt ob ein Objekt eine Instanz eines anderen Objekts ist.</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "&lt;", "#Less_than_operator")}}</dt>
 <dd>Kleiner-als-Operator.</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "&gt;", "#Greater_than_operator")}}</dt>
 <dd>Größer-als-Operator.</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "&lt;=", "#Less_than_or_equal_operator")}}</dt>
 <dd>"Kleiner als oder gleich" - Operator.</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "&gt;=", "#Greater_than_or_equal_operator")}}</dt>
 <dd>"Größer als oder gleich" - Operator.</dd>
</dl>

<h3 id="Gleichheit-Operatoren">Gleichheit-Operatoren</h3>

<p>Das Ergebnis der Auswertung eines Gleichheit-Operators ist immer vom Typ <code>Boolean</code>,&nbsp;<span style="line-height: 1.5;">&nbsp;basierend darauf, ob der Wahrheitswert des Vergleichs&nbsp;</span><code style="font-style: normal; line-height: 1.5;">wahr</code><span style="line-height: 1.5;">&nbsp;(true) ist.</span></p>

<dl>
 <dt>{{jsxref("Operators/Comparison_Operators", "==", "#Equality")}}</dt>
 <dd>Gleichheit-Operator.</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "!=", "#Inequality")}}</dt>
 <dd>Ungleichheit-Operator.</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "===", "#Identity")}}</dt>
 <dd>Identitäts-Operator.</dd>
 <dt>{{jsxref("Operators/Comparison_Operators", "!==", "#Nonidentity")}}</dt>
 <dd>Nonidentity operator.</dd>
</dl>

<h3 id="Bitweise-Verschieben-Operatoren">Bitweise-Verschieben-Operatoren</h3>

<p>Programmschritte, die alle Bits eines Operanden verschieben.</p>

<dl>
 <dt>{{jsxref("Operators/Bitwise_Operators", "&lt;&lt;", "#Left_shift")}}</dt>
 <dd>Operator für bitweises Verschieben nach links.</dd>
 <dt>{{jsxref("Operators/Bitwise_Operators", "&gt;&gt;", "#Right_shift")}}</dt>
 <dd>Operator für bitweises Verschieben nach rechts.</dd>
 <dt>{{jsxref("Operators/Bitwise_Operators", "&gt;&gt;&gt;", "#Unsigned_right_shift")}}</dt>
 <dd>Operator für vorzeichenloses (unsigned) bitweises Verschieben nach rechts.</dd>
</dl>

<h3 id="Bin.C3.A4re_bitweise_Operatoren">Binäre bitweise Operatoren</h3>

<p>Bitweise Operatoren behandeln ihre Operanden als eine Menge von 32 Bits (Nullen und Einsen) und geben die in JavaScript&nbsp;üblichen numerischen Werte zurück.</p>

<dl>
 <dt>{{jsxref("Operators/Bitwise_Operators", "&amp;", "#Bitwise_AND")}}</dt>
 <dd>Bitweises UND (AND).</dd>
 <dt>{{jsxref("Operators/Bitwise_Operators", "|", "#Bitwise_OR")}}</dt>
 <dd>Bitweises ODER (OR).</dd>
 <dt>{{jsxref("Operators/Bitwise_Operators", "^", "#Bitwise_XOR")}}</dt>
 <dd>Bitweises ENTWEDER-ODER (XOR).</dd>
</dl>

<h3 id="Bin.C3.A4re_logische_Operatoren">Binäre logische Operatoren</h3>

<p>Logische Operatoren werden normalerweise mit Booleschen (logischen) Werten benutzt und sie liefern dann einen Booleschen Wert zurück.</p>

<dl>
 <dt>{{jsxref("Operators/Logical_Operators", "&amp;&amp;", "#Logical_AND")}}</dt>
 <dd>Logisches UND (AND).</dd>
 <dt>{{jsxref("Operators/Logical_Operators", "||", "#Logical_OR")}}</dt>
 <dd>Logisches ODER (OR).</dd>
</dl>

<h3 id="Bedingter_(tern.C3.A4rer)_Operator">Bedingter (ternärer) Operator</h3>

<dl>
 <dt>{{jsxref("Operators/Conditional_Operator", "(condition ? ifTrue : ifFalse)")}}</dt>
 <dd>
 <p>Der bedingte Operator liefert einen von zwei Werten zurück, in Abhängigkeit des logischen Wertes der Bedingung.</p>
 </dd>
</dl>

<h3 id="Zuweisungsoperator">Zuweisungsoperator</h3>

<p>Der Zuweisungsoperator weist seinem linken Operand einen Wert zu, in Abhängigkeit des Wertes seines rechten Operands.</p>

<dl>
 <dt>{{jsxref("Operators/Assignment_Operators", "=", "#Assignment")}}</dt>
 <dd>Zuweisungsoperator.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "*=", "#Multiplication_assignment")}}</dt>
 <dd>Multiplikationszuweisung.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "/=", "#Division_assignment")}}</dt>
 <dd>Teilungszuweisung.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "%=", "#Remainder_assignment")}}</dt>
 <dd>Restzuweisung.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "+=", "#Addition_assignment")}}</dt>
 <dd>Additionszuweisung.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "-=", "#Subtraction_assignment")}}</dt>
 <dd>Subtraktionszuweisung.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "&lt;&lt;=", "#Left_shift_assignment")}}</dt>
 <dd>Links-verschieben-Zuweisung.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "&gt;&gt;=", "#Right_shift_assignment")}}</dt>
 <dd>Rechts-verschieben-Zuweisung.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "&gt;&gt;&gt;=", "#Unsigned_right_shift_assignment")}}</dt>
 <dd>Vorzeichenlose (unsigned) Rechts-verschieben-Zuweisung.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "&amp;=", "#Bitwise_AND_assignment")}}</dt>
 <dd>Bitweise UND-Zuweisung.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "^=", "#Bitwise_XOR_assignment")}}</dt>
 <dd>Bitweise ENTWEDER-ODER-Zuweisung.</dd>
 <dt>{{jsxref("Operators/Assignment_Operators", "|=", "#Bitwise_OR_assignment")}}</dt>
 <dd>Bitweise ODER-Zuweisung.</dd>
 <dt>{{experimental_inline()}} {{jsxref("Operators/Destructuring_assignment", "[a, b] = [1, 2]")}}<br />
 {{experimental_inline()}} {{jsxref("Operators/Destructuring_assignment", "{a, b} = {a:1, b:2}")}}</dt>
 <dd>
 <p>Destructuring Assignment (etwa: "Umstrukturierungs-Zuweisung) ermöglicht das Zuweisen von Daten aus Arrays oder Objekten an Variablen, mit einer ähnlichen Syntax wie bei Array- oder Objekt-Literalen.</p>
 </dd>
</dl>

<h3 id="Komma-Operator">Komma-Operator</h3>

<dl>
 <dt>{{jsxref("Operators/Comma_Operator", ",")}}</dt>
 <dd>
 <p>Der Komma-Operator erlaubt es mehrere Ausdrücke innerhalb eines einzigen Ausdrucks zu evaluieren und liefert das Ergebnis des letzten Ausdrucks.</p>
 </dd>
</dl>

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
   <td>Initiale Definition.</td>
  </tr>
  <tr>
   <td>{{SpecName('ES5.1', '#sec-11', 'Expressions')}}</td>
   <td>{{Spec2('ES5.1')}}</td>
   <td>&nbsp;</td>
  </tr>
  <tr>
   <td>{{SpecName('ES6', '#sec-ecmascript-language-expressions', 'ECMAScript Language: Expressions')}}</td>
   <td>{{Spec2('ES6')}}</td>
   <td>Neu: Spread-Operator, destructuring assignment, <code>super</code> keyword, Array comprehensions, Generator comprehensions</td>
  </tr>
 </tbody>
</table>

<h2 id="Siehe_auch">Siehe auch</h2>

<ul>
 <li><a href="/en-US/docs/Web/JavaScript/Reference/Operators/Operator_Precedence">Operator-Rangfolge</a></li>
</ul>

