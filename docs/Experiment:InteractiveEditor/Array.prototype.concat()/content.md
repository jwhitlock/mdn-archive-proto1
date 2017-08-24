---
version: prototype1
revision_id: 1293073
locale: en-US
slug: Experiment:InteractiveEditor/Array.prototype.concat()
tags: "Array" "Method" "JavaScript" "Prototype" "Reference"
title: Array.prototype.concat()
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{JSRef}}</div>

<p>The <code><strong>concat()</strong></code> method is used to merge two or more arrays. This method does not change the existing arrays, but instead returns a new array.</p>

<div>{{EmbedInteractiveExample("pages/js/array-concat.html")}}</div>

<h2 id="Syntax">Syntax</h2>

<pre class="syntaxbox">
var <var>new_array</var> = <var>old_array</var>.concat(<var>value1</var>[, <var>value2</var>[, ...[, <var>valueN</var>]]])</pre>

<h3 id="Parameters">Parameters</h3>

<dl>
 <dt><code>value<em>N</em></code></dt>
 <dd>Arrays and/or values to concatenate into a new array. See the description below for details.</dd>
</dl>

<h3 id="Return_value">Return value</h3>

<p>A new {{jsxref("Array")}} instance.</p>

<h2 id="Description">Description</h2>

<p>The <code>concat</code> method creates a new array consisting of the elements in the object on which it is called, followed in order by, for each argument, the elements of that argument (if the argument is an array) or the argument itself (if the argument is not an array). It does not recurse into nested array arguments.</p>

<p>The <code>concat</code> method does not alter <code>this</code> or any of the arrays provided as arguments but instead returns a shallow copy that contains copies of the same elements combined from the original arrays. Elements of the original arrays are copied into the new array as follows:</p>

<ul>
 <li>Object references (and not the actual object): <code>concat</code> copies object references into the new array. Both the original and new array refer to the same object. That is, if a referenced object is modified, the changes are visible to both the new and original arrays. This includes elements of array arguments that are also arrays.</li>
 <li>Data types such&nbsp;as strings, numbers and booleans (not {{jsxref("Global_Objects/String", "String")}}, {{jsxref("Global_Objects/Number", "Number")}}, and {{jsxref("Global_Objects/Boolean", "Boolean")}} objects): <code>concat</code> copies the values of strings and numbers into the new array.</li>
</ul>

<div class="note">
<p><strong>Note:</strong> Concatenating array(s)/value(s) will leave the originals untouched. Furthermore, any operation on the new array(only if the element is not object reference)&nbsp;will have no effect on the original arrays, and vice versa.</p>
</div>

<h2 id="Examples">Examples</h2>

<h3 id="Concatenating_two_arrays">Concatenating two arrays</h3>

<p>The following code concatenates two arrays:</p>

<pre class="brush: js">
var alpha = ['a', 'b', 'c'];
var numeric = [1, 2, 3];

alpha.concat(numeric);
// result in ['a', 'b', 'c', 1, 2, 3]
</pre>

<h3 id="Concatenating_three_arrays">Concatenating three arrays</h3>

<p>The following code concatenates three arrays:</p>

<pre class="brush: js">
var num1 = [1, 2, 3],
    num2 = [4, 5, 6],
    num3 = [7, 8, 9];

var nums = num1.concat(num2, num3);

console.log(nums); 
// results in [1, 2, 3, 4, 5, 6, 7, 8, 9]
</pre>

<h3 id="Concatenating_values_to_an_array">Concatenating values to an array</h3>

<p>The following code concatenates three values to an array:</p>

<pre class="brush: js">
var alpha = ['a', 'b', 'c'];

var alphaNumeric = alpha.concat(1, [2, 3]);

console.log(alphaNumeric); 
// results in ['a', 'b', 'c', 1, 2, 3]
</pre>

<h3 id="Concatenating_nested_arrays">Concatenating nested arrays</h3>

<p>The following code concatenates nested arrays and demonstrates retention of references:</p>

<pre class="brush: js">
var num1 = [[1]];
var num2 = [2, [3]];

var nums = num1.concat(num2);

console.log(nums);
// results in [[1], 2, [3]]

// modify the first element of num1
num1[0].push(4);

console.log(nums);
// results in [[1, 4], 2, [3]]
</pre>

<h2 id="Specifications">Specifications</h2>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="col">Specification</th>
   <th scope="col">Status</th>
   <th scope="col">Comment</th>
  </tr>
  <tr>
   <td>{{SpecName('ES3')}}</td>
   <td>{{Spec2('ES3')}}</td>
   <td>Initial definition. Implemented in JavaScript 1.2.</td>
  </tr>
  <tr>
   <td>{{SpecName('ES5.1', '#sec-15.4.4.4', 'Array.prototype.concat')}}</td>
   <td>{{Spec2('ES5.1')}}</td>
   <td>&nbsp;</td>
  </tr>
  <tr>
   <td>{{SpecName('ES6', '#sec-array.prototype.concat', 'Array.prototype.concat')}}</td>
   <td>{{Spec2('ES6')}}</td>
   <td>&nbsp;</td>
  </tr>
  <tr>
   <td>{{SpecName('ESDraft', '#sec-array.prototype.concat', 'Array.prototype.concat')}}</td>
   <td>{{Spec2('ESDraft')}}</td>
   <td>&nbsp;</td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<div>{{CompatibilityTable}}</div>

<div id="compat-desktop">
<table class="compat-table">
 <tbody>
  <tr>
   <th>Feature</th>
   <th>Chrome</th>
   <th>Firefox (Gecko)</th>
   <th>Edge</th>
   <th>Internet Explorer</th>
   <th>Opera</th>
   <th>Safari</th>
  </tr>
  <tr>
   <td>Basic support</td>
   <td>{{CompatChrome("1.0")}}</td>
   <td>{{CompatGeckoDesktop("1.7")}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatIE("5.5")}}</td>
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
   <th>Feature</th>
   <th>Android</th>
   <th>Chrome for Android</th>
   <th>Edge</th>
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
   <td>{{CompatVersionUnknown}}</td>
  </tr>
 </tbody>
</table>
</div>

<h2 id="See_also">See also</h2>

<ul>
 <li>{{jsxref("Array.push", "push")}} / {{jsxref("Array.pop", "pop")}}&nbsp;— add/remove elements from the end of the array</li>
 <li>{{jsxref("Array.unshift", "unshift")}} / {{jsxref("Array.shift", "shift")}}&nbsp;— add/remove elements from the beginning of the array</li>
 <li>{{jsxref("Array.splice", "splice")}}&nbsp;— add/remove elements from the specified location of the array</li>
 <li>{{jsxref("String.prototype.concat()")}}</li>
 <li>{{jsxref("Symbol.isConcatSpreadable")}} – control flattening.</li>
</ul>

