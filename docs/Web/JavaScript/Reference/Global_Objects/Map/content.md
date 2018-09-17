---
version: prototype1
revision_id: 1411826
locale: en-US
slug: Web/JavaScript/Reference/Global_Objects/Map
tags: "ECMAScript 2015" "JavaScript" "Map"
title: Map
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: True
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{JSRef}}</div>

<p><span class="seoSummary">The <strong><code>Map</code></strong> object holds key-value pairs.</span> Unlike other languages, any value (both objects and {{Glossary("Primitive", "primitive values")}}) may be used as either a key or a value.</p>

<h2 id="Syntax">Syntax</h2>

<pre class="syntaxbox">new Map([<em>iterable</em>])</pre>

<h3 id="Parameters">Parameters</h3>

<dl>
	<dt><code>iterable</code></dt>
	<dd>An {{jsxref("Array")}} or other <a href="/en-US/docs/Web/JavaScript/Guide/iterable">iterable</a> object whose elements are key-value pairs (arrays with two elements, e.g. <code>[[ 1, 'one' ],[ 2, 'two' ]]</code>). Each key-value pair is added to the new <code>Map</code>; <code>null</code> values are treated as <code>undefined</code>.</dd>
</dl>

<h2 id="Description">Description</h2>

<p>A <code>Map</code> object iterates its elements in insertion order — a {{jsxref("Statements/for...of", "for...of")}} loop returns an array of <code>[key, value]</code> for each iteration.<br>
 </p>

<h3 id="Key_equality">Key equality</h3>

<p>Key equality is based on the "SameValueZero" algorithm: <code>NaN</code> is considered the same as <code>NaN</code> (even though <code>NaN !== NaN</code>) and all other values are considered equal according to the semantics of the <code>===</code> operator. In the current ECMAScript specification <code>-0</code> and <code>+0</code> are considered equal, although this was not so in earlier drafts. See "Value equality for -0 and 0" in the <a href="#Browser_compatibility">browser compatibility</a> table for details.</p>

<h3 id="Objects_and_maps_compared">Objects and maps compared</h3>

<p>{{jsxref("Object", "Objects")}} are similar to <code>Maps</code> in that both let you set keys to values, retrieve those values, delete keys, and detect whether something is stored at a key. Because of this (and because there were no built-in alternatives), <code>Object</code>s have been used as <code>Maps</code> historically; however, there are important differences that make using a <code>Map</code> preferable in certain cases:</p>

<ul>
	<li>The keys of an <code>Object</code> are {{jsxref("String", "Strings")}} and {{jsxref("Symbol", "Symbols")}}, whereas they can be any value for a <code>Map</code>, including functions, objects, and any primitive.</li>
	<li>The keys in Map are ordered while keys added to object are not. Thus, when iterating over it, a Map object returns keys in order of insertion.</li>
	<li>You can get the size of a <code>Map</code> easily with the <code>size</code> property, while the number of properties in an <code>Object</code> must be determined manually.</li>
	<li>A <code>Map</code> is an <a href="/en-US/docs/Web/JavaScript/Guide/iterable">iterable</a> and can thus be directly iterated, whereas iterating over an <code>Object</code> requires obtaining its keys in some fashion and iterating over them.</li>
	<li>An <code>Object</code> has a prototype, so there are default keys in the map that could collide with your keys if you're not careful. As of ES5 this can be bypassed by using <code>map = Object.create(null)</code>, but this is seldom done.</li>
	<li>A <code>Map</code> may perform better in scenarios involving frequent addition and removal of key pairs.</li>
</ul>

<h2 id="Properties">Properties</h2>

<dl>
	<dt><code>Map.length</code></dt>
	<dd>The value of the <code>length</code> property is 0.</dd>
	<dt>{{jsxref("Map.@@species", "get Map[@@species]")}}</dt>
	<dd>The constructor function that is used to create derived objects.</dd>
	<dt>{{jsxref("Map.prototype")}}</dt>
	<dd>Represents the prototype for the <code>Map</code> constructor. Allows the addition of properties to all <code>Map</code> objects.</dd>
</dl>

<h2 id="Map_instances"><code>Map</code> instances</h2>

<p>All <code>Map</code> instances inherit from {{jsxref("Map.prototype")}}.</p>

<h3 id="Properties_2">Properties</h3>

<p>{{page('en-US/Web/JavaScript/Reference/Global_Objects/Map/prototype','Properties')}}</p>

<h3 id="Methods">Methods</h3>

<p>{{page('en-US/Web/JavaScript/Reference/Global_Objects/Map/prototype','Methods')}}</p>

<h2 id="Examples">Examples</h2>

<h3 id="Using_the_Map_object">Using the <code>Map</code> object</h3>

<pre class="brush: js">var myMap = new Map();

var keyString = 'a string',
    keyObj = {},
    keyFunc = function() {};

// setting the values
myMap.set(keyString, "value associated with 'a string'");
myMap.set(keyObj, 'value associated with keyObj');
myMap.set(keyFunc, 'value associated with keyFunc');

myMap.size; // 3

// getting the values
myMap.get(keyString);    // "value associated with 'a string'"
myMap.get(keyObj);       // "value associated with keyObj"
myMap.get(keyFunc);      // "value associated with keyFunc"

myMap.get('a string');   // "value associated with 'a string'"
                         // because keyString === 'a string'
myMap.get({});           // undefined, because keyObj !== {}
myMap.get(function() {}) // undefined, because keyFunc !== function () {}
</pre>

<h3 id="Using_NaN_as_Map_keys">Using <code>NaN</code> as <code>Map</code> keys</h3>

<p><code>NaN</code> can also be used as a key. Even though every <code>NaN</code> is not equal to itself (<code>NaN !== NaN</code> is true), the following example works because <code>NaN</code>s are indistinguishable from each other:</p>

<pre class="brush: js">var myMap = new Map();
myMap.set(NaN, 'not a number');

myMap.get(NaN); // "not a number"

var otherNaN = Number('foo');
myMap.get(otherNaN); // "not a number"
</pre>

<h3 id="Iterating_Maps_with_for..of">Iterating <code>Maps</code> with <code>for..of</code></h3>

<p>Maps can be iterated using a <code>for..of</code> loop:</p>

<pre class="brush: js">var myMap = new Map();
myMap.set(0, 'zero');
myMap.set(1, 'one');
for (var [key, value] of myMap) {
  console.log(key + ' = ' + value);
}
// 0 = zero
// 1 = one

for (var key of myMap.keys()) {
  console.log(key);
}
// 0
// 1

for (var value of myMap.values()) {
  console.log(value);
}
// zero
// one

for (var [key, value] of myMap.entries()) {
  console.log(key + ' = ' + value);
}
// 0 = zero
// 1 = one
</pre>

<h3 id="Iterating_Maps_with_forEach()">Iterating <code>Maps</code> with <code>forEach()</code></h3>

<p>Maps can be iterated using the <code>forEach()</code> method:</p>

<pre class="brush: js">myMap.forEach(function(value, key) {
  console.log(key + ' = ' + value);
});
// Will show 2 logs; first with "0 = zero" and second with "1 = one"
</pre>

<h3 id="Relation_with_Array_objects">Relation with <code>Array</code> objects</h3>

<pre class="brush: js">var kvArray = [['key1', 'value1'], ['key2', 'value2']];

// Use the regular Map constructor to transform a 2D key-value Array into a map
var myMap = new Map(kvArray);

myMap.get('key1'); // returns "value1"

// Use the Array.from function to transform a map into a 2D key-value Array
console.log(Array.from(myMap)); // Will show you exactly the same Array as kvArray

// Or use the keys or values iterators and convert them to an array
console.log(Array.from(myMap.keys())); // Will show ["key1", "key2"]
</pre>

<h3 id="Cloning_and_merging_Maps">Cloning and merging <code>Maps</code></h3>

<p>Just like Arrays, Maps can be cloned:</p>

<pre class="brush: js">var original = new Map([
  [1, 'one']
]);

var clone = new Map(original);

console.log(clone.get(1)); // one
console.log(original === clone); // false. Useful for shallow comparison</pre>

<p>Keep in mind that the <em>data</em> itself is not cloned</p>

<p>Maps can be merged, maintaining key uniqueness:</p>

<pre class="brush: js">var first = new Map([
  [1, 'one'],
  [2, 'two'],
  [3, 'three'],
]);

var second = new Map([
  [1, 'uno'],
  [2, 'dos']
]);

// Merge two maps. The last repeated key wins.
// Spread operator essentially converts a Map to an Array
var merged = new Map([...first, ...second]);

console.log(merged.get(1)); // uno
console.log(merged.get(2)); // dos
console.log(merged.get(3)); // three</pre>

<p>Maps can be merged with Arrays, too:</p>

<pre class="brush: js">var first = new Map([
  [1, 'one'],
  [2, 'two'],
  [3, 'three'],
]);

var second = new Map([
  [1, 'uno'],
  [2, 'dos']
]);

// Merge maps with an array. The last repeated key wins.
var merged = new Map([...first, ...second, [1, 'eins']]);

console.log(merged.get(1)); // eins
console.log(merged.get(2)); // dos
console.log(merged.get(3)); // three</pre>

<h3 id="Specifications">Specifications</h3>

<table class="standard-table">
	<tbody>
		<tr>
			<th scope="col">Specification</th>
			<th scope="col">Status</th>
			<th scope="col">Comment</th>
		</tr>
		<tr>
			<td>{{SpecName('ES2015', '#sec-map-objects', 'Map')}}</td>
			<td>{{Spec2('ES2015')}}</td>
			<td>Initial definition.</td>
		</tr>
		<tr>
			<td>{{SpecName('ESDraft', '#sec-map-objects', 'Map')}}</td>
			<td>{{Spec2('ESDraft')}}</td>
			<td> </td>
		</tr>
	</tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<div class="hidden">The compatibility table on this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</div>

<p>{{Compat("javascript.builtins.Map")}}</p>

<h2 id="See_also">See also</h2>

<ul>
	<li><a href="https://bugzilla.mozilla.org/show_bug.cgi?id=697479" class="link-https">Map and Set bug at Mozilla</a></li>
	<li><a href="http://wiki.ecmascript.org/doku.php?id=harmony:simple_maps_and_sets" class="external">ECMAScript Harmony proposal</a></li>
	<li>{{jsxref("Set")}}</li>
	<li>{{jsxref("WeakMap")}}</li>
	<li>{{jsxref("WeakSet")}}</li>
</ul>
