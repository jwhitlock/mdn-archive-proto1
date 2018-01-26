---
version: prototype1
revision_id: 1350730
locale: en-US
slug: Web/API/ImageBitmapRenderingContext
tags: "API" "Canvas" "Interface" "Reference" "Experimental" "OffscreenCanvas"
title: ImageBitmapRenderingContext
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{APIRef("Canvas API")}} {{SeeCompatTable}}</div>

<p>The <strong><code>ImageBitmapRenderingContext</code></strong> interface is a canvas rendering context which only provides the functionality to replace the canvas's contents with the given {{domxref("ImageBitmap")}}. Its context id (the first argument to {{domxref("HTMLCanvasElement.getContext()")}} or {{domxref("OffscreenCanvas.getContext()")}}&nbsp; is <code>"bitmaprenderer"</code>.</p>

<p>This interface is available in both, the window and the <a href="https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API">worker</a> context.</p>

<h2 id="Methods">Methods</h2>

<dl>
 <dt>{{domxref("ImageBitmapRenderingContext.transferFromImageBitmap()")}}</dt>
 <dd>
 <p>Displays the given <code>ImageBitmap</code> in the canvas associated with this rendering context. Ownership of the <code>ImageBitmap</code> is transferred to the canvas. This was previously named <code>transferImageBitmap()</code>, but was renamed in a spec change. The old name is being kept as an alias to avoid code breakage.</p>
 </dd>
</dl>

<h2 id="Specifications">Specifications</h2>

<p>{{WhyNoSpecStart}} Currently drafted as a proposal in the <a href="https://wiki.whatwg.org/wiki/OffscreenCanvas">OffscreenCanvas</a> specification.{{WhyNoSpecEnd}}</p>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<div>
<div class="hidden">The compatibility table on this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</div>

<p>{{Compat("api.ImageBitmapRenderingContext")}}</p>
</div>

<h2 id="See_also">See also</h2>

<ul>
 <li>{{domxref("OffScreenCanvas")}}</li>
</ul>

