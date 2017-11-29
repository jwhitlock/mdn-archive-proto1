---
version: prototype1
revision_id: 1331576
locale: en-US
slug: Web/CSS/background-color
tags: "CSS" "HTML Colors" "HTML Styles" "Layout" "Styles" "Styling HTML" "CSS Property" "Graphics" "Reference" "CSS Background" "background-color"
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

<p>The <strong><code>background-color</code></strong> <a href="/en-US/docs/Web/CSS">CSS</a> property sets the background color of an element, using either a {{cssxref("&lt;color&gt;")}} value or the keyword <code>transparent</code>.</p>

<pre class="brush: css no-line-numbers">
/* Keyword values */
background-color: red;

/* Hexadecimal value */
background-color: #bbff00;

/* Hexadecimal value with alpha channel */
background-color: #11ffee00; /* 00 - fully transparent */
background-color: #11ffeeff; /* ff - fully opaque */

/* RGB value */
background-color: rgb(255, 255, 128);

/* RGBA value or RGB with alpha channel */
background-color: rgba(117, 190, 218, 0.0); /* 0.0 - fully transparent */
background-color: rgba(117, 190, 218, 0.5); /* 0.5 - semi-transparent */
background-color: rgba(117, 190, 218, 1.0); /* 1.0 - fully opaque */
​​​​​​​
/* HSLA value */
background-color: hsla(50, 33%, 25%, 0.75);

/* Special keyword values */
background-color: currentcolor;
background-color: transparent;

/* Global values */
background-color: inherit;
background-color: initial;
background-color: unset;</pre>

<div class="hidden" id="background-color">
<pre class="brush: html">
&lt;div id="container"&gt;
  &lt;div class="subcontainer"&gt;
    &lt;div id="keyword" class="color"&gt;&lt;/div&gt;
    &lt;div class="caption"&gt;skyblue&lt;/div&gt;
  &lt;/div&gt;
  &lt;div class="subcontainer"&gt;
    &lt;div id="hex" class="color"&gt;&lt;/div&gt;
    &lt;div class="caption"&gt;#bbff00;&lt;/div&gt;
  &lt;/div&gt;
  &lt;div class="subcontainer"&gt;
    &lt;div id="rgb" class="color"&gt;&lt;/div&gt;
    &lt;div class="caption"&gt;rgb(240, 220, 180)&lt;/div&gt;
  &lt;/div&gt;
  &lt;div class="subcontainer"&gt;
    &lt;div id="rgba" class="color"&gt;&lt;/div&gt;
    &lt;div class="caption"&gt;rgba(240, 220, 180, 0.5)&lt;/div&gt;
  &lt;/div&gt;
  &lt;div class="subcontainer"&gt;
    &lt;div id="hsl" class="color"&gt;&lt;/div&gt;
    &lt;div class="caption"&gt;hsl(50, 60%, 75%)&lt;/div&gt;
  &lt;/div&gt;
  &lt;div class="subcontainer"&gt;
    &lt;div id="currentcolor" class="color"&gt;&lt;/div&gt;
    &lt;div class="caption"&gt;currentcolor&lt;/div&gt;
  &lt;/div&gt;
  &lt;div class="subcontainer"&gt;
    &lt;div id="transparent" class="color"&gt;&lt;/div&gt;
    &lt;div class="caption"&gt;transparent&lt;/div&gt;
  &lt;/div&gt;
&lt;/div&gt;
</pre>

<pre class="brush: css">
#container {
  width: 100%;
  background-color: #F4F7F8;
  display: flex;
  flex-wrap: wrap;
}

.subcontainer {
  border: 1px solid black;
  height: 80px;
  margin: 10px;
  flex: 1 0 auto;
  display: flex;
  flex-direction: column;
  background-color: #dcdcdc;
  background-image:
      linear-gradient(45deg, rgb(0, 0, 0, 0.1) 25%, transparent 25%),
      linear-gradient(225deg, rgb(0, 0, 0, 0.1) 25%, transparent 25%),
      linear-gradient(225deg, rgb(0, 0, 0, 0.1) 25%, transparent 25%),
      linear-gradient(45deg, rgb(0, 0, 0, 0.1) 25%, transparent 25%);
  background-size: 20px 20px;
  background-position: 0 0, -10px -10px;
}

.color {
  width: 100%;
  flex: 1 0 auto;
}

.caption {
  background-color: white;
  padding: 10px;
  text-align: center;
  white-space: nowrap;
  color: black;
  font-family: monospace;
  font-weight: bold;
}

#keyword {
  background-color: skyblue;
}

#hex {
  background-color: #bbff00;
}

#rgb {
  background-color: rgb(240, 220, 180);
}

#rgba {
  background-color: rgb(240, 220, 180, 0.5);
}

#hsl {
  background-color: hsl(50, 60%, 75%);
}

#currentcolor {
  background-color: currentcolor;
}

#transparent {
  background-color: transparent;
}</pre>
</div>

<p>{{EmbedLiveSample("background-color", 1200, 210, "", "", "example-outcome-frame")}}</p>

<div>{{cssinfo}}</div>

<h2 id="Syntax">Syntax</h2>

<p>The <code>background-color</code> property is specified as a single <code><a href="#&lt;color&gt;">&lt;color&gt;</a></code> value.</p>

<h3 id="Values">Values</h3>

<dl>
 <dt><a id="&lt;color&gt;"></a>{{cssxref("&lt;color&gt;")}}</dt>
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
 <li><a href="/en-US/docs/Web/CSS/CSS_Background_and_Borders/Using_CSS_multiple_backgrounds" title="en/CSS/Multiple backgrounds">Multiple backgrounds</a></li>
 <li>The {{cssxref("&lt;color&gt;")}} data type</li>
 <li>Other color-related properties: {{cssxref("color")}}, {{cssxref("border-color")}}, {{cssxref("outline-color")}}, {{cssxref("text-decoration-color")}}, {{cssxref("text-emphasis-color")}}, {{cssxref("text-shadow")}}, {{cssxref("caret-color")}}, and {{cssxref("column-rule-color")}}</li>
 <li><a href="/en-US/docs/Web/HTML/Applying_color">Applying color to HTML elements using CSS</a></li>
</ul>

