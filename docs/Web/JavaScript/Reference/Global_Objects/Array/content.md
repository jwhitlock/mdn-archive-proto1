---
version: prototype1
revision_id: 1340658
locale: en-US
slug: Web/JavaScript/Reference/Global_Objects/Array
tags: "Array" "Example" "JavaScript" "Reference" "Global Objects"
title: Array
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: True
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{JSRef}}</div>

<p>The JavaScript <strong><code>Array</code></strong>&nbsp;object is a global object that&nbsp;is used in the&nbsp;construction&nbsp;of&nbsp;arrays; which are high-level, list-like objects.</p>

<p><strong>Create an Array</strong></p>

<pre class="brush: js">
var fruits = ['Apple', 'Banana'];

console.log(fruits.length);
// 2
</pre>

<p><strong>Access (index into) an Array item</strong></p>

<pre class="brush: js">
var first = fruits[0];
// Apple

var last = fruits[fruits.length - 1];
// Banana
</pre>

<p><strong>Loop over an Array</strong></p>

<pre class="brush: js">
fruits.forEach(function(item, index, array) {
&nbsp; console.log(item, index);
});
// Apple 0
// Banana 1
</pre>

<p><strong>Add to the end of an Array</strong></p>

<pre class="brush: js">
var newLength = fruits.push('Orange');
// ["Apple", "Banana", "Orange"]
</pre>

<p><strong>Remove from the end of an Array</strong></p>

<pre class="brush: js">
var last = fruits.pop(); // remove Orange (from the end)
// ["Apple", "Banana"];
</pre>

<p><strong>Remove from the front of an Array</strong></p>

<pre class="brush: js">
var first = fruits.shift(); // remove Apple from the front
// ["Banana"];
</pre>

<p><strong>Add to the front of an Array</strong></p>

<pre class="brush: js">
var newLength = fruits.unshift('Strawberry') // add to the front
// ["Strawberry", "Banana"];
</pre>

<p><strong>Find the index of an item in the Array</strong></p>

<pre class="brush: js">
fruits.push('Mango');
// ["Strawberry", "Banana", "Mango"]

var pos = fruits.indexOf('Banana');
// 1
</pre>

<p><strong>Remove an item by index position</strong></p>

<pre class="brush: js">
var removedItem = fruits.splice(pos, 1); // this is how to remove an item
                                        
// ["Strawberry", "Mango"]</pre>

<p><strong>Remove items from an index position</strong></p>

<pre class="brush: js">
var vegetables = ['Cabbage', 'Turnip', 'Radish', 'Carrot'];
console.log(vegetables); 
// ["Cabbage", "Turnip", "Radish", "Carrot"]

var pos = 1, n = 2;

var removedItems = vegetables.splice(pos, n); 
// this is how to remove items, n defines the number of items to be removed,
// from that position(pos) onward to the end of array.

console.log(vegetables); 
// ["Cabbage", "Carrot"] (the original array is changed)

console.log(removedItems); 
// ["Turnip", "Radish"]</pre>

<p><strong>Copy an Array</strong></p>

<pre class="brush: js">
var shallowCopy = fruits.slice(); // this is how to make a copy
// ["Strawberry", "<code>Mango</code>"]
</pre>

<h2 id="Syntax">Syntax</h2>

<pre class="syntaxbox">
[<var>element0</var>, <var>element1</var>, ..., <var>elementN</var>]
new Array(<var>element0</var>, <var>element1</var>[, ...[, <var>elementN</var>]])
new Array(<var>arrayLength</var>)</pre>

<h3 id="Parameters">Parameters</h3>

<dl>
 <dt><code>element<em>N</em></code></dt>
 <dd>A JavaScript array is initialized with the given elements, except in the case where a single argument is passed to the <code>Array</code> constructor and that argument is a number (see the arrayLength parameter below). Note that this special case only applies to JavaScript arrays created with the <code>Array</code> constructor, not array literals created with the bracket syntax.</dd>
 <dt><code>arrayLength</code></dt>
 <dd>If the only argument passed to the <code>Array</code> constructor is an integer between 0 and 2<sup>32</sup>-1 (inclusive), this returns a new JavaScript array with its&nbsp;<code>length</code>&nbsp;property set to that number (<strong>Note:</strong> this implies an array of <code>arrayLength</code> empty slots, not slots with actual <code>undefined</code> values). If the argument is any other number, a {{jsxref("RangeError")}} exception is thrown.</dd>
</dl>

<h2 id="Description">Description</h2>

<p>Arrays are list-like objects whose prototype has methods to perform traversal and mutation operations. Neither the length of a JavaScript array nor the types of its elements are fixed. Since an array's length can change at any time, and data can be stored at non-contiguous locations in the array, JavaScript arrays are not guaranteed to be dense; this depends on how the programmer chooses to use them. In general, these are convenient characteristics; but if these features are not desirable for your particular use, you might consider using typed arrays.</p>

<p>Arrays cannot use strings&nbsp;as element indexes (as in an&nbsp;<a href="https://en.wikipedia.org/wiki/Associative_array">associative array</a>) but must use&nbsp;integers. Setting or accessing via non-integers using&nbsp;<a href="/en-US/docs/Web/JavaScript/Guide/Working_with_Objects#Objects_and_properties">bracket notation</a> (or <a href="/en-US/docs/Web/JavaScript/Reference/Operators/Property_Accessors">dot notation</a>)&nbsp;will not set or retrieve an element from the array list itself, but will set or access a variable&nbsp;associated with that array's <a href="/en-US/docs/Web/JavaScript/Data_structures#Properties">object property&nbsp;collection</a>. The array's object properties and list of&nbsp;array elements are separate, and the array's <a href="/en-US/docs/Web/JavaScript/Guide/Indexed_collections#Array_methods">traversal and mutation operations</a> cannot be applied to these named properties.</p>

<h3 id="Accessing_array_elements">Accessing array elements</h3>

<p>JavaScript arrays are zero-indexed: the first element of an array is at index <code>0</code>, and the last element is at the index equal to the value of the array's {{jsxref("Array.length", "length")}} property minus 1. Using an invalid index number returns <code>undefined</code>.</p>

<pre class="brush: js">
var arr = ['this is the first element', 'this is the second element', 'this is the last element'];
console.log(arr[0]);              // logs 'this is the first element'
console.log(arr[1]);              // logs 'this is the second element'
console.log(arr[arr.length - 1]); // logs 'this is the last element'
</pre>

<p>Array elements are object properties in the same way that <code>toString</code> is a property, but trying to access an element of an array as follows throws a syntax error because the property name is not valid:</p>

<pre class="brush: js">
console.log(arr.0); // a syntax error
</pre>

<p>There is nothing special about JavaScript arrays and the properties that cause this. JavaScript properties that begin with a digit cannot be referenced with dot notation; and must be accessed using bracket notation. For example, if you had an object with a property named <code>'3d'</code>, it can only be referenced using bracket notation. E.g.:</p>

<pre class="brush: js">
var years = [1950, 1960, 1970, 1980, 1990, 2000, 2010];
console.log(years.0);   // a syntax error
console.log(years[0]);  // works properly
</pre>

<pre class="brush: js">
renderer.3d.setTexture(model, 'character.png');     // a syntax error
renderer['3d'].setTexture(model, 'character.png');  // works properly
</pre>

<p>Note that in the <code>3d</code> example, <code>'3d'</code> had to be quoted. It's possible to quote the JavaScript array indexes as well (e.g., <code>years['2']</code> instead of <code>years[2]</code>), although it's not necessary. The 2 in <code>years[2]</code> is coerced into a string by the JavaScript engine through an implicit <code>toString</code> conversion. It is, for this reason, that <code>'2'</code> and <code>'02'</code> would refer to two different slots on the <code>years</code> object and the following example could be <code>true</code>:</p>

<pre class="brush: js">
console.log(years['2'] != years['02']);
</pre>

<p>Similarly, object properties which happen to be reserved words(!) can only be accessed as string literals in bracket notation(but it can be accessed by dot notation in firefox 40.0a2 at least):</p>

<pre class="brush: js">
var promise = {
  'var'  : 'text',
  'array': [1, 2, 3, 4]
};

console.log(promise['var']);
</pre>

<h3 id="Relationship_between_length_and_numerical_properties">Relationship between <code>length</code> and numerical properties</h3>

<p>A JavaScript array's {{jsxref("Array.length", "length")}} property and numerical properties are connected. Several of the built-in array methods (e.g., {{jsxref("Array.join", "join")}}, {{jsxref("Array.slice", "slice")}}, {{jsxref("Array.indexOf", "indexOf")}}, etc.) take into account the value of an array's {{jsxref("Array.length", "length")}} property when they're called. Other methods (e.g., {{jsxref("Array.push", "push")}}, {{jsxref("Array.splice", "splice")}}, etc.) also result in updates to an array's {{jsxref("Array.length", "length")}} property.</p>

<pre class="brush: js">
var fruits = [];
fruits.push('banana', 'apple', 'peach');

console.log(fruits.length); // 3
</pre>

<p>When setting a property on a JavaScript array when the property is a valid array index and that index is outside the current bounds of the array, the engine will update the array's {{jsxref("Array.length", "length")}} property accordingly:</p>

<pre class="brush: js">
fruits[5] = 'mango';
console.log(fruits[5]); // 'mango'
console.log(Object.keys(fruits));  // ['0', '1', '2', '5']
console.log(fruits.length); // 6
</pre>

<p>Increasing the {{jsxref("Array.length", "length")}}.</p>

<pre class="brush: js">
fruits.length = 10;
console.log(Object.keys(fruits)); // ['0', '1', '2', '5']
console.log(fruits.length); // 10
</pre>

<p>Decreasing the {{jsxref("Array.length", "length")}} property does, however, delete elements.</p>

<pre class="brush: js">
fruits.length = 2;
console.log(Object.keys(fruits)); // ['0', '1']
console.log(fruits.length); // 2
</pre>

<p>This is explained further on the {{jsxref("Array.length")}} page.</p>

<h3 id="Creating_an_array_using_the_result_of_a_match">Creating an array using the result of a match</h3>

<p>The result of a match between a regular expression and a string can create a JavaScript array. This array has properties and elements which provide information about the match. Such an array is returned by {{jsxref("RegExp.exec")}}, {{jsxref("String.match")}}, and {{jsxref("String.replace")}}. To help explain these properties and elements, look at the following example and then refer to the table below:</p>

<pre class="brush: js">
// Match one d followed by one or more b's followed by one d
// Remember matched b's and the following d
// Ignore case

var myRe = /d(b+)(d)/i;
var myArray = myRe.exec('cdbBdbsbz');
</pre>

<p>The properties and elements returned from this match are as follows:</p>

<table class="fullwidth-table">
 <tbody>
  <tr>
   <td class="header">Property/Element</td>
   <td class="header">Description</td>
   <td class="header">Example</td>
  </tr>
  <tr>
   <td><code>input</code></td>
   <td>A read-only property that reflects the original string against which the regular expression was matched.</td>
   <td>cdbBdbsbz</td>
  </tr>
  <tr>
   <td><code>index</code></td>
   <td>A read-only property that is the zero-based index of the match in the string.</td>
   <td>1</td>
  </tr>
  <tr>
   <td><code>[0]</code></td>
   <td>A read-only element that specifies the last matched characters.</td>
   <td>dbBd</td>
  </tr>
  <tr>
   <td><code>[1], ...[n]</code></td>
   <td>Read-only elements that specify the parenthesized substring matches, if included in the regular expression. The number of possible parenthesized substrings is unlimited.</td>
   <td>[1]: bB<br />
    [2]: d</td>
  </tr>
 </tbody>
</table>

<h2 id="Properties">Properties</h2>

<dl>
 <dt><code>Array.length</code></dt>
 <dd>The <code>Array</code> constructor's length property whose value is 1.</dd>
 <dt>{{jsxref("Array.@@species", "get Array[@@species]")}}</dt>
 <dd>The constructor function that is used to create derived objects.</dd>
 <dt>{{jsxref("Array.prototype")}}</dt>
 <dd>Allows the addition of properties to all array objects.</dd>
</dl>

<h2 id="Methods">Methods</h2>

<dl>
 <dt>{{jsxref("Array.from()")}}</dt>
 <dd>Creates a new <code>Array</code> instance from an array-like or iterable object.</dd>
 <dt>{{jsxref("Array.isArray()")}}</dt>
 <dd>Returns true if a variable is an array, if not false.</dd>
 <dt>{{jsxref("Array.of()")}}</dt>
 <dd>Creates a new <code>Array</code> instance with a variable number of arguments, regardless of number or type of the arguments.</dd>
</dl>

<h2 id="Array_instances"><code>Array</code> instances</h2>

<p>All <code>Array</code> instances inherit from {{jsxref("Array.prototype")}}. The prototype object of the <code>Array</code> constructor can be modified to affect all <code>Array</code> instances.</p>

<h3 id="Properties_2">Properties</h3>

<div>{{page('/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/prototype', 'Properties')}}</div>

<h3 id="Methods_2">Methods</h3>

<h4 id="Mutator_methods">Mutator methods</h4>

<div>{{page('en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/prototype', 'Mutator_methods')}}</div>

<h4 id="Accessor_methods">Accessor methods</h4>

<div>{{page('en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/prototype', 'Accessor_methods')}}</div>

<h4 id="Iteration_methods">Iteration methods</h4>

<div>{{page('en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/prototype', 'Iteration_methods')}}</div>

<h2 id="Array_generic_methods"><code>Array</code> generic methods</h2>

<div class="warning">
<p><strong>Array generics are non-standard, deprecated and will get removed in the near future</strong>.&nbsp;</p>
</div>

<p>Sometimes you would like to apply array methods to strings or other array-like objects (such as function {{jsxref("Functions/arguments", "arguments", "", 1)}}). By doing this, you treat a string as an array of characters (or otherwise treat a non-array as an array). For example, in order to check that every character in the variable <var>str</var> is a letter, you would write:</p>

<pre class="brush: js">
function isLetter(character) {
  return character &gt;= 'a' &amp;&amp; character &lt;= 'z';
}

if (Array.prototype.every.call(str, isLetter)) {
  console.log("The string '" + str + "' contains only letters!");
}
</pre>

<p>This notation is rather wasteful and JavaScript 1.6 introduced a generic shorthand:</p>

<pre class="brush: js">
if (Array.every(str, isLetter)) {
  console.log("The string '" + str + "' contains only letters!");
}
</pre>

<p>{{jsxref("Global_Objects/String", "Generics", "#String_generic_methods", 1)}} are also available on {{jsxref("String")}}.</p>

<p>These are <strong>not</strong> part of ECMAScript standards and they are not supported by non-Gecko browsers. As a standard&nbsp;alternative, you can convert your object to a proper array using&nbsp;{{jsxref("Array.from()")}};&nbsp;although that method may&nbsp;not be supported in old browsers:</p>

<pre class="brush: js">
if (Array.from(str).every(isLetter)) { 
&nbsp; console.log("The string '" + str + "' contains only letters!"); 
}
</pre>

<h2 id="Examples">Examples</h2>

<h3 id="Creating_an_array">Creating an array</h3>

<p>The following example creates an array, <code>msgArray</code>, with a length of 0, then assigns values to <code>msgArray[0]</code> and <code>msgArray[99]</code>, changing the length of the array to 100.</p>

<pre class="brush: js">
var msgArray = [];
msgArray[0] = 'Hello';
msgArray[99] = 'world';

if (msgArray.length === 100) {
  console.log('The length is 100.');
}
</pre>

<h3 id="Creating_a_two-dimensional_array">Creating a two-dimensional array</h3>

<p>The following creates a chess board as a two-dimensional array of strings. The first move is made by copying the 'p' in (6,4) to (4,4). The old position (6,4) is made blank.</p>

<pre class="brush: js">
var board = [ 
  ['R','N','B','Q','K','B','N','R'],
  ['P','P','P','P','P','P','P','P'],
  [' ',' ',' ',' ',' ',' ',' ',' '],
  [' ',' ',' ',' ',' ',' ',' ',' '],
  [' ',' ',' ',' ',' ',' ',' ',' '],
  [' ',' ',' ',' ',' ',' ',' ',' '],
  ['p','p','p','p','p','p','p','p'],
  ['r','n','b','q','k','b','n','r'] ];

console.log(board.join('\n') + '\n\n');

// Move King's Pawn forward 2
board[4][4] = board[6][4];
board[6][4] = ' ';
console.log(board.join('\n'));
</pre>

<p>Here is the output:</p>

<pre class="eval">
R,N,B,Q,K,B,N,R
P,P,P,P,P,P,P,P
 , , , , , , , 
 , , , , , , , 
 , , , , , , , 
 , , , , , , , 
p,p,p,p,p,p,p,p
r,n,b,q,k,b,n,r

R,N,B,Q,K,B,N,R
P,P,P,P,P,P,P,P
 , , , , , , , 
 , , , , , , , 
 , , , ,p, , , 
 , , , , , , , 
p,p,p,p, ,p,p,p
r,n,b,q,k,b,n,r
</pre>

<h3 id="Using_an_array_to_tabulate_a_set_of_values">Using an array to tabulate a set of values</h3>

<pre class="brush: js">
values = [];
for (var x = 0; x &lt; 10; x++){
 values.push([
  2 ** x,
  2 * x ** 2
 ])
};
console.table(values)</pre>

<p>Results in</p>

<pre class="eval">
0	1	0
1	2	2
2	4	8
3	8	18
4	16	32
5	32	50
6	64	72
7	128	98
8	256	128
9	512	162</pre>

<p>(First column is the (index))</p>

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
   <td>Initial definition.</td>
  </tr>
  <tr>
   <td>{{SpecName('ES5.1', '#sec-15.4', 'Array')}}</td>
   <td>{{Spec2('ES5.1')}}</td>
   <td>New methods added: {{jsxref("Array.isArray")}}, {{jsxref("Array.prototype.indexOf", "indexOf")}}, {{jsxref("Array.prototype.lastIndexOf", "lastIndexOf")}}, {{jsxref("Array.prototype.every", "every")}}, {{jsxref("Array.prototype.some", "some")}}, {{jsxref("Array.prototype.forEach", "forEach")}}, {{jsxref("Array.prototype.map", "map")}}, {{jsxref("Array.prototype.filter", "filter")}}, {{jsxref("Array.prototype.reduce", "reduce")}}, {{jsxref("Array.prototype.reduceRight", "reduceRight")}}</td>
  </tr>
  <tr>
   <td>{{SpecName('ES6', '#sec-array-objects', 'Array')}}</td>
   <td>{{Spec2('ES6')}}</td>
   <td>New methods added: {{jsxref("Array.from")}}, {{jsxref("Array.of")}}, {{jsxref("Array.prototype.find", "find")}}, {{jsxref("Array.prototype.findIndex", "findIndex")}}, {{jsxref("Array.prototype.fill", "fill")}}, {{jsxref("Array.prototype.copyWithin", "copyWithin")}}</td>
  </tr>
  <tr>
   <td>{{SpecName('ESDraft', '#sec-array-objects', 'Array')}}</td>
   <td>{{Spec2('ESDraft')}}</td>
   <td>New method added: {{jsxref("Array.prototype.includes()")}}</td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<div class="hidden">The compatibility table in this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</div>

<p>{{Compat("javascript.builtins.Array")}}</p>

<h2 id="See_also">See also</h2>

<ul>
 <li><a href="/en-US/docs/Web/JavaScript/Guide/Working_with_Objects#Indexing_object_properties">JavaScript Guide: “Indexing object properties”</a></li>
 <li><a href="/en-US/docs/Web/JavaScript/Guide/Predefined_Core_Objects#Array_Object">JavaScript Guide: “Predefined Core Objects: <code>Array</code> Object”</a></li>
 <li><a href="/en-US/docs/Web/JavaScript/Reference/Operators/Array_comprehensions">Array comprehensions</a></li>
 <li><a href="https://github.com/plusdude/array-generics">Polyfill for JavaScript 1.8.5 Array Generics and ECMAScript 5 Array Extras</a></li>
 <li><a href="/en-US/docs/JavaScript_typed_arrays">Typed Arrays</a></li>
</ul>

