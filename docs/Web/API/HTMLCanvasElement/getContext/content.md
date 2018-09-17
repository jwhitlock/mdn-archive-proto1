---
version: prototype1
revision_id: 1367329
locale: en-US
slug: Web/API/HTMLCanvasElement/getContext
tags: "API" "Canvas" "Method" "Reference" "HTMLCanvasElement"
title: HTMLCanvasElement.getContext()
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{APIRef("Canvas API")}}</div>

<p class="summary">The <strong><code>HTMLCanvasElement.getContext()</code></strong> method returns a drawing context on the canvas, or {{jsxref("null")}} if the context identifier is not supported.</p>

<h2 id="Syntax">Syntax</h2>

<pre class="syntaxbox">
var <em>ctx</em> = <em>canvas</em>.getContext(<em>contextType</em>);
var <em>ctx</em> = <em>canvas</em>.getContext(<em>contextType</em>, <em>contextAttributes</em>);
</pre>

<h3 id="Parameters">Parameters</h3>

<dl>
 <dt>contextType</dt>
 <dd>Is a {{domxref("DOMString")}} containing the context identifier defining the drawing context associated to the canvas. Possible values are:
 <ul>
  <li><code>"2d"</code>, leading to the creation of a {{domxref("CanvasRenderingContext2D")}} object representing a two-dimensional rendering context.</li>
  <li><code>"webgl"</code> (or <code>"experimental-webgl"</code>) which will create a {{domxref("WebGLRenderingContext")}} object representing a three-dimensional rendering context. This context is only available on browsers that implement <a href="https://developer.mozilla.org/en-US/docs/Web/WebGL">WebGL</a> version 1 (OpenGL ES 2.0).</li>
  <li><code>"webgl2"</code> which will create a {{domxref("WebGL2RenderingContext")}} object representing a three-dimensional rendering context. This context is only available on browsers that implement <a href="https://developer.mozilla.org/en-US/docs/Web/WebGL">WebGL</a> version 2 (OpenGL ES 3.0). {{experimental_inline}}</li>
  <li><code>"bitmaprenderer"</code> which will create an {{domxref("ImageBitmapRenderingContext")}} which only provides functionality to replace the content of the canvas with a given {{domxref("ImageBitmap")}}.</li>
 </ul>

 <div class="note">
 <p><strong>Note</strong>: The identifier "<code>experimental-webgl</code>" is used in new implementations of WebGL. These implementations have either not reached test suite conformance, or the graphic drivers on the platform are not yet stable. The <a href="https://www.khronos.org/">Khronos Group</a> certifies WebGL implementations under certain <a href="https://www.khronos.org/registry/webgl/sdk/tests/CONFORMANCE_RULES.txt">conformance rules</a>.</p>
 </div>
 </dd>
 <dt><code>contextAttributes</code></dt>
 <dd>
 <p>You can use several context attributes when creating your rendering context, for example:</p>

 <pre class="brush: js">
const gl = canvas.getContext('webgl', {
  antialias: false,
  depth: false
});</pre>
 2d context attributes:

 <ul>
  <li><strong><code>alpha</code></strong>: Boolean that indicates if the canvas contains an alpha channel. If set to <code>false</code>, the browser now knows that the backdrop is always opaque, which can speed up drawing of transparent content and images.</li>
  <li>{{non-standard_inline}} (Gecko only) <strong><code>willReadFrequently</code></strong>: Boolean that indicates whether or not a lot of read-back operations are planned. This will force the use of a software (instead of hardware accelerated) 2D canvas and can save memory when calling {{domxref("CanvasRenderingContext2D.getImageData", "getImageData()")}} frequently. This option is only available, if the flag <code>gfx.canvas.willReadFrequently.enable</code> is set to <code>true</code> (which, by default, is only the case for B2G/Firefox OS).</li>
  <li>{{non-standard_inline}} (Blink only) <strong><code>storage</code></strong>: String that indicates which storage is used ("persistent" by default).</li>
 </ul>
 WebGL context attributes:

 <ul>
  <li><strong><code>alpha</code></strong>: Boolean that indicates if the canvas contains an alpha buffer.</li>
  <li><strong><code>depth</code></strong>: Boolean that indicates that the drawing buffer has a depth buffer of at least 16 bits.</li>
  <li><strong><code>stencil</code></strong>: Boolean that indicates that the drawing buffer has a stencil buffer of at least 8 bits.</li>
  <li><strong><code>antialias</code></strong>: Boolean that indicates whether or not to perform anti-aliasing.</li>
  <li><strong><code>premultipliedAlpha</code></strong>: Boolean that indicates that the page compositor will assume the drawing buffer contains colors with pre-multiplied alpha.</li>
  <li><strong><code>preserveDrawingBuffer</code></strong>: If the value is true the buffers will not be cleared and will preserve their values until cleared or overwritten by the author.</li>
  <li><code><strong>failIfMajorPerformanceCaveat</strong></code>: Boolean that indicates if a context will be created if the system performance is low.</li>
 </ul>
 </dd>
</dl>

<h3 id="Return_value">Return value</h3>

<p>A {{domxref("RenderingContext")}} which is either a</p>

<ul>
 <li>{{domxref("CanvasRenderingContext2D")}} for <code>"2d"</code>,</li>
 <li>{{domxref("WebGLRenderingContext")}} for <code>"webgl"</code> and <code>"experimental-webgl"</code>,</li>
 <li>{{domxref("WebGL2RenderingContext")}} for <code>"webgl2"</code>&nbsp;or</li>
 <li>{{domxref("ImageBitmapRenderingContext")}} for <code>"bitmaprenderer"</code>.</li>
</ul>

<p>If the <em>contextType</em> doesn't match a possible drawing context, <code>null</code> is returned.</p>

<h2 id="Examples">Examples</h2>

<p>Given this {{HTMLElement("canvas")}} element:</p>

<pre class="brush: html">
&lt;canvas id="canvas" width="300" height="300"&gt;&lt;/canvas&gt;
</pre>

<p>You can get a <code>2d</code> context of the canvas with the following code:</p>

<pre class="brush: js">
var canvas = document.getElementById('canvas');
var ctx = canvas.getContext('2d');
console.log(ctx); // CanvasRenderingContext2D { ... }
</pre>

<p>Now you have the <a href="/en-US/docs/Web/API/CanvasRenderingContext2D">2D rendering context</a> for a canvas and you can draw within it.</p>

<h2 id="Specifications">Specifications</h2>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="col">Specification</th>
   <th scope="col">Status</th>
   <th scope="col">Comment</th>
  </tr>
  <tr>
   <td>{{SpecName('HTML WHATWG', "scripting.html#dom-canvas-getcontext", "HTMLCanvasElement.getContext")}}</td>
   <td>{{Spec2('HTML WHATWG')}}</td>
   <td>No change since the latest snapshot, {{SpecName('HTML5 W3C')}}</td>
  </tr>
  <tr>
   <td>{{SpecName('HTML5.1', "scripting-1.html#dom-canvas-getcontext", "HTMLCanvasElement.getContext")}}</td>
   <td>{{Spec2('HTML5.1')}}</td>
   <td>&nbsp;</td>
  </tr>
  <tr>
   <td>{{SpecName('HTML5 W3C', "scripting-1.html#dom-canvas-getcontext", "HTMLCanvasElement.getContext")}}</td>
   <td>{{Spec2('HTML5 W3C')}}</td>
   <td>Snapshot of the {{SpecName('HTML WHATWG')}} containing the initial definition.</td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<div class="hidden">The compatibility table on this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</div>

<p>{{Compat("api.HTMLCanvasElement.getContext")}}</p>

<h2 id="See_also">See also</h2>

<ul>
 <li>The interface defining it, {{domxref("HTMLCanvasElement")}}.</li>
 <li>{{domxref("OffscreenCanvas.getContext()")}}</li>
 <li>Available rendering contexts: {{domxref("CanvasRenderingContext2D")}}, {{domxref("WebGLRenderingContext")}} and {{domxref("WebGL2RenderingContext")}} and&nbsp;{{domxref("ImageBitmapRenderingContext")}}.</li>
</ul>
