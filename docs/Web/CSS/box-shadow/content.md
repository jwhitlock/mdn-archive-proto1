---
version: prototype1
revision_id: 1342755
locale: en-US
slug: Web/CSS/box-shadow
tags: "CSS" "CSS Styles" "HTML Colors" "Styles" "Shadows" "Styling HTML" "CSS Property" "Reference" "box-shadow" "CSS Backgrounds and Borders"
title: box-shadow
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{CSSRef}}</div>

<p><span class="seoSummary">The <strong><code>box-shadow</code></strong> CSS property is used to add shadow effects around an element's frame. You can specify multiple effects separated by commas if you wish to do so.</span> A box shadow is described by X and Y offsets relative to the element, blur and spread radii, and color.</p>

<div>{{EmbedInteractiveExample("pages/css/box-shadow.html")}}</div>

<p>The <code>box-shadow</code> property enables you to cast a drop shadow from the frame of almost any element. If a {{cssxref("border-radius")}} is specified on the element with a box shadow, the box shadow takes on the same rounded corners. The z-ordering of multiple box shadows is the same as multiple <a href="/en-US/CSS/text-shadow">text shadows</a> (the first specified shadow is on top).</p>

<p><a href="/en-US/docs/Web/CSS/CSS_Box_Model/Box-shadow_generator">Box-shadow generator</a> is an interactive tool allowing you to generate a <code>box-shadow</code>.</p>

<h2 id="Syntax">Syntax</h2>

<pre class="brush: css no-line-numbers">
/* offset-x | offset-y | color */
box-shadow: 60px -16px teal;

/* offset-x | offset-y | blur-radius | color */
box-shadow: 10px 5px 5px black;

/* offset-x | offset-y | blur-radius | spread-radius | color */
box-shadow: 2px 2px 2px 1px rgba(0, 0, 0, 0.2);

/* inset | offset-x | offset-y | color */
box-shadow: inset 5em 1em gold;

/* Any number of shadows, separated by commas */
box-shadow: 3px 3px red, -1em 0 0.4em olive;

/* Global keywords */
box-shadow: inherit;
box-shadow: initial;
box-shadow: unset;
</pre>

<p>Specify a single box-shadow using:</p>

<ul>
 <li>Two, three, or four <code><a href="/en-US/docs/Web/CSS/length">&lt;length&gt;</a></code> values.

  <ul>
   <li>If only two values are given, they are interpreted as <code><a href="#&lt;offset-x&gt; &lt;offset-y&gt;">&lt;offset-x&gt;&lt;offset-y&gt;</a></code> values.</li>
   <li>If a third value is given, it is interpreted as a <code><a href="#&lt;blur-radius&gt;">&lt;blur-radius&gt;</a></code>.</li>
   <li>If a fourth value is given, it is interpreted as a <code><a href="#&lt;spread-radius&gt;">&lt;spread-radius&gt;</a></code>.</li>
  </ul>
 </li>
 <li>Optionally, the <code><a href="#inset">inset</a></code> keyword.</li>
 <li>Optionally, a <code><a href="#&lt;color&gt;">&lt;color&gt;</a></code> value.</li>
</ul>

<p>To specify multiple shadows, provide a comma-separated list of shadows.</p>

<h3 id="Values">Values</h3>

<dl>
 <dt><a id="inset" name="inset"><code>inset</code></a></dt>
 <dd>If not specified (default), the shadow is assumed to be a drop shadow (as if the box were raised above the content).<br />
 The presence of the <code>inset</code> keyword changes the shadow to one inside the frame (as if the content was depressed inside the box). Inset shadows are drawn inside the border (even transparent ones), above the background, but below content.</dd>
 <dt><a id="&lt;offset-x&gt; &lt;offset-y&gt;" name="&lt;offset-x&gt; &lt;offset-y&gt;"><code>&lt;offset-x&gt;</code> <code>&lt;offset-y&gt;</code></a></dt>
 <dd>These are two {{cssxref("&lt;length&gt;")}} values to set the shadow offset. <code>&lt;offset-x&gt;</code> specifies the horizontal distance. Negative values place the shadow to the left of the element. <code>&lt;offset-y&gt;</code> specifies the vertical distance. Negative values place the shadow above the element. See {{cssxref("&lt;length&gt;")}} for possible units.<br />
 If both values are <code>0</code>, the shadow is placed behind the element (and may generate a blur effect if <code>&lt;blur-radius&gt;</code> and/or <code>&lt;spread-radius&gt;</code> is set).</dd>
 <dt><a id="&lt;blur-radius&gt;" name="&lt;blur-radius&gt;"><code>&lt;blur-radius&gt;</code></a></dt>
 <dd>This is a third {{cssxref("&lt;length&gt;")}} value. The larger this value, the bigger the blur, so the shadow becomes bigger and lighter. Negative values are not allowed. If not specified, it will be <code>0</code> (the shadow's edge is sharp). The specification does not include an exact algorithm for how the blur radius should be calculated, however, it does elaborate as follows:</dd>
 <dd>
 <blockquote>…for a long, straight shadow edge, this should create a color transition the length of the blur distance that is perpendicular to and centered on the shadow’s edge, and that ranges from the full shadow color at the radius endpoint inside the shadow to fully transparent at the endpoint outside it.</blockquote>
 </dd>
 <dt><a id="&lt;spread-radius&gt;" name="&lt;spread-radius&gt;"><code>&lt;spread-radius&gt;</code></a></dt>
 <dd>This is a fourth {{cssxref("&lt;length&gt;")}} value. Positive values will cause the shadow to expand and grow bigger, negative values will cause the shadow to shrink. If not specified, it will be <code>0</code> (the shadow will be the same size as the element).</dd>
 <dt><a id="&lt;color&gt;" name="&lt;color&gt;"><code>&lt;color&gt;</code></a></dt>
 <dd>See {{cssxref("&lt;color&gt;")}} values for possible keywords and notations.<br />
 If not specified, the color used depends on the browser - it is usually the value of the {{cssxref("color")}} property, but note that Safari currently paints a transparent shadow in this case.</dd>
</dl>

<h3 id="Interpolation">Interpolation</h3>

<p>Each shadow in the list (treating <code>none</code> as a 0-length list) is interpolated via the color (as color) component, and x, y, blur, and (when appropriate) spread (as length) components. For each shadow, if both input shadows are or are not <code>inset</code>, then the interpolated shadow must match the input shadows in that regard. If any pair of input shadows has one <code>inset</code> and the other not <code>inset</code>, the entire shadow list is uninterpolable. If the lists of shadows have different lengths, then the shorter list is padded at the end with shadows whose color is <code>transparent</code>, all lengths are <code>0</code>, and whose <code>inset</code> (or not) matches the longer list.</p>

<h3 id="Formal_syntax">Formal syntax</h3>

<pre class="syntaxbox">
{{csssyntax}}</pre>

<h2 id="Examples">Examples</h2>

<ul>
 <li><a href="http://www.elektronotdienst-nuernberg.de/bugs/box-shadow_inset.html">box-shadow test</a></li>
 <li><a href="http://markusstange.wordpress.com/2009/02/15/fun-with-box-shadows/">box-shadow tutorial and examples</a></li>
 <li><a href="https://cssgenerator.org/box-shadow-css-generator.html">Box Shadow CSS Generator</a></li>
</ul>

<h2 class="cleared" id="Specifications">Specifications</h2>

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
   <td>{{SpecName('CSS3 Backgrounds', '#box-shadow', 'box-shadow')}}</td>
   <td>{{Spec2('CSS3 Backgrounds')}}</td>
   <td>Initial definition</td>
  </tr>
 </tbody>
</table>

<p>{{cssinfo}}</p>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<p>&nbsp;</p>

<div class="hidden">The compatibility table on this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</div>

<p>{{Compat("css.properties.box-shadow")}}</p>

<p>&nbsp;</p>

<h2 id="See_also">See also</h2>

<ul>
 <li>The {{cssxref("&lt;color&gt;")}} data type</li>
 <li>Other color-related properties: {{cssxref("color")}}, {{cssxref("background-color")}}, {{cssxref("border-color")}}, {{cssxref("outline-color")}}, {{cssxref("text-decoration-color")}}, {{cssxref("text-emphasis-color")}}, {{cssxref("caret-color")}}, and {{cssxref("column-rule-color")}}</li>
 <li><a href="/en-US/docs/Web/HTML/Applying_color">Applying color to HTML elements using CSS</a></li>
</ul>

