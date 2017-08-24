---
version: prototype1
revision_id: 1293047
locale: en-US
slug: Experiment:InteractiveEditor/transform
tags: "CSS" "CSS Property" "Property" "Reference" "Transforms" "NeedsBrowserCompatibility"
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

<p>The CSS <strong><code>transform</code></strong> property lets you modify the coordinate space of the CSS visual formatting model. Using it, elements can be translated, rotated, scaled, and skewed.</p>

<div>{{EmbedInteractiveExample("pages/css/transform.html")}}</div>

<p>If the property has a value different than <code>none</code>, a <a href="/en-US/docs/Web/CSS/CSS_Positioning/Understanding_z_index/The_stacking_context">stacking context</a> will be created. In that case the object will act as a containing block for <code>position</code><code>: fixed</code> elements that it contains.</p>

<p>{{cssinfo}}</p>

<h2 id="Syntax">Syntax</h2>

<p>The <code>transform</code> property may be specified as either the keyword value <code><a href="#none">none</a></code> or as one or more <code><a href="#&lt;transform-function&gt;">&lt;transform-function&gt;</a></code> values.</p>

<h3 id="Values">Values</h3>

<dl>
 <dt><a id="&lt;transform-function&gt;" name="&lt;transform-function&gt;"><code>&lt;transform-function&gt;</code></a></dt>
 <dd>One or more of the <a href="/en-US/docs/Web/CSS/transform-function">CSS transform functions</a> to be applied, see below. Composite transforms are effectively applied in order from left to right.</dd>
 <dt><a id="none" name="none"><code>none</code></a></dt>
 <dd>Specifies that no transform should be applied.</dd>
</dl>

<h3 id="Formal_syntax">Formal syntax</h3>

<pre class="syntaxbox">
{{csssyntax}}</pre>

<h2 id="Examples">Examples</h2>

<p>See <a href="/en-US/docs/Web/Guide/CSS/Using_CSS_transforms">Using CSS transforms</a>.</p>

<h2 id="Live_example">Live example</h2>

<h3 id="HTML_content">HTML content</h3>

<pre class="brush: html">
&lt;p&gt;Transformed element&lt;/p&gt;</pre>

<h3 id="CSS_content">CSS content</h3>

<pre class="brush: css">
p {
  border: solid red;

  -webkit-transform: translate(100px) rotate(20deg);
  -webkit-transform-origin: 0 -250px;

  transform: translate(100px) rotate(20deg);
  transform-origin: 0 -250px;
}</pre>

<p>{{EmbedLiveSample("Live_example", "400", "170")}}</p>

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
   <td>Initial definition</td>
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
   <th>Edge</th>
   <th>Firefox (Gecko)</th>
   <th>Internet Explorer</th>
   <th>Opera</th>
   <th>Safari</th>
  </tr>
  <tr>
   <td>Basic support</td>
   <td>{{CompatVersionUnknown}} {{property_prefix("-webkit")}}<br />
    36</td>
   <td>{{CompatVersionUnknown}}{{property_prefix("-webkit")}}<br />
    {{CompatVersionUnknown}}</td>
   <td>{{CompatGeckoDesktop("1.9.1")}}{{property_prefix("-moz")}}<sup>[1]</sup><br />
    {{CompatGeckoDesktop("16.0")}}<sup>[2]</sup></td>
   <td>9.0{{property_prefix("-ms")}}<sup>[3]</sup><br />
    10.0</td>
   <td>10.5{{property_prefix("-o")}}<br />
    12.10<br />
    15.0{{property_prefix("-webkit")}}<br />
    23</td>
   <td>3.1{{property_prefix("-webkit")}}<br />
    9.0</td>
  </tr>
  <tr>
   <td>3D Support</td>
   <td>12.0{{property_prefix("-webkit")}}<br />
    36</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>10.0{{property_prefix("-moz")}}<br />
    {{CompatGeckoDesktop("16.0")}}</td>
   <td>10.0</td>
   <td>15.0{{property_prefix("-webkit")}}<br />
    23</td>
   <td>
    <p>4.0{{property_prefix("-webkit")}}<br />
     9.0</p>
   </td>
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
   <th>Edge</th>
   <th>Firefox Mobile (Gecko)</th>
   <th>IE Mobile</th>
   <th>Opera Mobile</th>
   <th>Safari Mobile</th>
  </tr>
  <tr>
   <td>Basic support</td>
   <td>{{CompatAndroid(2.1)}}{{property_prefix("-webkit")}}<sup>[4]</sup></td>
   <td>{{CompatVersionUnknown}}{{property_prefix("-webkit")}}</td>
   <td>{{CompatVersionUnknown}}{{property_prefix("-webkit")}}<br />
    {{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}<br />
    11.0{{property_prefix("-webkit")}}<sup>[5]</sup></td>
   <td>11.5{{property_prefix("-webkit")}}</td>
   <td>3.2 {{CompatVersionUnknown}}{{property_prefix("-webkit")}}<br />
    9.0</td>
  </tr>
  <tr>
   <td>3D Support</td>
   <td>{{CompatAndroid(3.0)}}{{property_prefix("-webkit")}}</td>
   <td>{{CompatVersionUnknown}}{{ property_prefix("-webkit")}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>22{{property_prefix("-webkit")}}</td>
   <td>3.2 {{CompatVersionUnknown}}{{property_prefix("-webkit")}}<br />
    9.0</td>
  </tr>
 </tbody>
</table>
</div>

<p>[1] Gecko 14.0 removed the experimental support for <code>skew()</code>, but it was reintroduced in Gecko 15.0 for compatibility reasons. As it is non-standard and will likely be removed in the future, do not use it.</p>

<p>[2] Before Firefox 16, the translation values of <code>matrix()</code> and <code>matrix3d()</code> could be {{cssxref("&lt;length&gt;")}}, in addition to the standard {{cssxref("&lt;number&gt;")}}.</p>

<p>In addition to the unprefixed support, Gecko 44.0 {{geckoRelease("44.0")}} added support for a <code>-webkit</code> prefixed version of the property for web compatibility reasons behind the preference <code>layout.css.prefixes.webkit</code>, defaulting to <code>false</code>. Since Gecko 49.0 {{geckoRelease("49.0")}} the preference defaults to <code>true</code>.</p>

<p>[3] Internet Explorer 5.5 or later supports a proprietary <a href="https://msdn.microsoft.com/en-us/library/ms533014(VS.85,loband).aspx">Matrix Filter</a> which can be used to achieve a similar effect.</p>

<p>Internet Explorer 9.0 or earlier has no support for 3D transforms.&nbsp;Mixing 3D and&nbsp;2D transform functions,&nbsp;such as <code>-ms-transform:rotate(10deg) translateZ(0);</code>, will prevent the entire property from being applied.</p>

<p>Internet Explorer does not support the&nbsp;global values <code>initial</code> and <code>unset.</code></p>

<p>[4] Android 2.3 has a bug where input forms will "jump" when typing, if any container element has a <code>-webkit-transform</code>.</p>

<p>[5] Internet Explorer 11.0 supports the {{property_prefix("-webkit")}} <a href="https://msdn.microsoft.com/library/jj127312#code-snippet-1">prefixed variant as an alias for the default one</a>.</p>

<h2 id="See_also">See also</h2>

<ul>
 <li><a href="/en-US/docs/CSS/Using_CSS_transforms">Using CSS Transforms</a></li>
 <li><a href="/en-US/docs/Web/CSS/transform-function">&lt;translation-function&gt;</a> data type</li>
 <li><a href="https://www.paulirish.com/2010/introducing-css3please/#comment-36380">More info</a> on CSS3 Rotation / Matrix Filter issues in the comments on Paul Irish's blog.</li>
 <li>A cross-browser 2D <a href="https://louisremi.github.io/jquery.transform.js/">transform plugin for jQuery</a></li>
</ul>

