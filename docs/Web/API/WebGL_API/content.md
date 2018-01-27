---
version: prototype1
revision_id: 1351303
locale: en-US
slug: Web/API/WebGL_API
tags: "3D" "WebGL" "WebGL API" "Media" "3D Graphics" "Advanced" "Graphics" "Overview"
title: The WebGL API: 2D and 3D graphics for the web
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{WebGLSidebar}}</div>

<div class="summary">
<p>WebGL (Web Graphics Library) is a JavaScript API for rendering interactive 3D and 2D graphics within any compatible web browser without the use of plug-ins. WebGL does so by introducing an API that closely conforms to OpenGL ES 2.0 that can be used in HTML5 {{HTMLElement("canvas")}} elements.</p>
</div>

<p>Support for WebGL is present in <a href="/en-US/Firefox" title="Firefox 4 for developers">Firefox</a>&nbsp;4+, <a href="http://www.google.com/chrome/" title="http://www.google.com/chrome/">Google Chrome</a> 9+, <a href="http://www.opera.com/" title="http://www.opera.com/">Opera</a>&nbsp;12+, <a href="http://www.apple.com/safari/" title="http://www.apple.com/fr/safari/">Safari </a>5.1+, <a href="http://windows.microsoft.com/en-us/internet-explorer/browser-ie" title="http://windows.microsoft.com/en-us/internet-explorer/download-ie">Internet Explorer</a> 11+, and <a href="https://www.microsoft.com/en-us/windows/microsoft-edge">Microsoft Edge</a> build 10240+; however, the user's device must also have hardware that supports these features.</p>

<p>The {{HTMLElement("canvas")}} element is also used by <a href="/en-US/docs/Web/API/Canvas_API">Canvas 2D</a> to do 2D graphics on web pages.</p>

<h2 id="Reference">Reference</h2>

<h3 id="Standard_interfaces">Standard interfaces</h3>

<div class="index">
<ul>
 <li>{{domxref("WebGLRenderingContext")}}</li>
 <li>{{domxref("WebGL2RenderingContext")}} {{experimental_inline}}</li>
 <li>{{domxref("WebGLActiveInfo")}}</li>
 <li>{{domxref("WebGLBuffer")}}</li>
 <li>{{domxref("WebGLContextEvent")}}</li>
 <li>{{domxref("WebGLFramebuffer")}}</li>
 <li>{{domxref("WebGLProgram")}}</li>
 <li>{{domxref("WebGLQuery")}} {{experimental_inline}}</li>
 <li>{{domxref("WebGLRenderbuffer")}}</li>
 <li>{{domxref("WebGLSampler")}} {{experimental_inline}}</li>
 <li>{{domxref("WebGLShader")}}</li>
 <li>{{domxref("WebGLShaderPrecisionFormat")}}</li>
 <li>{{domxref("WebGLSync")}} {{experimental_inline}}</li>
 <li>{{domxref("WebGLTexture")}}</li>
 <li>{{domxref("WebGLTransformFeedback")}} {{experimental_inline}}</li>
 <li>{{domxref("WebGLUniformLocation")}}</li>
 <li>{{domxref("WebGLVertexArrayObject")}} {{experimental_inline}}</li>
</ul>
</div>

<h3 id="Extensions">Extensions</h3>

<div class="index">
<ul>
 <li>{{domxref("ANGLE_instanced_arrays")}}</li>
 <li>{{domxref("EXT_blend_minmax")}}</li>
 <li>{{domxref("EXT_color_buffer_float")}}</li>
 <li>{{domxref("EXT_color_buffer_half_float")}}</li>
 <li>{{domxref("EXT_disjoint_timer_query")}}</li>
 <li>{{domxref("EXT_frag_depth")}}</li>
 <li>{{domxref("EXT_sRGB")}}</li>
 <li>{{domxref("EXT_shader_texture_lod")}}</li>
 <li>{{domxref("EXT_texture_filter_anisotropic")}}</li>
 <li>{{domxref("OES_element_index_uint")}}</li>
 <li>{{domxref("OES_standard_derivatives")}}</li>
 <li>{{domxref("OES_texture_float")}}</li>
 <li>{{domxref("OES_texture_float_linear")}}</li>
 <li>{{domxref("OES_texture_half_float")}}</li>
 <li>{{domxref("OES_texture_half_float_linear")}}</li>
 <li>{{domxref("OES_vertex_array_object")}}</li>
 <li>{{domxref("WEBGL_color_buffer_float")}}</li>
 <li>{{domxref("WEBGL_compressed_texture_astc")}}</li>
 <li>{{domxref("WEBGL_compressed_texture_atc")}}</li>
 <li>{{domxref("WEBGL_compressed_texture_etc")}}</li>
 <li>{{domxref("WEBGL_compressed_texture_etc1")}}</li>
 <li>{{domxref("WEBGL_compressed_texture_pvrtc")}}</li>
 <li>{{domxref("WEBGL_compressed_texture_s3tc")}}</li>
 <li>{{domxref("WEBGL_compressed_texture_s3tc_srgb")}}</li>
 <li>{{domxref("WEBGL_debug_renderer_info")}}</li>
 <li>{{domxref("WEBGL_debug_shaders")}}</li>
 <li>{{domxref("WEBGL_depth_texture")}}</li>
 <li>{{domxref("WEBGL_draw_buffers")}}</li>
 <li>{{domxref("WEBGL_lose_context")}}</li>
</ul>
</div>

<h3 id="Events">Events</h3>

<ul>
 <li>{{Event("webglcontextlost")}}</li>
 <li>{{Event("webglcontextrestored")}}</li>
 <li>{{Event("webglcontextcreationerror")}}</li>
</ul>

<h3 id="Constants_and_types">Constants and types</h3>

<ul>
 <li><a href="/en-US/docs/Web/API/WebGL_API/Constants">WebGL constants</a></li>
 <li><a href="/en-US/docs/Web/API/WebGL_API/Types">WebGL types</a></li>
</ul>

<h3 id="WebGL_2">WebGL 2</h3>

<p>WebGL 2 is a major update to WebGL which is provided through the {{domxref("WebGL2RenderingContext")}} interface. It is based on OpenGL ES 3.0 and new features include:</p>

<ul>
 <li><a href="/en-US/docs/Web/API/WebGL2RenderingContext/texImage3D">3D textures</a>,</li>
 <li><a href="/en-US/docs/Web/API/WebGLSampler">Sampler objects</a>,</li>
 <li><a href="/en-US/docs/Web/API/WebGL2RenderingContext#Uniform_buffer_objects">Uniform Buffer objects</a>,</li>
 <li><a href="/en-US/docs/Web/API/WebGLSync">Sync objects</a>,</li>
 <li><a href="/en-US/docs/Web/API/WebGLQuery">Query objects</a>,</li>
 <li><a href="/en-US/docs/Web/API/WebGLTransformFeedback">Transform Feedback objects</a>,</li>
 <li>Promoted extensions that are now core to WebGL 2: <a href="/en-US/docs/Web/API/WebGLVertexArrayObject">Vertex Array objects</a>, <a href="/en-US/docs/Web/API/WebGL2RenderingContext/drawArraysInstanced">instancing</a>, <a href="/en-US/docs/Web/API/WebGL2RenderingContext/drawBuffers">multiple render targets</a>, <a href="/en-US/docs/Web/API/EXT_frag_depth">fragment depth</a>.</li>
</ul>

<p>See also the blog post <a href="https://hacks.mozilla.org/2017/01/webgl-2-lands-in-firefox/">"WebGL 2 lands in Firefox"</a> and <a href="http://webglsamples.org/WebGL2Samples/">webglsamples.org/WebGL2Samples</a> for a few demos.</p>

<h2 id="Guides_and_tutorials">Guides and tutorials</h2>

<p>Below, you'll find an assortment of guides to help you learn WebGL concepts and tutorials that offer step-by-step lessons and examples.</p>

<h3 id="Guides">Guides</h3>

<dl>
 <dt><a href="/en-US/docs/Web/API/WebGL_API/Data">Data in WebGL</a></dt>
 <dd>A guide to variables, buffers, and other types of data used when writing WebGL code.</dd>
 <dt><a href="/en-US/docs/Web/API/WebGL_API/WebGL_best_practices">WebGL best practices</a></dt>
 <dd>Tips and suggestions to help you improve the quality, performance, and reliability of your WebGL content.</dd>
 <dt><a href="/en-US/docs/Web/API/WebGL_API/Using_Extensions">Using extensions</a></dt>
 <dd>A guide to using WebGL extensions.</dd>
</dl>

<h3 id="Tutorials">Tutorials</h3>

<dl>
 <dt><a href="/en-US/docs/Web/API/WebGL_API/Tutorial">WebGL tutorial</a></dt>
 <dd>A beginner's guide to WebGL core concepts. A good place to start if you don't have previous WebGL experience.</dd>
</dl>

<h3 id="Examples">Examples</h3>

<dl>
 <dt><a href="/en-US/docs/Web/API/WebGL_API/Basic_2D_animation_example">A basic 2D WebGL animation example</a></dt>
 <dd>This example demonstrates the simple animation of a one-color shape. Topics examined are adapting to aspect ratio differences, a function to build shader programs from sets of multiple shaders, and the basics of drawing in WebGL.</dd>
</dl>

<h3 id="Advanced_tutorials">Advanced tutorials</h3>

<dl>
 <dt><a href="/en-US/docs/Web/API/WebGL_API/WebGL_model_view_projection">WebGL model view projection</a></dt>
 <dd>A detailed explanation of the three core matrices that are typically used to represent a 3D object view: the model, view and projection matrices.</dd>
 <dt><a href="/en-US/docs/Web/API/WebGL_API/Matrix_math_for_the_web">Matrix math for the web</a></dt>
 <dd>A useful guide to how 3D transform matrices work, and can be used on the web — both for WebGL calculations and in CSS3 transforms.</dd>
</dl>

<h2 id="Resources">Resources</h2>

<ul>
 <li><a href="https://www.youtube.com/embed/H4c8t6myAWU/?feature=player_detailpage">Raw WebGL: An introduction to WebGL</a> A talk by Nick Desaulniers that introduces the basics of WebGL. This is a great place to start if you've never done low-level graphics programming.</li>
 <li><a href="http://www.khronos.org/webgl/" title="http://www.khronos.org/webgl/">Khronos WebGL site</a> The main web site for WebGL at the Khronos Group.</li>
 <li><a href="http://learningwebgl.com/blog/?page_id=1217" title="http://learningwebgl.com/blog/">Learning WebGL</a> A site with tutorials on how to use WebGL.</li>
 <li><a href="http://www.html5rocks.com/en/tutorials/webgl/webgl_fundamentals/" title="http://www.html5rocks.com/en/tutorials/webgl/webgl_fundamentals/">WebGL Fundamentals</a> A basic tutorial with fundamentals of WebGL.</li>
 <li><a href="http://webglplayground.net" title="http://webglplayground.net">WebGL playground</a> An online tool for creating and sharing WebGL projects. Good for quick prototyping and experimenting.</li>
 <li><a href="http://www.webglacademy.com" title="http://www.webglacademy.com">WebGL Academy</a> An HTML/JavaScript editor with tutorials to learn basics of webgl programming.</li>
 <li><a href="http://webglstats.com/">WebGL Stats</a> A site with statistics about WebGL capabilities in browsers on different platforms.</li>
</ul>

<h3 id="Libraries">Libraries</h3>

<ul>
 <li><a class="link-https" href="https://github.com/toji/gl-matrix" title="https://github.com/toji/gl-matrix">glMatrix</a> JavaScript Matrix and Vector library for High Performance WebGL apps</li>
 <li><a href="http://sylvester.jcoglan.com/" title="http://sylvester.jcoglan.com/">Sylvester</a> An open source library for manipulating vectors and matrices. Not optimized for WebGL but extremely robust.</li>
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
   <td>{{SpecName('WebGL')}}</td>
   <td>{{Spec2('WebGL')}}</td>
   <td>Initial definition. Based on OpenGL ES 2.0</td>
  </tr>
  <tr>
   <td>{{SpecName('WebGL2')}}</td>
   <td>{{Spec2('WebGL2')}}</td>
   <td>Builds on top of WebGL 1. Based on OpenGL ES 3.0.</td>
  </tr>
  <tr>
   <td>{{SpecName('OpenGL ES 2.0')}}</td>
   <td>{{Spec2('OpenGL ES 2.0')}}</td>
   <td>&nbsp;</td>
  </tr>
  <tr>
   <td>{{SpecName('OpenGL ES 3.0')}}</td>
   <td>{{Spec2('OpenGL ES 3.0')}}</td>
   <td>&nbsp;</td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<div>{{CompatibilityTable}}</div>

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
   <td>9</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatGeckoDesktop("2.0")}}</td>
   <td>11</td>
   <td>12</td>
   <td>5.1</td>
  </tr>
  <tr>
   <td>WebGL 2</td>
   <td>56</td>
   <td>{{CompatNo}}</td>
   <td>{{CompatGeckoDesktop("51")}}</td>
   <td>{{CompatNo}}</td>
   <td>43</td>
   <td>{{CompatNo}}</td>
  </tr>
 </tbody>
</table>
</div>

<div id="compat-mobile">
<table class="compat-table">
 <tbody>
  <tr>
   <th>Feature</th>
   <th>Chrome for Android</th>
   <th>Edge</th>
   <th>Firefox Mobile (Gecko)</th>
   <th>IE Mobile</th>
   <th>Opera Mobile</th>
   <th>Safari Mobile</th>
  </tr>
  <tr>
   <td>Basic support</td>
   <td>25</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>4</td>
   <td>{{CompatNo}}</td>
   <td>12</td>
   <td>8.1</td>
  </tr>
  <tr>
   <td>WebGL 2</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatUnknown}}</td>
   <td>{{CompatUnknown}}</td>
  </tr>
 </tbody>
</table>
</div>

<h3 id="Compatibility_notes">Compatibility notes</h3>

<p>In addition to the browser, the GPU itself also needs to support the feature. So, for example, S3 Texture Compression (S3TC) is only available on Tegra-based tablets. Most browsers make the WebGL context available through the <code>webgl</code> context name, but older ones need <code>experimental-webgl</code> as well. In addition, the upcoming <a href="/en-US/docs/Web/API/WebGL2RenderingContext">WebGL 2</a> is fully backwards-compatible and will have the context name <code>webgl2</code>.</p>

<h3 id="Gecko_notes">Gecko notes</h3>

<h4 id="WebGL_debugging_and_testing">WebGL debugging and testing</h4>

<p>Starting with Gecko 10.0 {{geckoRelease("10.0")}}, there are two preferences available which let you control the capabilities of WebGL for testing purposes:</p>

<dl>
 <dt><code>webgl.min_capability_mode</code></dt>
 <dd>A Boolean property that, when <code>true</code>, enables a minimum capability mode. When in this mode, WebGL is configured to only support the bare minimum feature set and capabilities required by the WebGL specification. This lets you ensure that your WebGL code will work on any device or browser, regardless of their capabilities. This is <code>false</code> by default.</dd>
 <dt><code>webgl.disable_extensions</code></dt>
 <dd>A Boolean property that, when <code>true</code>, disables all WebGL extensions. This is <code>false</code> by default.</dd>
</dl>

<h2 id="See_also">See also</h2>

<ul>
 <li><a href="/en-US/docs/Web/API/Canvas_API">Canvas</a></li>
 <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/WebGLRenderingContext/getSupportedExtensions#Browser_compatibility">Compatibility info about WebGL extensions</a></li>
</ul>

