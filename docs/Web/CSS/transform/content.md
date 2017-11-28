---
version: prototype1
revision_id: 1331147
locale: en-US
slug: Web/CSS/transform
tags: "CSS" "CSS Property" "Reference" "Transforms" "NeedsBrowserCompatibility"
title: transform
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{CSSRef}}</div>

<p>The <strong><code>transform</code></strong> <a href="/en-US/docs/Web/CSS">CSS</a> property lets you modify the coordinate space of the CSS visual formatting model. Using it, elements can be translated, rotated, scaled, and skewed.</p>

<div>{{EmbedInteractiveExample("pages/css/transform.html")}}</div>

<p>If the property has a value different than <code>none</code>, a <a href="/en-US/docs/Web/CSS/CSS_Positioning/Understanding_z_index/The_stacking_context">stacking context</a> will be created. In that case the object will act as a containing block for <code>position: fixed</code> elements that it contains.</p>

<h2 id="Syntax">Syntax</h2>

<p>The <code>transform</code> property may be specified as either the keyword value <code><a href="#none">none</a></code> or as one or more <code><a href="#&lt;transform-function&gt;">&lt;transform-function&gt;</a></code> values.</p>

<h3 id="Values">Values</h3>

<dl>
 <dt id="&lt;transform-function&gt;">{{cssxref("&lt;transform-function&gt;")}}</dt>
 <dd>One or more of the <a href="/en-US/docs/Web/CSS/transform-function">CSS transform functions</a> to be applied. Composite transforms are effectively applied in order from left to right.</dd>
 <dt id="none"><code>none</code></dt>
 <dd>Specifies that no transform should be applied.</dd>
</dl>

<h3 id="Formal_syntax">Formal syntax</h3>

<pre class="syntaxbox">
{{csssyntax}}</pre>

<h2 id="Examples">Examples</h2>

<h3 id="HTML">HTML</h3>

<pre class="brush: html">
&lt;p&gt;Transformed element&lt;/p&gt;</pre>

<h3 id="CSS">CSS</h3>

<pre class="brush: css">
p {
  border: solid red;
  transform: translate(100px) rotate(20deg);
  transform-origin: 0 -250px;
}</pre>

<h3 id="Result">Result</h3>

<p>{{EmbedLiveSample("Examples", "400", "170")}}</p>

<p>Please see <a href="/en-US/docs/Web/Guide/CSS/Using_CSS_transforms">Using CSS transforms</a> and {{cssxref("&lt;transform-function&gt;")}} for more examples.</p>

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
   <td>{{SpecName('CSS Transforms 2', '#transform-functions', 'transform')}}</td>
   <td>{{Spec2('CSS Transforms 2')}}</td>
   <td>Adds 3D transform functions.</td>
  </tr>
  <tr>
   <td>{{SpecName('CSS3 Transforms', '#transform-property', 'transform')}}</td>
   <td>{{Spec2('CSS3 Transforms')}}</td>
   <td>Initial definition.</td>
  </tr>
 </tbody>
</table>

<p>{{cssinfo}}</p>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<div class="hidden">The compatibility table on this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</div>

<p>{{Compat("css.properties.transform")}}</p>

<h2 id="See_also">See also</h2>

<ul>
 <li><a href="/en-US/docs/CSS/Using_CSS_transforms">Using CSS transforms</a></li>
 <li>{{cssxref("&lt;transform-function&gt;")}} data type</li>
 <li>A cross-browser 2D <a href="https://louisremi.github.io/jquery.transform.js/">transform plugin for jQuery</a></li>
</ul>

