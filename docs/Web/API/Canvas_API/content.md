---
version: prototype1
revision_id: 1367247
locale: en-US
slug: Web/API/Canvas_API
tags: "API" "Canvas" "Overview" "JavaScript" "Reference"
title: Canvas API
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{CanvasSidebar}}</div>

<p class="summary">Added in <a href="/en-US/docs/HTML/HTML5">HTML5</a>, the <strong>HTML {{HTMLElement("canvas")}} element</strong> can be used to draw graphics via scripting in <a href="/en-US/docs/Web/JavaScript">JavaScript</a>. For example, it can be used to draw graphs, make photo compositions, create animations, or even do real-time video processing or rendering.</p>

<p>Mozilla applications gained support for <code>&lt;canvas&gt;</code> starting with Gecko 1.8 (i.e. <a href="/en-US/docs/Mozilla/Firefox/Releases/1.5">Firefox 1.5</a>). The element was originally introduced by Apple for the OS X Dashboard and Safari. Internet Explorer supports <code>&lt;canvas&gt;</code> from version 9 onwards; for earlier versions of IE, a page can effectively add support for <code>&lt;canvas&gt;</code> by including a script from Google's <a href="https://github.com/arv/explorercanvas">Explorer Canvas</a> project. Google Chrome and Opera 9 also support <code>&lt;canvas&gt;</code>.</p>

<p>The <code>&lt;canvas&gt;</code> element is also used by <a href="/en-US/docs/Web/WebGL">WebGL</a> to draw&nbsp;hardware-accelerated 3D graphics on web pages.</p>

<h2 id="Example">Example</h2>

<p>This is just a simple code snippet which uses the {{domxref("CanvasRenderingContext2D.fillRect()")}} method.</p>

<h3 id="HTML">HTML</h3>

<pre class="brush: html">
&lt;canvas id="canvas"&gt;&lt;/canvas&gt;
</pre>

<h3 id="JavaScript">JavaScript</h3>

<pre class="brush: js">
var canvas = document.getElementById('canvas');
var ctx = canvas.getContext('2d');

ctx.fillStyle = 'green';
ctx.fillRect(10, 10, 100, 100);
</pre>

<p>Edit the code below and see your changes update live in the canvas:</p>

<div class="hidden">
<h6 id="Playable_code">Playable code</h6>

<pre class="brush: html">
&lt;canvas id="canvas" width="400" height="200" class="playable-canvas"&gt;&lt;/canvas&gt;
&lt;div class="playable-buttons"&gt;
&nbsp; &lt;input id="edit" type="button" value="Edit" /&gt;
&nbsp; &lt;input id="reset" type="button" value="Reset" /&gt;
&lt;/div&gt;
&lt;textarea id="code" class="playable-code"&gt;
ctx.fillStyle = 'green';
ctx.fillRect(10, 10, 100, 100);&lt;/textarea&gt;
</pre>

<pre class="brush: js">
var canvas = document.getElementById('canvas');
var ctx = canvas.getContext("2d");
var textarea = document.getElementById('code');
var reset = document.getElementById('reset');
var edit = document.getElementById('edit');
var code = textarea.value;

function drawCanvas() {
  ctx.clearRect(0, 0, canvas.width, canvas.height);
  eval(textarea.value);
}

reset.addEventListener('click', function() {
  textarea.value = code;
  drawCanvas();
});

edit.addEventListener('click', function() {
  textarea.focus();
})

textarea.addEventListener('input', drawCanvas);
window.addEventListener('load', drawCanvas);
</pre>
</div>

<p>{{ EmbedLiveSample('Playable_code', 700, 360) }}</p>

<h2 id="Reference">Reference</h2>

<div class="index">
<ul>
 <li>{{domxref("HTMLCanvasElement")}}</li>
 <li>{{domxref("CanvasRenderingContext2D")}}</li>
 <li>{{domxref("CanvasGradient")}}</li>
 <li>{{domxref("CanvasImageSource")}}</li>
 <li>{{domxref("CanvasPattern")}}</li>
 <li>{{domxref("ImageBitmap")}}</li>
 <li>{{domxref("ImageData")}}</li>
 <li>{{domxref("RenderingContext")}}</li>
 <li>{{domxref("TextMetrics")}}</li>
 <li>{{domxref("OffscreenCanvas")}}{{experimental_inline}}</li>
 <li>{{domxref("Path2D")}} {{experimental_inline}}{{domxref("ImageBitmapRenderingContext")}}{{experimental_inline}}</li>
</ul>
</div>

<p>The interfaces related to the <code>WebGLRenderingContext</code> are referenced under <a href="/en-US/docs/Web/WebGL" title="/en-US/docs/Web/WebGL">WebGL</a>.</p>

<p>{{domxref("CanvasCaptureMediaStream")}} is related.</p>

<h2 id="Guides_and_tutorials">Guides and tutorials</h2>

<dl>
 <dt><a href="/en-US/docs/Web/API/Canvas_API/Tutorial">Canvas tutorial</a></dt>
 <dd>A comprehensive tutorial covering both the basic usage of <code>&lt;canvas&gt;</code> and its advanced features.</dd>
 <dt><a href="/en-US/Add-ons/Code_snippets/Canvas">Code snippets: Canvas</a></dt>
 <dd>Some extension developer-oriented code snippets involving <code>&lt;canvas&gt;</code>.</dd>
 <dt><a href="/en-US/docs/Web/API/Canvas_API/A_basic_ray-caster">Demo: A basic ray-caster</a></dt>
 <dd>A demo of ray-tracing animation using canvas.</dd>
 <dt><a href="/en-US/docs/Web/API/Canvas_API/Drawing_DOM_objects_into_a_canvas">Drawing DOM objects into a canvas</a></dt>
 <dd>How to draw DOM content, such as HTML elements, into a canvas.</dd>
 <dt><a href="/en-US/docs/Web/API/Canvas_API/Manipulating_video_using_canvas">Manipulating video using canvas</a></dt>
 <dd>Combining {{HTMLElement("video")}} and {{HTMLElement("canvas")}} to manipulate video data in real time.</dd>
</dl>

<h2 id="Resources">Resources</h2>

<h3 id="Generic">Generic</h3>

<ul>
 <li><a href="http://joshondesign.com/p/books/canvasdeepdive/title.html">HTML5 Canvas Deep Dive</a></li>
 <li><a href="http://bucephalus.org/text/CanvasHandbook/CanvasHandbook.html">Canvas Handbook</a></li>
</ul>

<h3 id="Libraries">Libraries</h3>

<ul>
 <li><a href="http://fabricjs.com">Fabric.js</a> is an open-source canvas library with SVG parsing capabilities.</li>
 <li><a href="https://github.com/ericdrowell/KineticJS">Kinetic.js</a>&nbsp;is an open-source canvas library focused on&nbsp;interactivity for desktop and mobile applications.</li>
 <li><a href="http://paperjs.org/">Paper.js</a> is an open source vector graphics scripting framework that runs on top of the HTML5 Canvas.</li>
 <li><a href="http://origamijs.com/docs/">Origami.js</a> is an open source&nbsp;lightweight canvas library.</li>
 <li><a href="http://libcanvas.github.com/">libCanvas</a> is powerful and lightweight canvas framework.</li>
 <li><a href="https://p5js.org/">p5.js </a>has a full set of canvas drawing functionality for artists, designers, educators and beginners.</li>
 <li><a href="http://processingjs.org">Processing.js</a> is a port of the Processing visualization language.</li>
 <li><a href="https://playcanvas.com/">PlayCanvas</a> is an open source game engine.</li>
 <li><a href="http://www.pixijs.com/">Pixi.js</a> is an open source game engine.</li>
 <li><a href="http://www.liquidx.net/plotkit/">PlotKit</a> is a charting and graphing library.</li>
 <li><a class="link-https" href="https://github.com/jeremyckahn/rekapi">Rekapi</a> is an animation key-framing API for Canvas.</li>
 <li><a href="http://senchalabs.github.com/philogl/">PhiloGL</a> is a WebGL framework for data visualization, creative coding and game development.</li>
 <li><a href="http://thejit.org/">JavaScript InfoVis Toolkit</a> creates interactive 2D Canvas data visualizations for the Web.</li>
 <li><a href="http://www.createjs.com/easeljs">EaselJS</a> is a free/open source library to make it easier to use canvas for games and art</li>
 <li><a href="http://scrawl.rikweb.org.uk/">Scrawl-canvas</a> is another open-source javascript library for creating and manipulating 2d canvas elements</li>
 <li><a href="https://www.patrick-wied.at/static/heatmapjs/">heatmap.js</a> is an open source library to create canvas based heatmaps</li>
 <li>The <a href="http://zimjs.com">ZIM</a> framework provides conveniences, components and controls for coding creativity on the canvas — includes accessibility and hundreds of colorful tutorials.</li>
</ul>

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
   <td>{{SpecName('HTML WHATWG', 'scripting.html#the-canvas-element', '&lt;canvas&gt;')}}</td>
   <td>{{Spec2('HTML WHATWG')}}</td>
   <td>&nbsp;</td>
  </tr>
 </tbody>
</table>

<h2 id="See_also">See also</h2>

<ul>
 <li><a href="/en-US/docs/Web/WebGL">WebGL</a></li>
</ul>

