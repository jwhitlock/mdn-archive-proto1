---
version: prototype1
revision_id: 1364855
locale: en-US
slug: user:jwhitlock
tags: "user page"
title: user:jwhitlock
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>This is a test page for <a href="/en-US/profiles/jwhitlock">jwhitlock</a>.</p>

<p>This is my first edit in AWS. Editing is easy! And works every time!</p>

<p><img alt="Me in 2017" src="https://mdn.mozillademos.org/files/15321/avatar_2017.jpg" style="height:140px; width:140px" /></p>

<p>This is a test of the notification system.</p>

<div class="hidden">
<p>This text is hidden when reading.</p>
</div>

<p>{{ anch("foo", "bar") }}</p>

<h3 id="Subpages">Subpages</h3>

<p>{{ListSubpages}}</p>

<h3 id="Link_Test">Link Test</h3>

<ul>
 <li><a href="/en-US/docs/user%3Ajwhitlock/TextFormatting">/en-US/docs/user:jwhitlock/TextFormatting</a> - Absolute link, existing page</li>
 <li><a href="/en-US/docs/user%3Ajwhitlock/TextFormatting/">/en-US/docs/user:jwhitlock/TextFormatting/</a> - Absolute link, redirect to existing page</li>
 <li><a href="/en-US/docs/user%3Ajwhitlock/Missing">/en-US/docs/user:jwhitlock/Missing</a> - Absolute link, new page</li>
 <li><a href="user%3Ajwhitlock/TextFormatting">user:jwhitlock/TextFormatting</a> - Relative link, existing page</li>
 <li><a href="user%3Ajwhitlock/TextFormatting/">user:jwhitlock/TextFormatting/</a> - Relative link, redirect to existing page</li>
 <li><a href="user%3Ajwhitlock/Missing">user:jwhitlock/Missing</a> - Relative link, new page</li>
</ul>

<h2 id="Live_Sample_Demo">Live Sample Demo</h2>

<p>From <a href="/en-US/docs/MDN/Contribute/Structures/Live_samples">MDN/Contribute/Structures/Live_samples</a></p>

<h3 id="HTML">HTML</h3>

<pre class="brush: html line-numbers  language-html">
&lt;p&gt;A simple example of the live sample system in action.&lt;/p&gt;
&lt;div class="box"&gt;
  &lt;div id="item"&gt;Hello world! Welcome to MDN&lt;/div&gt;
&lt;/div&gt;
</pre>

<h3 id="CSS">CSS</h3>

<pre class="brush: css line-numbers  language-css">
.box {
  width: 200px;
  border-radius: 6px;
  padding: 20px;
  background-color: #ffaabb;
}

#item {
  font-weight: bold;
  text-align: center;
  font-family: sans-serif;
  font-size: 1.5em;
}
</pre>

<h3 id="JavaScript">JavaScript</h3>

<pre class="brush: js line-numbers  language-js">
var el = document.getElementById('item');
el.onclick = function() {
  alert('Owww, stop poking me!');
}
</pre>

<h3 id="Result">Result</h3>

<p>Here's the result:</p>

<p>{{EmbedLiveSample('Live_Sample_Demo')}}</p>

