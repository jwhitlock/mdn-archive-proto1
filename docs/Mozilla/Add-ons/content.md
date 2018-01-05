---
version: prototype1
revision_id: 1343354
locale: en-US
slug: Mozilla/Add-ons
tags: "Add-ons" "Landing" "Mozilla" "Extension" "Extensions"
title: Add-ons
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<div>&nbsp;</div>

<p><span class="seoSummary">Add-ons allow developers to extend and modify the functionality of Firefox.</span> They are written using standard Web technologies - JavaScript, HTML, and CSS - plus some dedicated JavaScript APIs. Among other things, an add-on could:</p>

<ul>
 <li>Change the appearance or content of particular websites</li>
 <li>Modify the Firefox user interface</li>
 <li>Add new features to Firefox</li>
</ul>

<p>There are several types of add-ons, but the most common type are extensions.</p>

<h2 id="Developing_extensions">Developing extensions</h2>

<p>In the past, there were several toolsets for developing Firefox extensions, but by the end of November 2017, extensions must be built using <a href="https://developer.mozilla.org/en-US/Add-ons/WebExtensions">WebExtensions APIs</a>. Other toolsets, such as overlay add-ons, bootstrapped add-ons, and the Add-on SDK, will be deprecated over the same period of time.</p>

<p>If you are writing a new extension, use <a href="https://developer.mozilla.org/en-US/Add-ons/WebExtensions">WebExtensions APIs</a>.</p>

<p>Extensions written using WebExtensions APIs for Firefox are designed to be cross-browser compatible. In most cases it will run in Chrome, Edge, and Opera with few if any changes. They are also fully compatible with multiprocess Firefox.<br />
 <br />
 <a href="https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">See the APIs currently supported in Firefox and other browsers</a>. We're continuing to design and implement new APIs in response to developer needs.<br />
 <br />
 Most of the WebExtensions APIs are also available on Firefox for Android.</p>

<h3 id="Migrate_an_existing_extension">Migrate an existing extension</h3>

<p>If you maintain a legacy extension, such as a XUL overlay, bootstrapped, or Add-on SDK-based extension, you can still port it to use WebExtension APIs.&nbsp; There are some <a href="/en-US/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">porting resources on MDN</a>.</p>

<p>For more information about transition support, please visit our <a href="/en-US/docs/">wiki page.</a></p>

<h2 id="Publishing_add-ons">Publishing add-ons</h2>

<p><a href="https://addons.mozilla.org">Addons.mozilla.org</a>, commonly known as "AMO," is Mozilla's official site for developers to list add-ons, and for users to discover them. By uploading your add-on to AMO, you can participate in our community of users and creators, and find an audience for your add-on.</p>

<p>You are not required to list your add-on on AMO, but your add-on must be signed by Mozilla or users won't be able to install it.</p>

<p>For an overview of the process of publishing your add-on, see <a href="https://developer.mozilla.org/en-US/Add-ons/Distribution">Signing and distributing your add-on</a>.</p>

<h2 id="Other_types_of_add-ons">Other types of add-ons</h2>

<p>In addition to extensions, there are a few other add-on types that allow users to customize Firefox. Those add-ons include:</p>

<ul>
 <li><a href="https://developer.mozilla.org/Add-ons/Themes/Background">Lightweight themes</a> are a simple way to provide limited customization for Firefox.</li>
 <li><a href="/en-US/Add-ons/Firefox_for_Android">Mobile add-ons</a> are for&nbsp;Firefox for Android. Note, though, that we intend to deprecate some of the technology underlying these APIs. In the future, WebExtensions APIs will be fully supported to an extent on Firefox for Android.</li>
 <li><a href="/en-US/docs/Creating_OpenSearch_plugins_for_Firefox">Search engine plugins</a> add new search engines to the browser's search bar.</li>
 <li><a href="/en-US/docs/Mozilla/Creating_a_spell_check_dictionary_add-on">User dictionaries</a> let you spell-check in different languages.</li>
 <li><a href="https://support.mozilla.org/kb/use-firefox-interface-other-languages-language-pack">Language packs</a> let you have more languages available for the user interface of Firefox.</li>
</ul>

<hr />
<h2 id="Contact_us">Contact us</h2>

<p>You can use the links below to get help, keep up to date with news around add-ons, and give us feedback.</p>

<h3 id="Add-ons_forum">Add-ons forum</h3>

<p>Use the <a href="https://discourse.mozilla.org/c/add-ons">Add-ons Discourse forum</a> to discuss all aspects of add-on development and to get help.</p>

<h3 id="Mailing_lists">Mailing lists</h3>

<p>Use the <strong>dev-addons</strong> list to discuss development of the add-ons ecosystem, including the development of the WebExtensions system and of AMO:</p>

<ul>
 <li><a href="https://mail.mozilla.org/listinfo/dev-addons">dev-addons list info</a></li>
 <li><a href="https://mail.mozilla.org/pipermail/dev-addons/">dev-addons archives</a></li>
</ul>

<h3 id="IRC">IRC</h3>

<p>If you're a fan of IRC, you can get in touch at:</p>

<ul>
 <li><a href="irc://irc.mozilla.org/addons">#addons</a> (discussion of the add-ons ecosystem)</li>
 <li><a href="irc://irc.mozilla.org/extdev">#extdev</a> (general discussion of add-on development)</li>
 <li><a href="irc://irc.mozilla.org/webextensions">#webextensions</a> (discussion around the WebExtensions API in particular)</li>
</ul>

<h3 id="Report_problems">Report problems</h3>

<h4 id="Security_vulnerabilities">Security vulnerabilities</h4>

<p>If you discover a security vulnerability in an add-on, even if it is not hosted on a Mozilla site, let us know and we will work with the developer to correct the issue. Please report them <a href="http://www.mozilla.org/projects/security/security-bugs-policy.html">confidentially </a>in <a href="https://bugzilla.mozilla.org/enter_bug.cgi?product=addons.mozilla.org&amp;component=Add-on%20Security&amp;maketemplate=Add-on%20Security%20Bug&amp;bit-23=1&amp;rep_platform=All&amp;op_sys=All">Bugzilla </a>or by emailing <a href="mailto:amo-admins@mozilla.org">amo-admins@mozilla.org</a>.</p>

<h4 id="Bugs_on_addons.mozilla.org_(AMO)">Bugs on addons.mozilla.org (AMO)</h4>

<p>If you find a problem with the site, we'd love to fix it. Please <a href="https://github.com/mozilla/addons/issues/new">file a bug report </a>and include as much detail as possible.</p>

