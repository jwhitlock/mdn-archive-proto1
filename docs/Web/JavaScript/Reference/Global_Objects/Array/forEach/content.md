---
version: prototype1
revision_id: 1337009
locale: en-US
slug: Web/JavaScript/Reference/Global_Objects/Array/forEach
tags: "Array" "ECMAScript 5" "Method" "JavaScript" "Prototype" "Reference"
title: Array.prototype.forEach()
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{JSRef}}</div>

<p>The <code><strong>forEach()</strong></code> method executes a provided function once for each array element.</p>

<pre class="brush: js">
const arr = ['a', 'b', 'c'];

arr.forEach(function(element) {
    console.log(element);
});

// a
// b
// c</pre>

<h2 id="Syntax">Syntax</h2>

<pre class="syntaxbox">
<var>arr</var>.forEach(function <var>callback(currentValue[, index[, array]]) {
    //your iterator
}</var>[, <var>thisArg</var>]);</pre>

<h3 id="Parameters">Parameters</h3>

<dl>
 <dt><code>callback</code></dt>
 <dd>Function to execute for each element, taking three arguments:
 <dl>
  <dt><code>currentValue</code></dt>
  <dd>The value of the current element being processed in the array.</dd>
  <dt><code>index</code>{{optional_inline}}</dt>
  <dd>The index of the current element being processed in the array.</dd>
  <dt><code>array</code>{{optional_inline}}</dt>
  <dd>The array that&nbsp;<code>forEach()</code> is being applied to.</dd>
 </dl>
 </dd>
 <dt><code>thisArg</code> {{Optional_inline}}</dt>
 <dd>
 <p>Value to use as <code><strong>this</strong></code> (i.e the reference <code>Object</code>) when executing <code>callback</code>.</p>
 </dd>
</dl>

<h3 id="Return_value">Return value</h3>

<p>{{jsxref("undefined")}}.</p>

<h2 id="Description">Description</h2>

<p><code>forEach()</code> executes the provided <code>callback</code> once for each element present in the array in ascending order. It is not invoked for index properties that have been deleted or are uninitialized (i.e. on sparse arrays).</p>

<p><code>callback</code> is invoked with <strong>three arguments</strong>:</p>

<ul>
 <li>the <strong>element value</strong></li>
 <li>the <strong>element index</strong></li>
 <li>the <strong>array being traversed</strong></li>
</ul>

<p>If a <code>thisArg</code> parameter is provided to <code>forEach()</code>, it will be used as callback's&nbsp;<code>this</code> value.&nbsp; Otherwise, the value {{jsxref("undefined")}} will be used as its <code>this</code> value. The <code>this</code> value ultimately observable by <code>callback</code> is determined according to <a href="/en-US/docs/Web/JavaScript/Reference/Operators/this">the usual rules for determining the <code>this</code> seen by a function</a>.</p>

<p>The range of elements processed by <code>forEach()</code> is set before the first invocation of <code>callback</code>. Elements that are appended to the array after the call to <code>forEach()</code> begins will not be visited by <code>callback</code>. If the values of existing elements of the array are changed, the value passed to <code>callback</code> will be the value at the time <code>forEach()</code> visits them; elements that are deleted before being visited are not visited. If elements that are already visited are removed (e.g. using {{jsxref("Array.prototype.shift()", "shift()")}}) during the iteration, later elements will be skipped - see example below.</p>

<p><code>forEach()</code> executes the <code>callback</code> function once for each array element; unlike {{jsxref("Array.prototype.map()", "map()")}} or {{jsxref("Array.prototype.reduce()", "reduce()")}} it always returns the value {{jsxref("undefined")}} and is not chainable. The typical use case is to execute side effects at the end of a chain.</p>

<p><code>forEach()</code>&nbsp;does not mutate the array on which it is called (although&nbsp;<code>callback</code>, if invoked, may do so).</p>

<div class="note">
<p>There is no way to stop or break a <code>forEach()</code> loop other than by throwing an exception. If you need such behavior, the <code>forEach()</code> method is the wrong tool.&nbsp;Use a plain loop instead. If you are testing the array elements for a predicate and need a Boolean return value, you can use {{jsxref("Array.prototype.every()", "every()")}} or {{jsxref("Array.prototype.some()", "some()")}} instead. If available, the new methods {{jsxref("Array.prototype.find()", "find()")}} or {{jsxref("Array.prototype.findIndex()", "findIndex()")}} can be used for early termination upon true predicates as well.</p>
</div>

<h2 id="Examples">Examples</h2>

<h3 id="Converting_from_for_to_forEach">Converting from for to forEach</h3>

<p>before</p>

<pre class="brush:js">
const items = ['item1', 'item2', 'item3'];
const copy = [];

for (let i=0; i&lt;items.length; i++) {
  copy.push(items[i])
}
</pre>

<p>after</p>

<pre class="brush:js">
const items = ['item1', 'item2', 'item3'];
const copy = [];

items.forEach(function(item){
  copy.push(item)
});

</pre>

<p>&nbsp;</p>

<h3 id="Printing_the_contents_of_an_array">Printing the contents of an array</h3>

<p>The following code logs a line for each element in an array:</p>

<pre class="brush:js">
function logArrayElements(element, index, array) {
  console.log('a[' + index + '] = ' + element);
}

// Notice that index 2 is skipped since there is no item at
// that position in the array.
[2, 5, , 9].forEach(logArrayElements);
// logs:
// a[0] = 2
// a[1] = 5
// a[3] = 9
</pre>

<h3 id="Using_thisArg">Using <code>thisArg</code></h3>

<p>The following (contrived) example updates an object's properties from each entry in the array:</p>

<pre class="brush:js">
function Counter() {
  this.sum = 0;
  this.count = 0;
}
Counter.prototype.add = function(array) {
  array.forEach(function(entry) {
    this.sum += entry;
    ++this.count;
  }, this);
  // ^---- Note
};

const obj = new Counter();
obj.add([2, 5, 9]);
obj.count;
// 3 
obj.sum;
// 16
</pre>

<p>Since the&nbsp;<code>thisArg</code>&nbsp;parameter (<code>this</code>) is provided to&nbsp;<code>forEach()</code>, it is passed to&nbsp;<code>callback</code> each time it's invoked, for use as its&nbsp;<code>this</code>&nbsp;value.</p>

<div class="note">
<p>If passing the function argument using an <a href="/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions">arrow function expression</a> the <code>thisArg</code> parameter can be omitted as arrow functions lexically bind the {{jsxref("Operators/this", "this")}} value.</p>
</div>

<h3 id="An_object_copy_function">An object copy function</h3>

<p>The following code creates a copy of a given object. There are different ways to create a copy of an object;&nbsp;the following is just one way and is presented to explain how <code>Array.prototype.forEach()</code> works by using ECMAScript 5 <code>Object.*</code> meta property functions.</p>

<pre class="brush: js">
function copy(obj) {
  const copy = Object.create(Object.getPrototypeOf(obj));
  const propNames = Object.getOwnPropertyNames(obj);

  propNames.forEach(function(name) {
    const desc = Object.getOwnPropertyDescriptor(obj, name);
    Object.defineProperty(copy, name, desc);
  });

  return copy;
}

const obj1 = { a: 1, b: 2 };
const obj2 = copy(obj1); // obj2 looks like obj1 now
</pre>

<h3 id="If_the_array_is_modified_during_iteration_other_elements_might_be_skipped.">If the array is modified during iteration, other elements might be skipped.</h3>

<p>The following example logs "one", "two", "four". When the entry containing the value "two" is reached, the first entry of the whole array is shifted off, which results in all remaining entries moving up one position. Because element "four" is now at an earlier position in the array, "three" will be skipped. <code>forEach()</code> does not make a copy of the array before iterating.</p>

<pre class="brush:js">
var words = ['one', 'two', 'three', 'four'];
words.forEach(function(word) {
  console.log(word);
  if (word === 'two') {
    words.shift();
  }
});
// one
// two
// four
</pre>

<h2 id="Polyfill">Polyfill</h2>

<p><code>forEach()</code> was added to the ECMA-262 standard in the 5th edition; as such it may not be present in other implementations of the standard. You can work around this by inserting the following code at the beginning of your scripts, allowing use of <code>forEach()</code> in implementations that don't natively support it. This algorithm is exactly the one specified in ECMA-262, 5th edition, assuming {{jsxref("Object")}} and {{jsxref("TypeError")}} have their original values and that <code>callback.call()</code> evaluates to the original value of {{jsxref("Function.prototype.call()")}}.</p>

<pre class="brush: js">
// Production steps of ECMA-262, Edition 5, 15.4.4.18
// Reference: http://es5.github.io/#x15.4.4.18
if (!Array.prototype.forEach) {

  Array.prototype.forEach = function(callback/*, thisArg*/) {

    var T, k;

    if (this == null) {
      throw new TypeError('this is null or not defined');
    }

    // 1. Let O be the result of calling toObject() passing the
    // |this| value as the argument.
    var O = Object(this);

    // 2. Let lenValue be the result of calling the Get() internal
    // method of O with the argument "length".
    // 3. Let len be toUint32(lenValue).
    var len = O.length &gt;&gt;&gt; 0;

    // 4. If isCallable(callback) is false, throw a TypeError exception. 
    // See: http://es5.github.com/#x9.11
    if (typeof callback !== 'function') {
      throw new TypeError(callback + ' is not a function');
    }

    // 5. If thisArg was supplied, let T be thisArg; else let
    // T be undefined.
    if (arguments.length &gt; 1) {
      T = arguments[1];
    }

    // 6. Let k be 0.
    k = 0;

    // 7. Repeat while k &lt; len.
    while (k &lt; len) {

      var kValue;

      // a. Let Pk be ToString(k).
      //    This is implicit for LHS operands of the in operator.
      // b. Let kPresent be the result of calling the HasProperty
      //    internal method of O with argument Pk.
      //    This step can be combined with c.
      // c. If kPresent is true, then
      if (k in O) {

        // i. Let kValue be the result of calling the Get internal
        // method of O with argument Pk.
        kValue = O[k];

        // ii. Call the Call internal method of callback with T as
        // the this value and argument list containing kValue, k, and O.
        callback.call(T, kValue, k, O);
      }
      // d. Increase k by 1.
      k++;
    }
    // 8. return undefined.
  };
}
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
   <td>{{SpecName('ES5.1', '#sec-15.4.4.18', 'Array.prototype.forEach')}}</td>
   <td>{{Spec2('ES5.1')}}</td>
   <td>Initial definition. Implemented in JavaScript 1.6.</td>
  </tr>
  <tr>
   <td>{{SpecName('ES6', '#sec-array.prototype.foreach', 'Array.prototype.forEach')}}</td>
   <td>{{Spec2('ES6')}}</td>
   <td>&nbsp;</td>
  </tr>
  <tr>
   <td>{{SpecName('ESDraft', '#sec-array.prototype.foreach', 'Array.prototype.forEach')}}</td>
   <td>{{Spec2('ESDraft')}}</td>
   <td>&nbsp;</td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<div>
<div class="hidden">The compatibility table in this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</div>

<p>{{Compat("javascript.builtins.Array.forEach")}}</p>
</div>

<h2 id="See_also">See also</h2>

<ul>
 <li>{{jsxref("Array.prototype.find()")}}</li>
 <li>{{jsxref("Array.prototype.findIndex()")}}</li>
 <li>{{jsxref("Array.prototype.map()")}}</li>
 <li>{{jsxref("Array.prototype.every()")}}</li>
 <li>{{jsxref("Array.prototype.some()")}}</li>
 <li>{{jsxref("Map.prototype.forEach()")}}</li>
 <li>{{jsxref("Set.prototype.forEach()")}}</li>
</ul>

