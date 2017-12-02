---
version: prototype1
revision_id: 1332479
locale: en-US
slug: Web/HTML/Element/canvas
tags: "HTML" "HTML5" "Web" "Canvas" "Element" "Reference" "HTML scripting"
title: <canvas>: The Graphics Canvas element
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: True
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>Use the <strong>HTML <code>&lt;canvas&gt;</code> element</strong> with either the <a href="/en-US/docs/Web/API/Canvas_API">canvas scripting API</a> or the <a href="/en-US/docs/Web/API/WebGL_API">WebGL API</a> to draw graphics and animations.</p>

<table class="properties">
 <tbody>
  <tr>
   <th scope="row"><a href="/en-US/docs/HTML/Content_categories">Content categories</a></th>
   <td><a href="/en-US/docs/HTML/Content_categories#Flow_content">Flow content</a>, <a href="/en-US/docs/HTML/Content_categories#Phrasing_content">phrasing content</a>, <a href="/en-US/docs/HTML/Content_categories#Embedded_content">embedded content</a>, palpable content.</td>
  </tr>
  <tr>
   <th scope="row">Permitted content</th>
   <td>Transparent but with no <a href="/en-US/docs/HTML/Content_categories#Interactive_content">interactive content</a> descendants except for {{HTMLElement("a")}} elements, {{HTMLElement("button")}} elements, {{HTMLElement("input")}} elements whose {{htmlattrxref("type", "input")}} attribute is <code>checkbox</code>, <code>radio</code>, or <code>button</code>.</td>
  </tr>
  <tr>
   <th scope="row">Tag omission</th>
   <td>{{no_tag_omission}}</td>
  </tr>
  <tr>
   <th scope="row">Permitted parents</th>
   <td>Any element that accepts <a href="/en-US/docs/HTML/Content_categories#Phrasing_content">phrasing content</a>.</td>
  </tr>
  <tr>
   <th scope="row">Permitted ARIA roles</th>
   <td>Any</td>
  </tr>
  <tr>
   <th scope="row">DOM interface</th>
   <td>{{domxref("HTMLCanvasElement")}}</td>
  </tr>
 </tbody>
</table>

<h2 id="Attributes">Attributes</h2>

<p>This element's attributes include the <a href="/en-US/docs/HTML/Global_attributes">global attributes</a>.</p>

<dl>
 <dt>{{htmlattrdef("height")}}</dt>
 <dd>The height of the coordinate space in CSS pixels. Defaults to 150.</dd>
 <dt>{{htmlattrdef("moz-opaque")}} {{non-standard_inline}} {{deprecated_inline}}</dt>
 <dd>Lets the canvas know whether or not translucency will be a factor. If the canvas knows there's no translucency, painting performance can be optimized. This is only supported by Mozilla-based browsers; use the standardized {{domxref("HTMLCanvasElement.getContext()", "canvas.getContext('2d', {&nbsp;alpha:&nbsp;false&nbsp;})")}} instead.</dd>
 <dt>{{htmlattrdef("width")}}</dt>
 <dd>The width of the coordinate space in CSS pixels. Defaults to 300.</dd>
</dl>

<h2 id="Usage_notes">Usage notes</h2>

<h3 id="Alternative_content">Alternative content</h3>

<p>You may (and should) provide alternate content inside the <code>&lt;canvas&gt;</code> block. That content will be rendered both on older browsers that don't support canvas and in browsers with JavaScript disabled.</p>

<h3 id="Required_&lt;canvas&gt;_tag">Required <code>&lt;/canvas&gt;</code> tag</h3>

<p>Unlike the {{HTMLElement("img")}} element, the {{HTMLElement("canvas")}} element <strong>requires</strong> the closing tag (<code>&lt;/canvas&gt;</code>).</p>

<h3 id="Sizing_the_canvas">Sizing the canvas</h3>

<p>The displayed size of the canvas can be changed using a stylesheet. The image is scaled during rendering to fit the styled size. If your renderings seem distorted, try specifying your <code>width</code> and <code>height</code> attributes explicitly in the <code>&lt;canvas&gt;</code> attributes, and not using CSS.</p>

<h2 id="Examples">Examples</h2>

<p>This code snippet adds a canvas element to your HTML document. A fallback text is provided if a browser is unable to render the canvas, or if can't read a canvas. Providing a useful fallback text or sub DOM helps to <a href="/en-US/docs/Web/API/Canvas_API/Tutorial/Hit_regions_and_accessibility">make the the canvas more accessible</a>.</p>

<pre class="brush: html">
&lt;canvas id="canvas" width="300" height="300"&gt;
  An alternative text describing what your canvas displays. 
&lt;/canvas&gt; </pre>

<p>Then in the JavaScript code, call {{domxref("HTMLCanvasElement.getContext()")}} to get a drawing context and start drawing onto the canvas:</p>

<pre class="brush: html">
&lt;script&gt;
var canvas = document.getElementById('canvas');
var ctx = canvas.getContext('2d');
ctx.fillStyle = 'green';
ctx.fillRect(10, 10, 100, 100);
&lt;/script&gt;</pre>

<h3 id="Opaque_canvas">Opaque canvas</h3>

<p>If your canvas does not use transparency, you can tell the browser that your canvas is opaque, this will be used internally to optimize rendering. To do this, set <code>alpha</code> to <code>false</code> when getting the drawing context:</p>

<pre class="brush: html">
&lt;script&gt;
var canvas = document.getElementById('canvas');
var ctx = canvas.getContext('2d', { alpha: false });
&lt;/script&gt;</pre>

<p>Before the <code>alpha</code> option was <a href="https://wiki.whatwg.org/wiki/CanvasOpaque" title="CanvasOpaque on the WHATWG wiki">standardized</a>, you could use the <code>moz-opaque</code> {{non-standard_inline}} {{deprecated_inline}} attribute on the canvas tag. However, this only works in Mozilla-based rendering engines and should be avoided; check <a href="https://bugzilla.mozilla.org/show_bug.cgi?id=878155">bug 878155</a> to track when this attribute will be removed.</p>

<pre class="brush: html">
&lt;canvas id="myCanvas" moz-opaque&gt;&lt;/canvas&gt;</pre>

<h2 id="Specifications">Specifications</h2>

<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">Specification</th>
   <th scope="col">Status</th>
   <th scope="col">Comment</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{SpecName('HTML WHATWG', 'scripting.html#the-canvas-element', '&lt;canvas&gt;')}}</td>
   <td>{{Spec2('HTML WHATWG')}}</td>
   <td>&nbsp;</td>
  </tr>
  <tr>
   <td>{{SpecName('HTML5 W3C', 'scripting-1.html#the-canvas-element', '&lt;canvas&gt;')}}</td>
   <td>{{Spec2('HTML5 W3C')}}</td>
   <td>Initial definition</td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<p class="hidden">The compatibility table in this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</p>

<p>{{Compat("html.elements.canvas")}}</p>

<h2 id="See_also">See also</h2>

<ul>
 <li><a href="/en-US/docs/Web/API/Canvas_API">MDN canvas portal</a></li>
 <li><a href="/en-US/docs/Web/API/Canvas_API/Tutorial">Canvas tutorial</a></li>
 <li><a href="https://simon.html5.org/dump/html5-canvas-cheat-sheet.html">Canvas cheat sheet</a></li>
 <li><a href="/en-US/demos/tag/tech:canvas">Canvas-related demos</a></li>
 <li><a href="https://developer.apple.com/library/safari/documentation/AudioVideo/Conceptual/HTML-canvas-guide/Introduction/Introduction.html">Canvas introduction by Apple</a></li>
</ul>

<div>{{HTMLRef}}</div>

