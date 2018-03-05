---
version: prototype1
revision_id: 1364563
locale: en-US
slug: Web/API/ImageBitmapFactories
tags: "API" "Mixin" "Canvas" "Workers" "Obsolete" "Interface" "Reference"
title: ImageBitmapFactories
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{APIRef("")}}</div>

<div class="warning">
<p><strong>Important</strong>: As of Firefox 52, the method defined in this mixin has been moved to the {{domxref("WindowOrWorkerGlobalScope")}} mixin, and other browsers will follow suit. Look to that page for up-to-date details.</p>
</div>

<p>The <code><strong>ImageBitmapFactories</strong></code> mixin interface contains utility methods to create an {{domxref("ImageBitmap")}}. There is no object of this type, but the two interfaces {{domxref("Window")}}, available within the regular browsing scope, and the {{domxref("WorkerGlobalScope")}} interface for workers, implement this interface.</p>

<h2 id="Methods">Methods</h2>

<dl>
	<dt>{{domxref("ImageBitmapFactories.createImageBitmap()")}}</dt>
	<dd>Accepts a variety of different image sources, and returns a {{domxref("Promise")}} which resolves to an {{domxref("ImageBitmap")}}. Optionally the source is cropped to the rectangle of pixels originating at <em>(sx, sy)</em> with width sw, and height sh.</dd>
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
			<td>{{SpecName('HTML WHATWG', "webappapis.html#imagebitmapfactories", "ImageBitmapFactories")}}</td>
			<td>{{Spec2('HTML WHATWG')}}</td>
			<td>&nbsp;</td>
		</tr>
	</tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<p>{{CompatibilityTable}}</p>

<div id="compat-desktop">
<table class="compat-table">
	<tbody>
		<tr>
			<th>Feature</th>
			<th>Chrome</th>
			<th>Firefox (Gecko)</th>
			<th>Internet Explorer</th>
			<th>Opera</th>
			<th>Safari</th>
		</tr>
		<tr>
			<td>Basic support</td>
			<td>{{CompatUnknown}}</td>
			<td>{{CompatGeckoDesktop(42)}} – {{CompatGeckoDesktop(52)}}</td>
			<td>{{CompatUnknown}}</td>
			<td>{{CompatUnknown}}</td>
			<td>{{CompatUnknown}}</td>
		</tr>
	</tbody>
</table>
</div>

<div id="compat-mobile">
<table class="compat-table">
	<tbody>
		<tr>
			<th>Feature</th>
			<th>Android</th>
			<th>Chrome for Android</th>
			<th>Firefox Mobile (Gecko)</th>
			<th>IE Mobile</th>
			<th>Opera Mobile</th>
			<th>Safari Mobile</th>
		</tr>
		<tr>
			<td>Basic support</td>
			<td>{{CompatUnknown}}</td>
			<td>{{CompatUnknown}}</td>
			<td>{{CompatGeckoMobile(42)}} – {{CompatGeckoMobile(52)}}</td>
			<td>{{CompatUnknown}}</td>
			<td>{{CompatUnknown}}</td>
			<td>{{CompatUnknown}}</td>
		</tr>
	</tbody>
</table>
</div>

<h2 id="See_also">See also</h2>

<ul>
	<li>{{domxref("CanvasRenderingContext2D.drawImage()")}}</li>
	<li>{{domxref("WebGLRenderingContext.texImage2D()")}}</li>
</ul>

