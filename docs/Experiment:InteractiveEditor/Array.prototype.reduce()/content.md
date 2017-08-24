---
version: prototype1
revision_id: 1293069
locale: en-US
slug: Experiment:InteractiveEditor/Array.prototype.reduce()
tags: "Array" "ECMAScript5" "Method" "Reduce" "JavaScript" "Prototype" "Reference"
title: Array.prototype.reduce()
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{JSRef}}</div>

<p>The <code><strong>reduce()</strong></code> method applies a function against an accumulator and each element in the array (from left to right) to reduce it to a single value.</p>

<div>{{EmbedInteractiveExample("pages/js/array-reduce.html")}}</div>

<h2 id="Syntax">Syntax</h2>

<pre class="syntaxbox">
<var>arr</var>.reduce(<var>callback[, </var><var>initialValue]</var>)</pre>

<h3 id="Parameters">Parameters</h3>

<dl>
 <dt><code>callback</code></dt>
 <dd>Function to execute on each element in the array, taking four arguments:
 <dl>
  <dt><code>accumulator</code></dt>
  <dd>The accumulator accumulates the callback's return values; it is the accumulated value previously returned in the last invocation of the callback, or <code>initialValue</code>, if supplied (see below).</dd>
  <dt><code>currentValue</code></dt>
  <dd>The current element being processed in the array.</dd>
  <dt><code>currentIndex</code></dt>
  <dd>The index of the current element being processed in the array. Starts at index 0, if an <code>initialValue</code> is provided, and at index 1 otherwise.</dd>
  <dt><code>array</code></dt>
  <dd>The array <code>reduce</code> was called upon.</dd>
 </dl>
 </dd>
 <dt><code>initialValue</code></dt>
 <dd>[Optional] Value to use as the first argument to the first call of the <code>callback</code>. If no initial value is supplied, the first element in the array will be used. Calling reduce on an empty array without an initial value is an error.</dd>
</dl>

<h3 id="Return_value">Return value</h3>

<p>The value that results from the reduction.</p>

<h2 id="Description">Description</h2>

<p><code>reduce</code> executes the <code>callback</code> function once for each element present in the array, excluding holes in the array, receiving four arguments:</p>

<ul>
 <li><code>accumulator</code></li>
 <li><code>currentValue</code></li>
 <li><code>currentIndex</code></li>
 <li><code>array</code></li>
</ul>

<p>The first time the callback is called, <code>accumulator</code> and <code>currentValue</code> can be one of two values. If <code>initialValue</code> is provided in the call to <code>reduce</code>, then <code>accumulator</code> will be equal to <code>initialValue</code>, and <code>currentValue</code> will be equal to the first value in the array. If no <code>initialValue</code> is provided, then <code>accumulator</code> will be equal to the first value in the array, and <code>currentValue</code> will be equal to the second.</p>

<p><strong>Note:</strong> If <code>initialValue</code> isn't provided, reduce will execute the callback function&nbsp;starting at index 1, skipping the first index. If <code>initialValue</code> is provided, it will start at index 0.</p>

<p>If the array is empty and no <code>initialValue</code> is provided, {{jsxref("TypeError")}} will be thrown. If the array has only one element (regardless of position) and no <code>initialValue</code> is provided, or if <code>initialValue</code> is provided but the array is empty, the solo value will be returned <em>without calling <code>callback</code>.</em></p>

<p>It is usually safer to provide an initial value because there are three possible outputs without <code>initialValue</code>, as shown in the following example.</p>

<pre class="brush: js">
var maxCallback = ( acc, cur ) =&gt; Math.max( acc.x, cur.x );
var maxCallback2 = ( max, cur ) =&gt; Math.max( max, cur );

// reduce() without initialValue
[ { x: 22 }, { x: 42 } ].reduce( maxCallback ); // 42
[ { x: 22 }            ].reduce( maxCallback ); // { x: 22 }
[                      ].reduce( maxCallback ); // TypeError

// map/reduce; better solution, also works for empty arrays
[ { x: 22 }, { x: 42 } ].map( el =&gt; el.x )
                        .reduce( maxCallback2, -Infinity );
</pre>

<h3 id="How_reduce_works">How reduce works</h3>

<p>Suppose the following use of <code>reduce</code> occurred:</p>

<pre class="brush: js">
[0, 1, 2, 3, 4].reduce(
&nbsp; function (
<code>    accumulator,</code>
&nbsp;   <code>currentValue</code>,
&nbsp;   <code>currentIndex</code>,
&nbsp;   array
  ) {
    return <code>accumulator</code> + currentValue;
  }
);
</pre>

<p>The callback would be invoked four times, with the arguments and return values in each call being as follows:</p>

<table>
 <thead>
  <tr>
   <th scope="col"><code>callback</code></th>
   <th scope="col"><code>accumulator</code></th>
   <th scope="col"><code>currentValue</code></th>
   <th scope="col"><code>currentIndex</code></th>
   <th scope="col"><code>array</code></th>
   <th scope="col">return value</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <th scope="row">first call</th>
   <td><code>0</code></td>
   <td><code>1</code></td>
   <td><code>1</code></td>
   <td><code>[0, 1, 2, 3, 4]</code></td>
   <td><code>1</code></td>
  </tr>
  <tr>
   <th scope="row">second call</th>
   <td><code>1</code></td>
   <td><code>2</code></td>
   <td><code>2</code></td>
   <td><code>[0, 1, 2, 3, 4]</code></td>
   <td><code>3</code></td>
  </tr>
  <tr>
   <th scope="row">third call</th>
   <td><code>3</code></td>
   <td><code>3</code></td>
   <td><code>3</code></td>
   <td><code>[0, 1, 2, 3, 4]</code></td>
   <td><code>6</code></td>
  </tr>
  <tr>
   <th scope="row">fourth call</th>
   <td><code>6</code></td>
   <td><code>4</code></td>
   <td><code>4</code></td>
   <td><code>[0, 1, 2, 3, 4]</code></td>
   <td><code>10</code></td>
  </tr>
 </tbody>
</table>

<p>The value returned by <code>reduce</code> would be that of the last callback invocation (<code>10</code>).</p>

<p>You can also provide an {{jsxref("Functions/Arrow_functions", "Arrow Function","",1)}}&nbsp;in lieu of a full function. The code below will produce the same output as the code in the block&nbsp;above:</p>

<pre class="brush: js">
[0, 1, 2, 3, 4].reduce( (prev, curr) =&gt; prev + curr );
</pre>

<p>If you were to provide an initial value as the second argument to <code>reduce</code>, the result would look like this:</p>

<pre class="brush: js">
[0, 1, 2, 3, 4].reduce(
&nbsp; (<code>accumulator</code>, currentValue, currentIndex, array) =&gt; {
    return <code>accumulator</code> + currentValue;
  },
  10
);
</pre>

<table>
 <thead>
  <tr>
   <th scope="col"><code>callback</code></th>
   <th scope="col"><code>accumulator</code></th>
   <th scope="col"><code>currentValue</code></th>
   <th scope="col"><code>currentIndex</code></th>
   <th scope="col"><code>array</code></th>
   <th scope="col">return value</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <th scope="row">first call</th>
   <td><code>10</code></td>
   <td><code>0</code></td>
   <td><code>0</code></td>
   <td><code>[0, 1, 2, 3, 4]</code></td>
   <td><code>10</code></td>
  </tr>
  <tr>
   <th scope="row">second call</th>
   <td><code>10</code></td>
   <td><code>1</code></td>
   <td><code>1</code></td>
   <td><code>[0, 1, 2, 3, 4]</code></td>
   <td><code>11</code></td>
  </tr>
  <tr>
   <th scope="row">third call</th>
   <td><code>11</code></td>
   <td><code>2</code></td>
   <td><code>2</code></td>
   <td><code>[0, 1, 2, 3, 4]</code></td>
   <td><code>13</code></td>
  </tr>
  <tr>
   <th scope="row">fourth call</th>
   <td><code>13</code></td>
   <td><code>3</code></td>
   <td><code>3</code></td>
   <td><code>[0, 1, 2, 3, 4]</code></td>
   <td><code>16</code></td>
  </tr>
  <tr>
   <th scope="row">fifth call</th>
   <td><code>16</code></td>
   <td><code>4</code></td>
   <td><code>4</code></td>
   <td><code>[0, 1, 2, 3, 4]</code></td>
   <td><code>20</code></td>
  </tr>
 </tbody>
</table>

<p>The value returned by&nbsp;<code>reduce</code> in this case would be <code>20</code>.</p>

<h2 id="Examples">Examples</h2>

<h3 id="Sum_all_the_values_of_an_array">Sum all the values of an array</h3>

<pre class="brush: js">
var sum = [0, 1, 2, 3].reduce(function (a, b) {
  return a + b;
}, 0);
// sum is 6
</pre>

<p>Alternatively, written with an arrow function:</p>

<pre class="brush: js">
var total = [ 0, 1, 2, 3 ].reduce(
&nbsp; ( acc, cur ) =&gt; acc + cur,
&nbsp; 0
);</pre>

<h3 id="Flatten_an_array_of_arrays">Flatten an array of arrays</h3>

<pre class="brush: js">
var flattened = [[0, 1], [2, 3], [4, 5]].reduce(
&nbsp; function(a, b) {
    return a.concat(b);
  },
&nbsp; []
);
// flattened is [0, 1, 2, 3, 4, 5]
</pre>

<p>Alternatively, written with an arrow function:</p>

<pre class="brush: js">
var flattened = [[0, 1], [2, 3], [4, 5]].reduce(
&nbsp; ( acc, cur ) =&gt; acc.concat(cur),
&nbsp; []
);
</pre>

<h3 id="Counting_instances_of_values_in_an_object">Counting instances of&nbsp;values in an object</h3>

<pre class="brush: js">
var names = ['Alice', 'Bob', 'Tiff', 'Bruce', 'Alice'];

var countedNames = names.reduce(function (allNames, name) { 
  if (name in allNames) {
    allNames[name]++;
&nbsp; }
&nbsp; else {
&nbsp;   allNames[name] = 1;
&nbsp; }
  return allNames;
}, {});
// countedNames is:
// { 'Alice': 2, 'Bob': 1, 'Tiff': 1, 'Bruce': 1 }
</pre>

<h3 id="Bonding_arrays_contained_in_an_array_of_objects_using_the_spread_operator_and_initialValue">Bonding arrays contained in an array of objects using the spread operator and initialValue</h3>

<pre class="brush: js">
// friends - an array of objects 
// where object field "books" - list of favorite books 
var friends = [{
&nbsp; name: 'Anna',
&nbsp; books: ['Bible', 'Harry Potter'],
&nbsp; age: 21
}, {
&nbsp; name: 'Bob',
&nbsp; books: ['War and peace', 'Romeo and Juliet'],
&nbsp; age: 26
}, {
&nbsp; name: 'Alice',
&nbsp; books: ['The Lord of the Rings', 'The Shining'],
&nbsp; age: 18
}];

// allbooks - list which will contain all friends' books +  
// additional list contained in initialValue
var allbooks = friends.reduce(function(prev, curr) {
  return [...prev, ...curr.books];
}, ['Alphabet']);

// allbooks = [
//   'Alphabet', 'Bible', 'Harry Potter', 'War and peace', 
//   'Romeo and Juliet', 'The Lord of the Rings',
//   'The Shining'
// ]</pre>

<h2 id="Polyfill">Polyfill</h2>

<pre class="brush: js">
// Production steps of ECMA-262, Edition 5, 15.4.4.21
// Reference: http://es5.github.io/#x15.4.4.21
// https://tc39.github.io/ecma262/#sec-array.prototype.reduce
if (!Array.prototype.reduce) {
  Object.defineProperty(Array.prototype, 'reduce', {
    value: function(callback /*, initialValue*/) {
      if (this === null) {
        throw new TypeError( 'Array.prototype.reduce ' + 
          'called on null or undefined' );
      }
      if (typeof callback !== 'function') {
        throw new TypeError( callback +
&nbsp;         ' is not a function');
      }

      // 1. Let O be ? ToObject(this value).
      var o = Object(this);

      // 2. Let len be ? ToLength(? Get(O, "length")).
      var len = o.length &gt;&gt;&gt; 0; 

      // Steps 3, 4, 5, 6, 7      
      var k = 0; 
      var value;

      if (arguments.length &gt;= 2) {
        value = arguments[1];
      } else {
        while (k &lt; len &amp;&amp; !(k in o)) {
          k++; 
        }

        // 3. If len is 0 and initialValue is not present,
&nbsp;       //    throw a TypeError exception.
        if (k &gt;= len) {
          throw new TypeError( 'Reduce of empty array ' +
&nbsp;           'with no initial value' );
        }
        value = o[k++];
      }

      // 8. Repeat, while k &lt; len
      while (k &lt; len) {
        // a. Let Pk be ! ToString(k).
        // b. Let kPresent be ? HasProperty(O, Pk).
        // c. If kPresent is true, then
        //    i.  Let kValue be ? Get(O, Pk).
        //    ii. Let accumulator be ? Call(
&nbsp;       //          callbackfn, undefined,
 &nbsp;      //          « accumulator, kValue, k, O »).
        if (k in o) {
          value = callback(value, o[k], k, o);
        }

        // d. Increase k by 1.      
        k++;
      }

      // 9. Return accumulator.
      return value;
    }
  });
}
</pre>

<p>If you need to support truly obsolete JavaScript engines that don't support <code><a href="/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/defineProperty">Object.defineProperty</a></code>, it's best not to polyfill <code>Array.prototype</code> methods at all, as you can't make them non-enumerable.</p>

<h2 id="Specifications">Specifications</h2>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="col">Specification</th>
   <th scope="col">Status</th>
   <th scope="col">Comment</th>
  </tr>
  <tr>
   <td>{{SpecName('ES5.1', '#sec-15.4.4.21', 'Array.prototype.reduce')}}</td>
   <td>{{Spec2('ES5.1')}}</td>
   <td>Initial definition. Implemented in JavaScript 1.8.</td>
  </tr>
  <tr>
   <td>{{SpecName('ES6', '#sec-array.prototype.reduce', 'Array.prototype.reduce')}}</td>
   <td>{{Spec2('ES6')}}</td>
   <td>&nbsp;</td>
  </tr>
  <tr>
   <td>{{SpecName('ESDraft', '#sec-array.prototype.reduce', 'Array.prototype.reduce')}}</td>
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
   <th>Edge</th>
   <th>Firefox (Gecko)</th>
   <th>Internet Explorer</th>
   <th>Opera</th>
   <th>Safari</th>
  </tr>
  <tr>
   <td>Basic support</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatGeckoDesktop("1.9")}}</td>
   <td>{{CompatIE("9")}}</td>
   <td>{{CompatOpera("10.5")}}</td>
   <td>{{CompatSafari("4.0")}}</td>
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
 <li>{{jsxref("Array.prototype.reduceRight()")}}</li>
</ul>

