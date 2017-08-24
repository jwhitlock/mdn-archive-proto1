---
version: prototype1
revision_id: 1293059
locale: en-US
slug: Experiment:InteractiveEditor/background-color
tags: "CSS" "Layout" "CSS Property" "Graphics" "Reference" "CSS Background"
title: background-color
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{CSSRef}}</div>

<p>The <strong><code>background-color</code></strong> <a href="/en-US/docs/Web/CSS">CSS</a> property sets the background color of an element, either through a color value or the keyword <code>transparent</code>.</p>

<div>{{EmbedInteractiveExample("pages/css/background-color.html")}}</div>

<div>{{cssinfo}}</div>

<h2 id="Syntax">Syntax</h2>

<p>The <code>background-color</code> property is specified as a single <code><a href="#&lt;color&gt;">&lt;color&gt;</a></code> value.</p>

<h3 id="Values">Values</h3>

<dl>
 <dt><a id="&lt;color&gt;"><code>&lt;color&gt;</code></a></dt>
 <dd>Is a CSS {{cssxref("&lt;color&gt;")}} that describes the uniform color of the background. Even if one or several {{cssxref("background-image")}} are defined, this color can be affect the rendering, by transparency if the images aren't opaque. In CSS, <code>transparent</code> is a color.</dd>
</dl>

<h3 id="Formal_syntax">Formal syntax</h3>

<pre class="syntaxbox">
{{csssyntax}}</pre>

<h2 id="Examples">Examples</h2>

<h3 id="HTML">HTML</h3>

<pre class="brush: html">
&lt;div class="exampleone"&gt;
 Lorem ipsum dolor sit amet, consectetuer
&lt;/div&gt;

&lt;div class="exampletwo"&gt;
  Lorem ipsum dolor sit amet, consectetuer
&lt;/div&gt;

&lt;div class="examplethree"&gt;
  Lorem ipsum dolor sit amet, consectetuer
&lt;/div&gt;</pre>

<h3 id="CSS">CSS</h3>

<pre class="brush: css; highlight:[2,7,12];">
.exampleone {
  background-color: teal;
  color: white;
}

.exampletwo {
  background-color: rgb(153,102,153);
  color: rgb(255,255,204);
}

.examplethree {
  background-color: #777799;
  color: #FFFFFF;
}
</pre>

<h3 id="Result">Result</h3>

<p>{{EmbedLiveSample("Examples","200","150")}}</p>

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
   <td>{{SpecName('CSS3 Backgrounds', '#background-color', 'background-color')}}</td>
   <td>{{Spec2('CSS3 Backgrounds')}}</td>
   <td>Though technically removing the <code>transparent</code> keyword, this doesn't change anything as it has been incorporated as a true {{cssxref("&lt;color&gt;")}}</td>
  </tr>
  <tr>
   <td>{{SpecName('CSS2.1', 'colors.html#propdef-background-color', 'background-color')}}</td>
   <td>{{Spec2('CSS2.1')}}</td>
   <td>No change</td>
  </tr>
  <tr>
   <td>{{SpecName('CSS1', '#background-color', 'background-color')}}</td>
   <td>{{Spec2('CSS1')}}</td>
   <td>Initial definition</td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<p class="hidden">The compatibility table in this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</p>

<p>{{Compat("css.properties.background-color")}}</p>

<h2 id="See_also">See also</h2>

<ul>
 <li>
  <p><a href="/en-US/docs/Web/CSS/CSS_Background_and_Borders/Using_CSS_multiple_backgrounds" title="en/CSS/Multiple backgrounds">Multiple backgrounds</a></p>
 </li>
</ul>

