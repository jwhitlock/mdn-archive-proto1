---
version: prototype1
revision_id: 1350732
locale: en-US
slug: Web/API/ImageData
tags: "API" "Canvas" "Images" "ImageData"
title: ImageData
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{APIRef("Canvas API")}}</div>

<p>The <code><strong>ImageData</strong></code> interface represents the underlying pixel data of an area of a {{HTMLElement("canvas")}} element. It is created using the {{domxref("ImageData.ImageData", "ImageData()")}} constructor or creator methods on the {{domxref("CanvasRenderingContext2D")}} object associated with a canvas: {{domxref("CanvasRenderingContext2D.createImageData", "createImageData()")}} and {{domxref("CanvasRenderingContext2D.getImageData", "getImageData()")}}. It can also be used to set a part of the canvas by using {{domxref("CanvasRenderingContext2D.putImageData", "putImageData()")}}.</p>

<h2 id="Constructors">Constructors</h2>

<dl>
 <dt>{{domxref("ImageData.ImageData", "ImageData()")}} {{experimental_inline}}</dt>
 <dd>Creates an <code>ImageData</code> object from a given {{jsxref("Uint8ClampedArray")}} and the size of the image it contains. If no array is given, it creates an image of a black rectangle. Note that this is the most common way to create such an object in workers as {{domxref("CanvasRenderingContext2D.createImageData", "createImageData()")}} is not available there.</dd>
</dl>

<h2 id="Properties">Properties</h2>

<dl>
 <dt>{{domxref("ImageData.data")}} {{readonlyInline}}</dt>
 <dd>Is a {{jsxref("Uint8ClampedArray")}} representing a one-dimensional array containing the data in the RGBA order, with integer values between <code>0</code> and <code>255</code> (included).</dd>
 <dt>{{domxref("ImageData.height")}} {{readonlyInline}}</dt>
 <dd>Is an <code>unsigned</code> <code>long</code> representing the actual height, in pixels, of the <code>ImageData</code>.</dd>
 <dt>{{domxref("ImageData.width")}} {{readonlyInline}}</dt>
 <dd>Is an <code>unsigned</code> <code>long</code> representing the actual width, in pixels, of the <code>ImageData</code>.</dd>
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
   <td>{{SpecName('HTML WHATWG', "the-canvas-element.html#imagedata", "ImageData")}}</td>
   <td>{{Spec2('HTML WHATWG')}}</td>
   <td>&nbsp;</td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<div>
<div class="hidden">The compatibility table on this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</div>

<p>{{Compat("api.ImageData")}}</p>
</div>

<h2 id="See_also">See also</h2>

<ul>
 <li>{{domxref("CanvasRenderingContext2D")}}</li>
 <li>The {{HTMLElement("canvas")}} element and its associated interface, {{domxref("HTMLCanvasElement")}}.</li>
</ul>

