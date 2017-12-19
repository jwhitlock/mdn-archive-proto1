---
version: prototype1
revision_id: 1337983
locale: en-US
slug: MDN/About/Promote
tags: "MDN Meta" "Guide"
title: Promote MDN
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{IncludeSubnav("/en-US/docs/MDN")}}</div>

<p>Love MDN? Help share the open-Web goodness with fellow web developers by promoting MDN! We have some ideas of ways you can do that.&nbsp; We also have wallpapers, stickers, posters, animations, website badges, you name it; link to it from here.</p>

<div class="callout-box">Want to know more <a href="/en-US/docs/MDN/About" title="Project:en/About">about MDN</a> or <a href="/en-US/docs/MDN/Contribute" title="Project:en/How_to_Help">how to help</a> make a great reference Wiki for web technologies?</div>

<h2 id="Share_links_on_social_media">Share links on social media</h2>

<p>Did you find an article on MDN especially helpful? Share it on <a href="https://twitter.com/">Twitter</a>, <a href="https://www.facebook.com/">Facebook</a>, <a href="https://news.ycombinator.com/">Hacker News</a>, <a href="https://www.reddit.com/">reddit</a>, or wherever you share cool stuff you like. It's great if you let us know at <a href="https://twitter.com/MozDevNet">@MozDevNet</a>, but certainly not required.</p>

<h2 id="Answer_questions_with_MDN_links">Answer questions with MDN links</h2>

<p>Whether the question is on <a href="http://stackoverflow.com/">Stack Overflow</a>, someone is shouting it to the <a href="https://twitter.com/">Twitterverse</a>, or your coworker is asking in your team's Slack channel, often answers to questions about web development can be found on MDN. Help the questioner find the best information about web development by sharing a link to MDN that answers their question.</p>

<h2 id="Cite_MDN_in_technical_talks">Cite MDN in technical talks</h2>

<p>Whether you're speaking to your local JavaScript meetup group or at a major technical conference, often MDN has articles that complement your topic, or provide further background to your audience. If your presentation is available online,&nbsp; it would be great if you could give us a shout at <a href="https://twitter.com/MozDevNet">@MozDevNet</a> with the link. But the most important thing is that you share great information with people who need it.</p>

<h2 id="WordPress_plugin">WordPress plugin</h2>

<p>The <a href="http://wordpress.org/plugins/promote-mdn/">Promote MDN plugin for WordPress</a> blogs is available to help people who blog about Web technologies or Mozilla-related products both promote their own blogs as well as MDN itself. It works in two ways:</p>

<ol>
 <li>When you publish a blog post, it automatically links key terms (such as "HTML", "JavaScript", and "CSS", among others) to the appropriate pages on MDN. This lets you write about Web technologies and automatically link to relevant documentation without having to do anything yourself. It's incredibly useful! The terms and their destination pages on MDN are configured in the def-list branch of the GitHub repo<a href="https://github.com/mdn/wp-promote-mdn/tree/def-list">https://github.com/mdn/wp-promote-mdn/tree/def-list</a>.</li>
</ol>

<p>Installing this plugin is helpful to you and to MDN both, so if you haven't already installed it, <a href="http://wordpress.org/plugins/promote-mdn/installation/">you should</a>! If you want to help code on the plugin, go to the <a href="https://github.com/mdn/wp-promote-mdn">wp-promote-mdn GitHub repo</a>.</p>

<h2 id="JavaScript_snippet">JavaScript snippet</h2>

<p>The recommended way to automatically link keywords to MDN pages is the Promote MDN WordPress plugin given above, but if your site or blog isn't running on WordPress, you can embed the JavaScript code below to do the same thing. This script does the same thing as the WordPress plugin; it converts known keywords in the page's content into links to the appropriate documentation on MDN.</p>

<p>You can configure the maximum number of keywords to turn into links by changing the value of <code>maxLinks</code> in the options object, <code>o</code>. You can also specify the elements to search, the class to use for the created link, and a set of additional keywords and target URLs to scan for.</p>

<p>To use this snippet, just embed it right before your closing <code>&lt;/body&gt;</code> tag at the end of your content.</p>

<pre class="brush: html">
&lt;script type="text/javascript" &gt;
&nbsp;&nbsp;&nbsp; (function (d,f,a) {
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // Your settings here
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; var o = {maxLinks: 4, searchElements: ['div', 'h'], linkClass: 'link-to-mdn', extraLinks: {'keywordx': 'http://example.com'}};

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; var s=d.createElement("script");s.type="text/javascript";if(s.f)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; {s.a=function(){if(s.f=="loaded"||s.f=="complete")
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; {s.a=null;PromoteMDN(o)}}}else{s.onload=function()
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; {PromoteMDN(o)}}s.src="https://raw.githubusercontent.com/riverspirit/promote-mdn-script/master/promote-mdn.js";
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; d.getElementsByTagName("head")[0].appendChild(s)
&nbsp;&nbsp;&nbsp; })(document,'readyState','onreadystatechange');
&lt;/script&gt;</pre>

<p>This snippet loads the primary code that does all the real work from Github. If you would prefer to host that code on your server yourself (for security, performance, etc.), just <a href="https://github.com/riverspirit/promote-mdn-script">download the code from Github</a>, add it to your site, and adjust the URL on line 9 of the code above to match.</p>

<h2 id="Web_site_banner_images">Web site banner images</h2>

<p>If you'd like to link to MDN from your web site using a promotional image, we have a number of them to choose from:</p>

<table class="standard-table">
 <tbody>
  <tr>
   <td><img alt="MDN Banner: 240x240px" src="https://mdn.mozillademos.org/files/15712/240x240%202alt-1%20-%20v2.png" style="height:240px; width:240px" /></td>
   <td><img alt="Better Docs for a Better Web" src="https://mdn.mozillademos.org/files/15713/240x480-1v2.png" style="height:480px; width:240px" /></td>
  </tr>
  <tr>
   <td><img alt="By Developers for Developers" src="https://mdn.mozillademos.org/files/15715/240x480-2v2.png" style="height:480px; width:240px" /></td>
   <td><img alt="Better Docs for a Better Web" src="https://mdn.mozillademos.org/files/15714/240x480-1.2v2.png" style="height:480px; width:240px" /></td>
  </tr>
 </tbody>
</table>

<p>Feel free to use these on your web site to link to MDN!</p>

<h2 id="Desktop_wallpapers">Desktop wallpapers</h2>

<p><img class="internal" src="/@api/deki/files/275/=Moz_ffx_openStandards_264x198.jpg" /></p>

<p>First designed at the 2006 Firefox Developer's Summit by Sean Martell based on an idea from Chris Beard, this graphic became a smash hit at the SXSW conference in 2007. Now available as a desktop wallpaper in a variety of sizes:</p>

<ul>
 <li><a class="superZoomLink" href="/@api/deki/files/276/=Moz_ffx_openStandards_800x600.jpg" title="File:en/Media_Gallery/Moz_ffx_openStandards_800x600.jpg">800x600 pixels</a></li>
 <li><a class="superZoomLink" href="/@api/deki/files/271/=Moz_ffx_openStandards_1024x768.jpg" title="File:en/Media_Gallery/Moz_ffx_openStandards_1024x768.jpg">1024x768 pixels</a></li>
 <li><a class="superZoomLink" href="/@api/deki/files/272/=Moz_ffx_openStandards_1280x1024.jpg" title="File:en/Media_Gallery/Moz_ffx_openStandards_1280x1024.jpg">1280x1024 pixels</a></li>
 <li><a class="superZoomLink" href="/@api/deki/files/273/=Moz_ffx_openStandards_1440x900.jpg" title="File:en/Media_Gallery/Moz_ffx_openStandards_1440x900.jpg">1440x900 pixels</a></li>
 <li><a class="superZoomLink" href="/@api/deki/files/274/=Moz_ffx_openStandards_1680x1050.jpg" title="File:en/Media_Gallery/Moz_ffx_openStandards_1680x1050.jpg">1680x1050 pixels</a></li>
</ul>

<p><small>These wallpapers are available for use under the terms of the <a class="external" href="http://creativecommons.org/licenses/by-nc/3.0/">Creative Commons Attribution-NonCommercial</a> license. These wallpapers are also covered by the <a class="external" href="http://www.mozilla.org/foundation/trademarks/policy.html">Mozilla Trademark Policy</a>. </small></p>
