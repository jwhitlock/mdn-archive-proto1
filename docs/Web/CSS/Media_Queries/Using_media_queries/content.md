---
version: prototype1
revision_id: 1325833
locale: en-US
slug: Web/CSS/Media_Queries/Using_media_queries
tags: "CSS" "Web" "Guide" "Media" "Advanced" "Media Queries" "Responsive Design"
title: Using media queries
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{cssref}}</div>

<p><strong>Media queries</strong> are useful when you want to apply CSS styles depending on a device's general type (such as print vs. screen), specific characteristics (such as the width of the browser viewport, or environment (such as ambient light conditions). With the huge variety of internet-connected devices available today, media queries are a vital tool for building websites and apps that are robust enough to work on whatever hardware your users have.</p>

<h2 id="Targeting_media_types">Targeting media types</h2>

<p><a class="internal" href="/en-US/docs/CSS/@media#Media_types">Media types</a> describe the general category of a given device. Although websites are commonly designed with screens in mind, you may want to create styles that target special devices such as printers or audio-based screenreaders. For example, this CSS targets printers:</p>

<pre class="brush: css">
@media print { ... }</pre>

<p>You can also target multiple devices. For instance, this <code>@media</code> rule uses two media queries to target both screen and print devices:</p>

<pre class="brush: css">
@media screen, print { ... }</pre>

<p>See <a class="internal" href="/en-US/docs/CSS/@media#Media_types">Media types</a> for a list of all media types. Because they describe devices in only very broad terms, just a few are available; to target more specific attributes, use <em>media features</em> instead.</p>

<h2 id="Targeting_media_features">Targeting media features</h2>

<p><a href="/en-US/docs/CSS/@media#Media_features">Media features</a> describe the specific characteristics of a given {{glossary("user agent")}}, output device, or environment. For instance, you can apply specific styles to widescreen monitors, computers that use mice, or to devices that are being used in low-light conditions. This example applies styles when the user's <em>primary</em> input mechanism (such as a mouse) can hover over elements:</p>

<pre class="brush: css">
@media (hover: hover) { ... }</pre>

<p>Many media features are <em>range features</em>, which means they can be prefixed with "min-" or "max-" to express "minimum condition" or "maximum condition" constraints. For example, this CSS will apply styles only if your browser's {{glossary("viewport")}} width is equal to or narrower than 12,450px:</p>

<pre class="brush: css">
@media (max-width: 12450px) { ... }</pre>

<p>If you create a media feature query without specifying a value, the nested styles will be used as long as the feature's value is non-zero. For example, this CSS will apply to any device with a color screen:</p>

<pre class="brush: css">
@media (color) { ... }</pre>

<p>If a feature doesn't apply to the device on which the browser is running, expressions involving that media feature are always false. For example, the styles nested inside the following query will never be used, because no speech-only device has a screen aspect ratio:</p>

<pre class="brush: css">
@media speech and (aspect-ratio: 11/5) { ... }</pre>

<p>For more media feature examples, please see the <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/@media#Media_features">reference page</a> for each specific feature.</p>

<h2 id="Creating_complex_media_queries">Creating complex media queries</h2>

<p>Sometimes you may want to create a media query that depends on multiple conditions. This is where the <em>logical operators</em> come in: <code>not</code>, <code>and</code>, and <code>only</code>. Furthermore, you can combine multiple media queries into a <em>comma-separated list</em>; this allows you to apply the same styles in different situations.</p>

<p>In the previous example, we've already seen the <code>and</code> operator used to group a media <em>type</em> with a media <em>feature</em>. The <code>and</code> operator can also combine multiple media features into a single media query. The <code>not</code> operator, meanwhile, negates a media query, basically reversing its normal meaning. The <code>only</code> operator prevents older browsers from applying the styles.</p>

<div class="note">
<p><strong>Note:</strong> In most cases, the <code>all</code> media type is used by default when no other type is specified. However, if you use the <code>not</code> or <code>only</code> operators, you must explicitly specify a media type.</p>
</div>

<h3 id="and"><code>and</code></h3>

<p>The <code>and</code> keyword combines a media feature with a media type <em>or</em> other media features. This example combines two media features to restrict styles to landscape-oriented devices with a width of at least 30 ems:</p>

<pre class="brush: css">
@media (min-width: 30em) and (orientation: landscape) { ... }</pre>

<p>To limit the styles to devices with a screen, you can chain the media features to the <code>screen</code> media type:</p>

<pre class="brush: css">
@media screen and (min-width: 30em) and (orientation: landscape) { ... }</pre>

<h3 id="comma-separated_lists">comma-separated lists</h3>

<p>You can use a comma-separated list to apply styles when the user's device matches any one of various media types, features, or states. For instance, the following rule will apply its styles if the user's device has either a minimum height of 680px <em>or</em> is a screen device in portrait mode:</p>

<pre class="brush: css">
@media (min-height: 680px), screen and (orientation: portrait) { ... }</pre>

<p>Taking the above example, if the user had a printer with a page height of 800px, the media statement would return true because the first query would apply. Likewise, if the user were on a smartphone in portrait mode with a viewport height of 480px, the second query would apply and the media statement would still return true.</p>

<h3 id="not"><code>not</code></h3>

<p>The <code>not</code> keyword inverts the meaning of an entire media query. It will only negate the specific media query it is applied to. (Thus, it will not apply to every media query in a comma-separated list of media queries.) The <code>not</code> keyword can't be used to negate an individual feature query, only an entire media query. The <code>not</code> is evaluated last in the following query:</p>

<pre class="brush: css">
@media not all and (monochrome) { ... }
</pre>

<p>... so that the above query is evaluated like this:</p>

<pre class="brush: css">
@media not (all and (monochrome)) { ... }
</pre>

<p>... rather than like this:</p>

<pre class="brush: css example-bad">
@media (not all) and (monochrome) { ... }</pre>

<p>As another example, the following media query:</p>

<pre class="brush: css">
@media not screen and (color), print and (color) { ... }
</pre>

<p>... is evaluated like this:</p>

<pre class="brush: css">
@media (not (screen and (color))), print and (color) { ... }</pre>

<h3 id="only"><code>only</code></h3>

<p>The <code>only</code> keyword prevents older browsers that do not support media queries with media features from applying the given styles. <em>It has no effect on modern browsers.</em></p>

<pre class="brush: html">
&lt;link rel="stylesheet" media="only screen and (color)" href="modern-styles.css" /&gt;
</pre>

<h2 id="See_also">See also</h2>

<ul>
 <li><a class="internal" href="/en-US/docs/CSS/@media#Media_types">Media types</a></li>
 <li><a href="/en-US/docs/CSS/@media#Media_features">Media features</a></li>
 <li><a href="/en-US/docs/CSS/Using_media_queries_from_code">Testing media queries using code</a></li>
 <li><a href="http://davidwalsh.name/animate-media-queries">CSS Animations Between Media Queries</a></li>
 <li><a href="/en-US/docs/Web/CSS/Mozilla_Extensions#Media_features">Extended Mozilla media features</a></li>
 <li><a href="/en-US/docs/Web/CSS/Webkit_Extensions#Media_features">Extended WebKit media features</a></li>
</ul>

