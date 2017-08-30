---
version: prototype1
revision_id: 1296595
locale: en-US
slug: Web/JavaScript/Reference/Global_Objects
tags: "JavaScript" "Reference"
title: Standard built-in objects
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{jsSidebar("Objects")}}</div>

<p>This chapter documents all of JavaScript's standard, built-in objects, including their methods and properties.</p>

<p>The term "global objects" (or standard built-in objects) here is not to be confused with the <strong>global object</strong>. Here, global objects refer to <strong>objects in the global scope</strong>. The <strong>global object</strong> itself can be accessed using the {{jsxref("Operators/this", "this")}} operator in the global scope (but only if ECMAScript 5 strict mode is not used; in that case it returns {{jsxref("undefined")}}). In fact, the global scope <strong>consists of</strong> the properties of the global object, including inherited properties, if any.</p>

<p>Other objects in the global scope are either <a href="/en-US/docs/Web/JavaScript/Guide/Working_with_Objects#Creating_new_objects">created by the user script</a> or provided by the host application. The host objects available in browser contexts are documented in the <a href="/en-US/docs/Web/API/Reference">API reference</a>. For more information about the distinction between the <a href="/en-US/docs/DOM/DOM_Reference">DOM</a> and core <a href="/en-US/docs/Web/JavaScript">JavaScript</a>, see <a href="/en-US/docs/Web/JavaScript/JavaScript_technologies_overview">JavaScript technologies overview</a>.</p>

<h2 id="Standard_objects_by_category">Standard objects by category</h2>

<h3 id="Value_properties">Value properties</h3>

<p>These global properties return a simple value; they have no properties or methods.</p>

<ul>
 <li>{{jsxref("Infinity")}}</li>
 <li>{{jsxref("NaN")}}</li>
 <li>{{jsxref("undefined")}}</li>
 <li>{{jsxref("null")}} literal</li>
</ul>

<h3 id="Function_properties">Function properties</h3>

<p>These global functions—functions which are called globally rather than on an object—directly return their results to the caller.</p>

<ul>
 <li>{{jsxref("Global_Objects/eval", "eval()")}}</li>
 <li>{{jsxref("Global_Objects/uneval", "uneval()")}} {{non-standard_inline}}</li>
 <li>{{jsxref("Global_Objects/isFinite", "isFinite()")}}</li>
 <li>{{jsxref("Global_Objects/isNaN", "isNaN()")}}</li>
 <li>{{jsxref("Global_Objects/parseFloat", "parseFloat()")}}</li>
 <li>{{jsxref("Global_Objects/parseInt", "parseInt()")}}</li>
 <li>{{jsxref("Global_Objects/decodeURI", "decodeURI()")}}</li>
 <li>{{jsxref("Global_Objects/decodeURIComponent", "decodeURIComponent()")}}</li>
 <li>{{jsxref("Global_Objects/encodeURI", "encodeURI()")}}</li>
 <li>{{jsxref("Global_Objects/encodeURIComponent", "encodeURIComponent()")}}</li>
 <li>{{jsxref("Global_Objects/escape", "escape()")}} {{deprecated_inline}}</li>
 <li>{{jsxref("Global_Objects/unescape", "unescape()")}} {{deprecated_inline}}</li>
</ul>

<h3 id="Fundamental_objects">Fundamental objects</h3>

<p>These are the fundamental, basic objects upon which all other objects are based. This includes objects that represent general objects, functions, and errors.</p>

<ul>
 <li>{{jsxref("Object")}}</li>
 <li>{{jsxref("Function")}}</li>
 <li>{{jsxref("Boolean")}}</li>
 <li>{{jsxref("Symbol")}}</li>
 <li>{{jsxref("Error")}}</li>
 <li>{{jsxref("EvalError")}}</li>
 <li>{{jsxref("InternalError")}}</li>
 <li>{{jsxref("RangeError")}}</li>
 <li>{{jsxref("ReferenceError")}}</li>
 <li>{{jsxref("SyntaxError")}}</li>
 <li>{{jsxref("TypeError")}}</li>
 <li>{{jsxref("URIError")}}</li>
</ul>

<h3 id="Numbers_and_dates">Numbers and dates</h3>

<p>These are the base objects representing numbers, dates, and mathematical calculations.</p>

<ul>
 <li>{{jsxref("Number")}}</li>
 <li>{{jsxref("Math")}}</li>
 <li>{{jsxref("Date")}}</li>
</ul>

<h3 id="Text_processing">Text processing</h3>

<p>These objects represent strings and support manipulating them.</p>

<ul>
 <li>{{jsxref("String")}}</li>
 <li>{{jsxref("RegExp")}}</li>
</ul>

<h3 id="Indexed_collections">Indexed collections</h3>

<p>These objects represent collections of data which are ordered by an index value. This includes (typed) arrays and array-like constructs.</p>

<ul>
 <li>{{jsxref("Array")}}</li>
 <li>{{jsxref("Int8Array")}}</li>
 <li>{{jsxref("Uint8Array")}}</li>
 <li>{{jsxref("Uint8ClampedArray")}}</li>
 <li>{{jsxref("Int16Array")}}</li>
 <li>{{jsxref("Uint16Array")}}</li>
 <li>{{jsxref("Int32Array")}}</li>
 <li>{{jsxref("Uint32Array")}}</li>
 <li>{{jsxref("Float32Array")}}</li>
 <li>{{jsxref("Float64Array")}}</li>
</ul>

<h3 id="Keyed_collections">Keyed collections</h3>

<p>These objects represent collections which use keys; these contain elements which are iterable in the order of insertion.</p>

<ul>
 <li>{{jsxref("Map")}}</li>
 <li>{{jsxref("Set")}}</li>
 <li>{{jsxref("WeakMap")}}</li>
 <li>{{jsxref("WeakSet")}}</li>
</ul>

<h3 id="Vector_collections">Vector collections</h3>

<p>{{Glossary("SIMD")}} vector data types are objects where data is arranged into lanes.</p>

<ul>
 <li>{{jsxref("SIMD")}} {{experimental_inline}}</li>
 <li>{{jsxref("Float32x4", "SIMD.Float32x4")}} {{experimental_inline}}</li>
 <li>{{jsxref("Float64x2", "SIMD.Float64x2")}} {{experimental_inline}}</li>
 <li>{{jsxref("Int8x16", "SIMD.Int8x16")}} {{experimental_inline}}</li>
 <li>{{jsxref("Int16x8", "SIMD.Int16x8")}} {{experimental_inline}}</li>
 <li>{{jsxref("Int32x4", "SIMD.Int32x4")}} {{experimental_inline}}</li>
 <li>{{jsxref("Uint8x16", "SIMD.Uint8x16")}} {{experimental_inline}}</li>
 <li>{{jsxref("Uint16x8", "SIMD.Uint16x8")}} {{experimental_inline}}</li>
 <li>{{jsxref("Uint32x4", "SIMD.Uint32x4")}} {{experimental_inline}}</li>
 <li>{{jsxref("Bool8x16", "SIMD.Bool8x16")}} {{experimental_inline}}</li>
 <li>{{jsxref("Bool16x8", "SIMD.Bool16x8")}} {{experimental_inline}}</li>
 <li>{{jsxref("Bool32x4", "SIMD.Bool32x4")}} {{experimental_inline}}</li>
 <li>{{jsxref("Bool64x2", "SIMD.Bool64x2")}} {{experimental_inline}}</li>
</ul>

<h3 id="Structured_data">Structured data</h3>

<p>These objects represent and interact with structured data buffers and data coded using JavaScript Object Notation (JSON).</p>

<ul>
 <li>{{jsxref("ArrayBuffer")}}</li>
 <li>{{jsxref("SharedArrayBuffer")}} {{experimental_inline}}</li>
 <li>{{jsxref("Atomics")}} {{experimental_inline}}</li>
 <li>{{jsxref("DataView")}}</li>
 <li>{{jsxref("JSON")}}</li>
</ul>

<h3 id="Control_abstraction_objects">Control abstraction objects</h3>

<ul>
 <li>{{jsxref("Promise")}}</li>
 <li>{{jsxref("Generator")}}</li>
 <li>{{jsxref("GeneratorFunction")}}</li>
 <li>{{experimental_inline}} {{jsxref("AsyncFunction")}}</li>
</ul>

<h3 id="Reflection">Reflection</h3>

<ul>
 <li>{{jsxref("Reflect")}}</li>
 <li>{{jsxref("Proxy")}}</li>
</ul>

<h3 id="Internationalization">Internationalization</h3>

<p>Additions to the ECMAScript core for language-sensitive functionalities.</p>

<ul>
 <li>{{jsxref("Intl")}}</li>
 <li>{{jsxref("Global_Objects/Collator", "Intl.Collator")}}</li>
 <li>{{jsxref("Global_Objects/DateTimeFormat", "Intl.DateTimeFormat")}}</li>
 <li>{{jsxref("Global_Objects/NumberFormat", "Intl.NumberFormat")}}</li>
</ul>

<h3 id="WebAssembly">WebAssembly</h3>

<ul>
 <li>{{jsxref("WebAssembly")}}</li>
 <li>{{jsxref("WebAssembly.Module")}}</li>
 <li>{{jsxref("WebAssembly.Instance")}}</li>
 <li>{{jsxref("WebAssembly.Memory")}}</li>
 <li>{{jsxref("WebAssembly.Table")}}</li>
 <li>{{jsxref("WebAssembly.CompileError")}}</li>
 <li>{{jsxref("WebAssembly.LinkError")}}</li>
 <li>{{jsxref("WebAssembly.RuntimeError")}}</li>
</ul>

<h3 id="Other">Other</h3>

<ul>
 <li><code><a href="/en-US/docs/Web/JavaScript/Reference/Functions/arguments">arguments</a></code></li>
</ul>

