---
version: prototype1
revision_id: 1322932
locale: en-US
slug: Web/CSS/Media_Queries
tags: "CSS" "Overview" "Reference" "CSS3 Media Queries" "Media Queries" "Responsive Design"
title: Media queries
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{CSSRef("CSS3 Media Queries")}}</div>

<p><strong>Media queries</strong> are a key component of <a href="/en-US/docs/Web/Apps/Progressive/Responsive">responsive design</a>, which make it possible for CSS to adapt based on various parameters or device characteristics. For example, a media query can apply different styles if the screen is smaller than a certain size, or based on whether the user is holding their device in portrait or landscape mode. The {{cssxref("@media")}} at-rule is used to conditionally apply styles to a document.</p>

<p>In addition, the media query syntax is also used in other contexts, such as in the {{HTMLElement("source")}} element's {{htmlattrxref("media", "source")}} attribute, which can be set to a media query string to use to determine whether or not to use that source when selecting the specific image to use in a {{HTMLElement("picture")}} element.</p>

<p>In addition, the {{domxref("Window.matchMedia()")}} method can be used to test the window against a media query. You can also use {{domxref("MediaQueryList.addListener()")}} to be notified whenever the state of the queries changes. With this functionality, your site or app can respond to changes in the device configuration, orientation, or state.</p>

<p>You can learn more about programmatically using media queries in <a href="/en-US/docs/Web/CSS/Media_Queries/Testing_media_queries">Testing media queries</a>.</p>

<h2 id="Reference">Reference</h2>

<h3 id="At-rules">At-rules</h3>

<div class="index">
<ul>
 <li>{{cssxref("@import")}}</li>
 <li>{{cssxref("@media")}}</li>
</ul>
</div>

<h2 id="Guides">Guides</h2>

<dl>
 <dt><a href="/en-US/docs/Web/CSS/Media_Queries/Using_media_queries">Using media queries</a></dt>
 <dd>Introduces media queries, their syntax, and the operators and media features which are used to construct media query expressions.</dd>
 <dt><a href="/en-US/docs/Web/CSS/Media_Queries/Testing_media_queries">Testing media queries</a></dt>
 <dd>Describes how to test media queries from your JavaScript code, programmatically, to determine the state of the device, and to set up listeners that let your code be notified when the results of media queries change (such as when the user rotates the screen, causing an orientation change).</dd>
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
   <td>{{SpecName('CSS3 Conditional')}}</td>
   <td>{{Spec2('CSS3 Conditional')}}</td>
   <td>&nbsp;</td>
  </tr>
  <tr>
   <td>{{SpecName('CSS4 Media Queries')}}</td>
   <td>{{Spec2('CSS4 Media Queries')}}</td>
   <td>&nbsp;</td>
  </tr>
  <tr>
   <td>{{SpecName('CSS3 Media Queries')}}</td>
   <td>{{Spec2('CSS3 Media Queries')}}</td>
   <td>&nbsp;</td>
  </tr>
  <tr>
   <td>{{SpecName('CSS2.1', 'media.html')}}</td>
   <td>{{Spec2('CSS2.1')}}</td>
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
   <td>1.0</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatGeckoDesktop(1.7)}}</td>
   <td>9.0</td>
   <td>9.2</td>
   <td>1.3</td>
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
   <th>Edge</th>
   <th>Firefox Mobile (Gecko)</th>
   <th>IE Mobile</th>
   <th>Opera Mobile</th>
   <th>Safari Mobile</th>
  </tr>
  <tr>
   <td>Basic support</td>
   <td>1.0</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatGeckoMobile(1.7)}}</td>
   <td>9.0</td>
   <td>9.0</td>
   <td>3.1</td>
  </tr>
 </tbody>
</table>
</div>

