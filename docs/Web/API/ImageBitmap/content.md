---
version: prototype1
revision_id: 1350726
locale: en-US
slug: Web/API/ImageBitmap
tags: "API" "Canvas" "Interface" "Reference" "ImageBitmap"
title: ImageBitmap
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{APIRef("Canvas API")}}</div>

<p>The <code><strong>ImageBitmap</strong></code> interface represents a bitmap image which can be drawn to a {{HTMLElement("canvas")}} without undue latency. It can be created from a variety of source objects using the {{domxref("ImageBitmapFactories.createImageBitmap", "createImageBitmap()")}} factory method. <code>ImageBitmap</code> provides an asynchronous and resource efficient pathway to prepare textures for rendering in WebGL.</p>

<h2 id="Properties">Properties</h2>

<dl>
 <dt>{{domxref("ImageBitmap.height")}} {{readonlyInline}}</dt>
 <dd>Is an <code>unsigned</code> <code>long</code> representing the height, in CSS pixels, of the <code>ImageData</code>.</dd>
 <dt>{{domxref("ImageBitmap.width")}} {{readonlyInline}}</dt>
 <dd>Is an <code>unsigned</code> <code>long</code> representing the width, in CSS pixels, of the <code>ImageData</code>.</dd>
</dl>

<h2 id="Methods">Methods</h2>

<dl>
 <dt>{{domxref("ImageBitmap.close()")}}</dt>
 <dd>
 <p>Disposes of all graphical resources associated with an <code>ImageBitmap</code>.</p>
 </dd>
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
   <td>{{SpecName('HTML WHATWG', "webappapis.html#imagebitmap", "ImageBitmap")}}</td>
   <td>{{Spec2('HTML WHATWG')}}</td>
   <td>&nbsp;</td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<div class="hidden">The compatibility table on this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</div>

<p>{{Compat("api.ImageBitmap")}}</p>

<h2 id="See_also">See also</h2>

<ul>
 <li>{{domxref("ImageBitmapFactories.createImageBitmap()")}}</li>
 <li>{{domxref("CanvasRenderingContext2D.drawImage()")}}</li>
 <li>{{domxref("WebGLRenderingContext.texImage2D()")}}</li>
 <li>{{domxref("OffScreenCanvas.transferToImageBitmap()")}}</li>
</ul>

