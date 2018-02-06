---
version: prototype1
revision_id: 1355275
locale: en-US
slug: Web/API/TextMetrics
tags: "API" "Canvas" "Reference" "Référence(2)" "TextMetrics"
title: TextMetrics
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{APIRef("Canvas API")}}</div>

<p>The <strong><code>TextMetrics</code></strong> interface represents the dimension of a text in the canvas, as created by the {{domxref("CanvasRenderingContext2D.measureText()")}} method.</p>

<h2 id="Properties">Properties</h2>

<dl>
 <dt>{{domxref("TextMetrics.width")}} {{readonlyInline}}</dt>
 <dd>Is a <code>double</code> giving the calculated width of a segment of inline text in CSS pixels. It takes into account the current font of the context.</dd>
 <dt>{{domxref("TextMetrics.actualBoundingBoxLeft")}} {{readonlyInline}}</dt>
 <dd>Is a <code>double</code> giving the distance parallel to the baseline from the alignment point given by the {{domxref("CanvasRenderingContext2D.textAlign")}} property to the left side of the bounding rectangle of the given text, in CSS pixels.</dd>
 <dt>{{domxref("TextMetrics.actualBoundingBoxRight")}} {{readonlyInline}}</dt>
 <dd>Is a <code>double</code> giving the distance parallel to the baseline from the alignment point given by the {{domxref("CanvasRenderingContext2D.textAlign")}} property to the right side of the bounding rectangle of the given text, in CSS pixels.</dd>
 <dt>{{domxref("TextMetrics.fontBoundingBoxAscent")}} {{readonlyInline}}</dt>
 <dd>Is a <code>double</code> giving the distance from the horizontal line indicated by the {{domxref("CanvasRenderingContext2D.textBaseline")}} attribute to the top of the highest bounding rectangle of all the fonts used to render the text, in CSS pixels.</dd>
 <dt>{{domxref("TextMetrics.fontBoundingBoxDescent")}} {{readonlyInline}}</dt>
 <dd>Is a <code>double</code> giving the distance from the horizontal line indicated by the {{domxref("CanvasRenderingContext2D.textBaseline")}} attribute to the bottom of the bounding rectangle of all the fonts used to render the text, in CSS pixels.</dd>
 <dt>{{domxref("TextMetrics.actualBoundingBoxAscent")}} {{readonlyInline}}</dt>
 <dd>Is a <code>double</code> giving the distance from the horizontal line indicated by the {{domxref("CanvasRenderingContext2D.textBaseline")}} attribute to the top of the bounding rectangle used to render the text, in CSS pixels.</dd>
 <dt>{{domxref("TextMetrics.actualBoundingBoxDescent")}} {{readonlyInline}}</dt>
 <dd>Is a <code>double</code> giving the distance from the horizontal line indicated by the {{domxref("CanvasRenderingContext2D.textBaseline")}} attribute to the bottom of the bounding rectangle used to render the text, in CSS pixels.</dd>
 <dt>{{domxref("TextMetrics.emHeightAscent")}} {{readonlyInline}}</dt>
 <dd>Is a <code>double</code> giving the distance from the horizontal line indicated by the {{domxref("CanvasRenderingContext2D.textBaseline")}} property to the top of the <em>em</em> square in the line box, in CSS pixels.</dd>
 <dt>{{domxref("TextMetrics.emHeightDescent")}} {{readonlyInline}}</dt>
 <dd>Is a <code>double</code> giving the distance from the horizontal line indicated by the {{domxref("CanvasRenderingContext2D.textBaseline")}} property to the bottom of the <em>em</em> square in the line box, in CSS pixels.</dd>
 <dt>{{domxref("TextMetrics.hangingBaseline")}} {{readonlyInline}}</dt>
 <dd>Is a <code>double</code> giving the distance from the horizontal line indicated by the {{domxref("CanvasRenderingContext2D.textBaseline")}} property to the hanging baseline of the line box, in CSS pixels.</dd>
 <dt>{{domxref("TextMetrics.alphabeticBaseline")}} {{readonlyInline}}</dt>
 <dd>Is a <code>double</code> giving the distance from the horizontal line indicated by the {{domxref("CanvasRenderingContext2D.textBaseline")}} property to the alphabetic baseline of the line box, in CSS pixels.</dd>
 <dt>{{domxref("TextMetrics.ideographicBaseline")}} {{readonlyInline}}</dt>
 <dd>Is a <code>double</code> giving the distance from the horizontal line indicated by the {{domxref("CanvasRenderingContext2D.textBaseline")}} property to the ideographic baseline of the line box, in CSS pixels.</dd>
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
   <td>{{SpecName('HTML WHATWG', "the-canvas-element.html#textmetrics", "TextMetrics")}}</td>
   <td>{{Spec2('HTML WHATWG')}}</td>
   <td>Initial definition</td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<div>
<div class="hidden">The compatibility table on this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</div>

<p>{{Compat("api.TextMetrics")}}</p>
</div>

<h2 id="See_also">See also</h2>

<ul>
 <li>Creator method in {{domxref("CanvasRenderingContext2D")}}.</li>
 <li>The {{HTMLElement("canvas")}} element and its associated interface, {{domxref("HTMLCanvasElement")}}</li>
</ul>

