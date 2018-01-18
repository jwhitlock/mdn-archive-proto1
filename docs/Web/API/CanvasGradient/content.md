---
version: prototype1
revision_id: 1348368
locale: en-US
slug: Web/API/CanvasGradient
tags: "API" "Canvas" "Gradients" "Interface" "Reference" "CanvasGradient"
title: CanvasGradient
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{APIRef("Canvas API")}}</div>

<p>The <code><strong>CanvasGradient</strong></code> interface represents an opaque object describing a gradient. It is returned by the methods {{domxref("CanvasRenderingContext2D.createLinearGradient()")}} or {{domxref("CanvasRenderingContext2D.createRadialGradient()")}}.</p>

<h2 id="Properties">Properties</h2>

<p><em>Representing an opaque object, there is no exposed property.</em></p>

<h2 id="Methods">Methods</h2>

<p><em>There is no inherited method.</em></p>

<dl>
 <dt>{{domxref("CanvasGradient.addColorStop()")}}</dt>
 <dd>Adds a new stop, defined by an <code>offset</code> and a <code>color</code>, to the gradient. If the offset is not between <code>0</code> and <code>1</code> an <code>INDEX_SIZE_ERR</code> is raised, if the color can't be parsed as a CSS {{cssxref("&lt;color&gt;")}}, a <code>SYNTAX_ERR</code> is raised.</dd>
</dl>

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
   <td>{{SpecName('HTML WHATWG', "the-canvas-element.html#canvasgradient", "CanvasGradient")}}</td>
   <td>{{Spec2('HTML WHATWG')}}</td>
   <td>&nbsp;</td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<div>
<div class="hidden">The compatibility table on this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</div>

<p>{{Compat("api.CanvasGradient")}}</p>
</div>

<h2 id="See_also">See also</h2>

<ul>
 <li>Creator methods in {{domxref("CanvasRenderingContext2D")}}.</li>
 <li>The {{HTMLElement("canvas")}} element and its associated interface, {{domxref("HTMLCanvasElement")}}.</li>
</ul>

