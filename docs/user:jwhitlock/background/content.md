---
version: prototype1
revision_id: 1328480
locale: en-US
slug: user:jwhitlock/background
tags: 
title: background
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p><em>From https://developer.mozilla.org/en-US/Add-ons/WebExtensions/manifest.json/background</em></p>

<div>{{AddonSidebar}}</div>

<table class="fullwidth-table standard-table">
 <tbody>
  <tr>
   <th scope="row" style="width: 30%;">Type</th>
   <td><code>Object</code></td>
  </tr>
  <tr>
   <th scope="row">Mandatory</th>
   <td>No</td>
  </tr>
  <tr>
   <th scope="row">Example</th>
   <td>
    <pre class="brush: json no-line-numbers">
"background": {
  "scripts": ["background.js"]
}</pre>
   </td>
  </tr>
 </tbody>
</table>

<p>Use the <code>background</code> key to include one or more background scripts, and optionally a background page in your extension.</p>

<p>Background scripts are the place to put code that needs to maintain long-term state, or perform long-term operations, independently of the lifetime of any particular web pages or browser windows.</p>

<p>Background scripts are loaded as soon as the extension is loaded and stay loaded until the extension is disabled or uninstalled. You can use any of the WebExtension APIs in the script, as long as you have requested the necessary <a href="/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json/permissions">permissions</a>.</p>

<p>See the "Background pages" section in <a href="/en-US/Add-ons/WebExtensions/Anatomy_of_a_WebExtension#Background_pages">Anatomy of an extension</a> for some more details.</p>

<p>The <code>background</code> key is an object that may have one of the following two properties, both optional:</p>

<table class="standard-table">
 <tbody>
  <tr>
   <td><code>"scripts"</code></td>
   <td>
    <p>An array of strings, each of which is a path to a JavaScript source. The path is relative to the manifest.json file itself. These are the background scripts that will be included in the extension.</p>

    <p>The scripts share the same <code>window</code> global.</p>

    <p>The scripts are loaded in the order they appear in the array.</p>

    <p><strong>Note that there is a bug affecting Firefox versions earlier than 50</strong>: when the Firefox debugger is open, scripts are not always loaded in the order given in the array. To work around this bug, you can use the <code>"page"</code> property and include background scripts from the page using <code>&lt;script&gt;</code> tags. This bug is fixed in Firefox 50, and from that point on, scripts are always loaded in the order given in the array.</p>

    <div class="note">
    <p><strong>Note:</strong> If you want to fetch a script from a remote location with the <code>&lt;script&gt;</code> tag (e.g. <code>&lt;script src = "https://code.jquery.com/jquery-1.7.1.min.js"&gt;</code>), you will also have to change the <code>content_security_policy</code> key in the manifest.json file of your extension.</p>
    </div>
   </td>
  </tr>
  <tr>
   <td><code>"page"</code></td>
   <td>
    <p>If you specify <code>"scripts"</code>, then an empty page will be created for your scripts to run in.</p>

    <p>If you need some particular content in the page, you can define your own page using the <code>"page"</code> option.</p>

    <p>If you use this property, you can no longer specify background scripts using <code>"scripts"</code>, but you can&nbsp; include your own scripts from the page, just like in a normal web page.</p>
   </td>
  </tr>
 </tbody>
</table>

<h2 id="Example">Example</h2>

<pre class="brush: json no-line-numbers">
&nbsp; "background": {
&nbsp;&nbsp;&nbsp; "scripts": ["jquery.js", "my-background.js"]
&nbsp; }</pre>

<p>Load two background scripts.</p>

<pre class="brush: json">
  "background": {
    "page": "my-background.html"
  }</pre>

<p>Load a custom background page.</p>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<p class="hidden">The compatibility table in this page is generated from structured data. If you'd like to contribute to the data, please check out <a href="https://github.com/mdn/browser-compat-data">https://github.com/mdn/browser-compat-data</a> and send us a pull request.</p>

<p>{{Compat("webextensions.manifest.background", 10)}}</p>

