---
version: prototype1
revision_id: 1348366
locale: en-US
slug: Web/API/CanvasPattern
tags: "API" "Canvas" "Interface" "Reference" "Référence(2)"
title: CanvasPattern
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{APIRef("Canvas API")}}</div>

<p>The <code><strong>CanvasPattern</strong></code> interface represents an opaque object describing a pattern, based on an image, a canvas or a video, created by the {{domxref("CanvasRenderingContext2D.createPattern()")}} method.</p>

<h2 id="Properties">Properties</h2>

<p><em>Representing an opaque object, there is no exposed property.</em></p>

<h2 id="Methods">Methods</h2>

<p><em>There is no inherited method.</em></p>

<dl>
 <dt>{{domxref("CanvasPattern.setTransform()")}} {{experimental_inline}}</dt>
 <dd>Applies an {{domxref("SVGMatrix")}} representing a linear transform to the pattern.</dd>
</dl>

<h2 id="Specifications" name="Specifications">Specifications</h2>

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
   <td>{{SpecName('HTML WHATWG', "the-canvas-element.html#canvaspattern", "CanvasPattern")}}</td>
   <td>{{Spec2('HTML WHATWG')}}</td>
   <td>Added <code>setTransform()</code> method in v5.</td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<div>
<div class="hidden">The compatibility table on this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</div>

<p>{{Compat("api.CanvasPattern")}}</p>
</div>

<h2 id="See_also">See also</h2>

<ul>
 <li>{{domxref("CanvasRenderingContext2D.createPattern()")}}</li>
 <li>The {{HTMLElement("canvas")}} element and its associated interface, {{domxref("HTMLCanvasElement")}}</li>
</ul>

