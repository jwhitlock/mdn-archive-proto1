---
version: prototype1
revision_id: 799391
locale: es
slug: Web/JavaScript/Referencia/Operadores
tags: "JavaScript" "Operators"
title: Operadores
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{jsSidebar("Operators")}}</div>

<p>Este capítulo documenta todos los operadores del lenguaje, expresiones y palabras clave.</p>

<h2 id="Expresiones_y_operadores_por_categor.C3.ADa">Expresiones y operadores por categoría</h2>

<p>Para un orden&nbsp;alfabético mira la barra lateral de la izquierda.</p>

<h3 id="Expresiones_primarias">Expresiones primarias</h3>

<p>Palabras clave básicas y expresiones generales en JavaScript.</p>

<dl>
 <dt>{{jsxref("Operadores/this", "this")}}</dt>
 <dd>La palabra reservada&nbsp;<code>this</code>&nbsp;hace referencia al contexto de la función ejecutada.</dd>
 <dt>{{jsxref("Operadores/function", "function")}}</dt>
 <dd>La palabra reservada&nbsp;<code>function</code> define una expresión de función.</dd>
</dl>

<dl>
 <dt>{{experimental_inline}} {{jsxref("Operators/class", "class")}}</dt>
 <dd>La palabra reservada&nbsp;<code>class</code>&nbsp;define una expresión <em>class</em>.</dd>
</dl>

<dl>
 <dt>{{experimental_inline}} {{jsxref("Operators/function*", "function*")}}</dt>
 <dd>La palabra reservada&nbsp;<code>function*</code>&nbsp;define una expresión de función generadora.</dd>
</dl>

<dl>
 <dt>{{experimental_inline}} {{jsxref("Operators/yield", "yield")}}</dt>
 <dd>Pausa&nbsp;y reanuda una función generadora <em>generator</em></dd>
 <dt>{{experimental_inline}} {{jsxref("Operators/yield*", "yield*")}}</dt>
 <dd>Delega a otra función generadora u objeto iterable.</dd>
</dl>

<dl>
 <dt>{{jsxref("Objetos_globales/Array", "[]")}}</dt>
 <dd>Sintaxis de inicialización de un arreglo literal.</dd>
</dl>

<dl>
 <dt><strong style="font-weight:bold">{{jsxref("Objetos_globales/Object", "{}")}}</strong></dt>
 <dd>Sintaxis de inicialización de un objeto literal.</dd>
</dl>

<dl>
 <dt>{{jsxref("Objetos_globales/RegExp", "/ab+c/i")}}</dt>
 <dd>Sintaxis de expresión regular.</dd>
 <dt>{{experimental_inline()}} {{jsxref("Operators/Array_comprehensions", "[for (x of y) x]")}}</dt>
 <dd>Comprensiones de Array.</dd>
 <dt>{{experimental_inline()}} {{jsxref("Operators/Generator_comprehensions", "(for (x of y) y)")}}</dt>
 <dd>Generador de comprensiones.</dd>
 <dt>{{jsxref("Operadores/Grouping", "( )")}}</dt>
 <dd>Operador de agrupación.</dd>
</dl>

<h3 id="Expresiones_al_lado_izquierdo">Expresiones al lado izquierdo</h3>

<p>Los valores al lado izquierdo son el&nbsp;destino de una asignación.</p>

<dl>
 <dt>{{jsxref("Operadores/Property_accessors", "Property accessors", "", 1)}}</dt>
 <dd>Operaciones miembro que proveen acceso a una propiedad o método de un objeto<br />
 (<code>object.property</code> and <code>object["property"]</code>).</dd>
 <dt>{{jsxref("Operadores/new", "new")}}</dt>
 <dd>El operador&nbsp;<code>new</code>&nbsp;crea una instancia de un constructor.</dd>
 <dt>{{experimental_inline()}} {{jsxref("Operadores/super", "super")}}</dt>
 <dd>La palabra reservada&nbsp;<code>super</code> llama al constructor padre.</dd>
 <dt>{{experimental_inline()}} {{jsxref("Operadores/Spread_operator", "...obj")}}</dt>
 <dd>El operador de propagación&nbsp;<em><strong>spread operator</strong></em>&nbsp;permite que una expresión sea expandida&nbsp;en situaciones&nbsp;donde múltiples argumentos (llamadas a funciones) o múltiples elementos (arreglos literales) son esperados.</dd>
</dl>

<h3 id="Incremento_y_decremento">Incremento y decremento</h3>

<p>Operadores Sufijo/prefijo de incremento y Sufijo/prefijo de decremento.</p>

<dl>
 <dt>{{jsxref("Operadores/Aritm%C3%A9ticos", "A++", "#Increment")}}</dt>
 <dd>Sufijo del operador de incremento.</dd>
 <dt>{{jsxref("Operadores/Aritm%C3%A9ticos", "A--", "#Decrement")}}</dt>
 <dd>Sufijo del operador de decremento.</dd>
 <dt>{{jsxref("Operadores/Aritm%C3%A9ticos", "++A", "#Increment")}}</dt>
 <dd>Prefijo del operador de incremento.</dd>
 <dt>{{jsxref("Operadores/Aritm%C3%A9ticos", "--A", "#Decrement")}}</dt>
 <dd>Prefijo del operador de decremento.</dd>
</dl>

<h3 id="Operadores_Unarios">Operadores Unarios</h3>

<p>Una operación unaria es una operación con un único operando.</p>

<dl>
 <dt>{{jsxref("Operadores/delete", "delete")}}</dt>
 <dd>El operador&nbsp;<code>delete</code> elimina una propiedad de un objeto.</dd>
 <dt>{{jsxref("Operadores/void", "void")}}</dt>
 <dd>El operador&nbsp;<code>void</code> descarta el valor de retorno de una expresión.</dd>
 <dt>{{jsxref("Operadores/typeof", "typeof")}}</dt>
 <dd>El operador&nbsp;<code>typeof</code> determina el tipo de un objeto dado.</dd>
 <dt>{{jsxref("Operadores/Aritm%C3%A9ticos", "+", "#Unary_plus")}}</dt>
 <dd>El operador&nbsp;unario positivo&nbsp;convierte su operando an un tipo numérico <em>Number</em></dd>
 <dt>{{jsxref("Operadores/Aritm%C3%A9ticos", "-", "#Unary_negation")}}</dt>
 <dd>El operador unario de negación&nbsp;convierte su operando a un tipo numérico <em>Number</em> y luego lo niega, es decir si es positivo lo vuelve negativo y viceversa.</dd>
 <dt>{{jsxref("Operadores/Aritm%C3%A9ticos", "~", "#Bitwise_NOT")}}</dt>
 <dd>Operador NOT en modo bit.</dd>
 <dt>{{jsxref("Operadores/Aritm%C3%A9ticos", "!", "#Logical_NOT")}}</dt>
 <dd>Operador lógico&nbsp;NOT.</dd>
</dl>

<h3 id="Operadores_aritm.C3.A9ticos">Operadores aritméticos</h3>

<p>Los operadores aritméticos toman valores numéricos (ya sean literales o variables) como sus operandos y retornan un único valor numérico.</p>

<dl>
 <dt>{{jsxref("Operadores/Aritm%C3%A9ticos", "+", "#Addition")}}</dt>
 <dd>Operador de adición o suma.</dd>
 <dt>{{jsxref("Operadores/Aritm%C3%A9ticos", "-", "#Subtraction")}}</dt>
 <dd>Operador de substracción o resta.</dd>
 <dt>{{jsxref("Operadores/Aritm%C3%A9ticos", "/", "#Division")}}</dt>
 <dd>Operador de división.</dd>
 <dt>{{jsxref("Operadores/Aritm%C3%A9ticos", "*", "#Multiplication")}}</dt>
 <dd>Operador de multiplicación.</dd>
 <dt>{{jsxref("Operadores/Aritm%C3%A9ticos", "%", "#Remainder")}}</dt>
 <dd>Operador de residuo.</dd>
</dl>

<h3 id="Operadores_relacionales">Operadores relacionales</h3>

<p>Un operador de comparación, compara sus operandos y retorna un valor boleano basado en determinar&nbsp;si la comparación es verdadera o no.</p>

<dl>
 <dt>{{jsxref("Operadores/in", "in")}}</dt>
 <dd>El operador&nbsp;<code>in</code> determina si un objeto tiene una propiedad dada.</dd>
 <dt>{{jsxref("Operadores/instanceof", "instanceof")}}</dt>
 <dd>El operador&nbsp;<code>instanceof</code> determina si un objeto es una instancia de otro objeto, es decir si fué creado con una función constructora determinada.</dd>
 <dt>{{jsxref("Operadores/Comparison_Operators", "&lt;", "#Less_than_operator")}}</dt>
 <dd>Operador <em>menor que</em>.</dd>
 <dt>{{jsxref("Operadores/Comparison_Operators", "&gt;", "#Greater_than_operator")}}</dt>
 <dd>Operador <em>mayor que.</em></dd>
 <dt>{{jsxref("Operadores/Comparison_Operators", "&lt;=", "#Less_than_or_equal_operator")}}</dt>
 <dd>Operador <em>menor o igual a</em></dd>
 <dt>{{jsxref("Operadores/Comparison_Operators", "&gt;=", "#Greater_than_or_equal_operator")}}</dt>
 <dd>Operador <em>mayor o igual a</em></dd>
</dl>

<h3 id="Operadores_de_igualdad">Operadores de igualdad</h3>

<p>El resultado de evaluar un operador de igualdad es siempre de tipo boleano y se basa en&nbsp;determinar cuando la comparación es verdadera.</p>

<dl>
 <dt>{{jsxref("Operadores/Comparison_Operators", "==", "#Equality")}}</dt>
 <dd>Operador de igualdad.</dd>
 <dt>{{jsxref("Operadores/Comparison_Operators", "!=", "#Inequality")}}</dt>
 <dd>Operador de desigualdad.</dd>
 <dt>{{jsxref("Operadores/Comparison_Operators", "===", "#Identity")}}</dt>
 <dd>Operador de igualdad estricto.</dd>
 <dt>{{jsxref("Operadores/Comparison_Operators", "!==", "#Nonidentity")}}</dt>
 <dd>Operador de desigualdad estricta.</dd>
</dl>

<h3 id="Operadores_de_desplazamiento_de_bits">Operadores de desplazamiento de bits</h3>

<p>Operaciones para desplazar todos los bits del operando.</p>

<dl>
 <dt>{{jsxref("Operadores/Bitwise_Operators", "&lt;&lt;", "#Left_shift")}}</dt>
 <dd>Operador de desplazamiento a la izquierda en modo bit.</dd>
 <dt>{{jsxref("Operadores/Bitwise_Operators", "&gt;&gt;", "#Right_shift")}}</dt>
 <dd>Operador de&nbsp;desplazamiento a la derecha en modo bit.</dd>
 <dt>{{jsxref("Operadores/Bitwise_Operators", "&gt;&gt;&gt;", "#Unsigned_right_shift")}}</dt>
 <dd>Operador de desplazamiento a la derecha en modo bit sin signo.</dd>
</dl>

<h3 id="Operadores_binarios_en_modo_bit">Operadores binarios en modo bit</h3>

<p>Los operators de modo bit&nbsp;tratan sus operandos como un set de 32 bits (ceros y unos) y retornan valores numéricos estandar de Javascript.</p>

<dl>
 <dt>{{jsxref("Operadores/Bitwise_Operators", "&amp;", "#Bitwise_AND")}}</dt>
 <dd>AND en modo bit.</dd>
 <dt>{{jsxref("Operadores/Bitwise_Operators", "|", "#Bitwise_OR")}}</dt>
 <dd>OR en modo bit.</dd>
 <dt>{{jsxref("Operadores/Bitwise_Operators", "^", "#Bitwise_XOR")}}</dt>
 <dd>XOR en modo bit.</dd>
</dl>

<h3 id="Operadores_l.C3.B3gicos_binarios">Operadores lógicos binarios</h3>

<p>Los operadores lógicos son tipicamente usados con valores boleanos (lógicos), y cuando es así, estos operadores retornan igualmente un valor boleano.</p>

<dl>
 <dt>{{jsxref("Operadores/Logical_Operators", "&amp;&amp;", "#Logical_AND")}}</dt>
 <dd>AND lógico.</dd>
 <dt>{{jsxref("Operadores/Logical_Operators", "||", "#Logical_OR")}}</dt>
 <dd>OR lógico.</dd>
</dl>

<h3 id="Operador_condicional_(ternario)">Operador condicional (ternario)</h3>

<dl>
 <dt>{{jsxref("Operadores/Conditional_Operator", "(condition ? ifTrue : ifFalse)")}}</dt>
 <dd>
 <p>El operador condicional retorna el segundo o el tercer operando, basado en el valor lógico&nbsp;del primero.</p>
 </dd>
</dl>

<h3 id="Operadores_de_asignaci.C3.B3n">Operadores de asignación</h3>

<p>Un operador de asignación, asigna un valor al operando de la izquierda basado en el valor del operando de la derecha.</p>

<dl>
 <dt>{{jsxref("Operadores/Assignment_Operators", "=", "#Assignment")}}</dt>
 <dd>Operador de asignación.</dd>
 <dt>{{jsxref("Operadores/Assignment_Operators", "*=", "#Multiplication_assignment")}}</dt>
 <dd>Operador de asignación de multiplication.</dd>
 <dt>{{jsxref("Operadores/Assignment_Operators", "/=", "#Division_assignment")}}</dt>
 <dd>Operador de asignación de división.</dd>
 <dt>{{jsxref("Operadores/Assignment_Operators", "%=", "#Remainder_assignment")}}</dt>
 <dd>Operador de asignación de residuo.</dd>
 <dt>{{jsxref("Operadores/Assignment_Operators", "+=", "#Addition_assignment")}}</dt>
 <dd>Operador de asignación de suma.</dd>
 <dt>{{jsxref("Operadores/Assignment_Operators", "-=", "#Subtraction_assignment")}}</dt>
 <dd>Subtraction assignment</dd>
 <dt>{{jsxref("Operadores/Assignment_Operators", "&lt;&lt;=", "#Left_shift_assignment")}}</dt>
 <dd>Operador de asignación y desplazamiento a la izquierda en modo bit.</dd>
 <dt>{{jsxref("Operadores/Assignment_Operators", "&gt;&gt;=", "#Right_shift_assignment")}}</dt>
 <dd>Operador de asignación y desplazamiento a la derecha en modo bit.</dd>
 <dt>{{jsxref("Operadores/Assignment_Operators", "&gt;&gt;&gt;=", "#Unsigned_right_shift_assignment")}}</dt>
 <dd>Operador de asignación y desplazamiento a la derecha en modo bit sin signo.</dd>
 <dt>{{jsxref("Operadores/Assignment_Operators", "&amp;=", "#Bitwise_AND_assignment")}}</dt>
 <dd>Operador de asignación de AND en modo bit.</dd>
 <dt>{{jsxref("Operadores/Assignment_Operators", "^=", "#Bitwise_XOR_assignment")}}</dt>
 <dd>Asignación de XOR en modo bit.</dd>
 <dt>{{jsxref("Operadores/Assignment_Operators", "|=", "#Bitwise_OR_assignment")}}</dt>
 <dd>asignación de OR en modo bit.</dd>
 <dt>{{experimental_inline()}} {{jsxref("Operadores/Destructuring_assignment", "[a, b] = [1, 2]")}}<br />
 {{experimental_inline()}} {{jsxref("Operadores/Destructuring_assignment", "{a, b} = {a:1, b:2}")}}</dt>
 <dd>
 <p>La sintaxis de asignación desestructurada es una expresión que permite extraer datos&nbsp;de un arreglo u objeto usando&nbsp;una sintaxis similar a la usada en&nbsp;arreglos literales y&nbsp;objetos literales.</p>
 </dd>
</dl>

<h3 id="Operador_de_coma">Operador de coma</h3>

<dl>
 <dt>{{jsxref("Operadores/Comma_Operator", ",")}}</dt>
 <dd>
 <p>El operador de coma permite que multiples expresiones sean evaluadas en una misma declaración&nbsp;y retorna el valor de la última exrpresión.</p>
 </dd>
</dl>

<h2 id="Especificaciones">Especificaciones</h2>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="col">Especificación</th>
   <th scope="col">Estatus</th>
   <th scope="col">Comentario</th>
  </tr>
  <tr>
   <td>ECMAScript 1st Edition.</td>
   <td>Estándar</td>
   <td>Definición inicial.</td>
  </tr>
  <tr>
   <td>{{SpecName('ES5.1', '#sec-11', 'Expressions')}}</td>
   <td>{{Spec2('ES5.1')}}</td>
   <td>&nbsp;</td>
  </tr>
  <tr>
   <td>{{SpecName('ES6', '#sec-ecmascript-language-expressions', 'ECMAScript Language: Expressions')}}</td>
   <td>{{Spec2('ES6')}}</td>
   <td>Nuevo: operador de propagación <strong><em>spread operator</em></strong>, asignación desestructurada <strong><em>destructuring assignment</em></strong>, palabra reservada&nbsp;<strong><code>super</code></strong>, comprensiones de arreglos <strong><em>Array comprehensions</em></strong>, Comprensiones generadoras <strong><em>Generator comprehensions</em></strong></td>
  </tr>
 </tbody>
</table>

<h2 id="Temas_relacionados">Temas relacionados</h2>

<ul>
 <li><a href="/en-US/docs/Web/JavaScript/Reference/Operators/Operator_Precedence">Precedencia de operadores</a></li>
</ul>

