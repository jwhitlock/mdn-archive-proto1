---
version: prototype1
revision_id: 1190309
locale: kab
slug: Mozilla/Add-ons
tags: 
title: Add-ons
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<p><span class="seoSummary">Izegrar ttaǧǧan ineflayen ad siɣzfen neɣ ad sniflen amek iteddu Firefox.</span> Ttawrun s useqdec n tizeɣt&nbsp; n tetiknulujiyin Web - JavaScript, HTML, and CSS - akked kra n igrudmawen usliɣen n yesnasen API n JavaScript. Gar wayen nniḍen, azegrir yezmer:</p>

<ul>
 <li>bedel tagammatt neɣ agbur n kra n ismal web.</li>
 <li>bedel agrudem uqedac n Firefox.</li>
 <li>Arrnu kra n tiseɣnatin ɣer Firefox.</li>
</ul>

<h2 id="Asnefli_izegrar-isemmaden">Asnefli izegrar-isemmaden</h2>

<p>llant akka tura aṭas n ttawilat iw snefli n (add-ons) izegrar-isemmaden Firefox,maca WebExtensions ad yuɣal d tagnut sya ɣer taggara 2017.tigrumma nniḍen n ifucka,ernud (add-ons)izegrar-isemmaden n afelselfu, add-ons bootstrap ed SDK add-on tettwarǧa ɣeluy n uzal n sen deg yiwet n tagwnitt.</p>

<p><a href="https://developer.mozilla.org/en-US/Add-ons/WebExtensions" style="margin-left: auto; margin-right: auto; margin-bottom: 20px; padding: 10px; text-align: center; border-radius: 4px; display: block; width: 30%;background-color: #81BC2E; color: white; text-shadow: 0px 1px 0px rgba(0, 0, 0, 0.25); box-shadow: 0px 1px 0px 0px rgba(0, 0, 0, 0.2), 0px -1px 0px 0px rgba(0, 0, 0, 0.3) inset;">Issin ugar ɣef&nbsp; WebExtensions &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </a></p>

<p>Ma yella turam azegrar amaynut asemmad,nesmagel-awen a ttarum i WebExtention.</p>

<p>WebExtensions are designed to be cross-browser compatible: WebExtensions written for Firefox will in most cases run in Chrome, Edge, and Opera with few if any changes. They are also fully compatible with multiprocess Firefox.<br />
 <br />
 Siked API ig etddun tura akka di Firefox akked iminigen nniḍen. We're continuing to design and implement new APIs in response to developer needs.<br />
 <br />
 Most of the WebExtensions APIs are also available on Firefox for Android.</p>

<h3 id="Migrate_an_Existing_Add-on">Migrate an Existing Add-on</h3>

<p>If you maintain a legacy add-on, such as a XUL overlay, bootstrapped, or Add-on SDK-based add-on, we recommend that you investigate porting it to WebExtensions. There are some <a href="/en-US/Add-ons/WebExtensions/Porting_a_legacy_Firefox_add-on">porting resources on MDN</a>.</p>

<p>We've collected <a href="https://wiki.mozilla.org/Add-ons/developer/communication">resources</a> on a wiki page to support developers through the transition. To get started, use the compatibility <a href="https://compatibility-lookup.services.mozilla.com/">Lookup Tool</a> to see if your add-on will be affected.</p>

<h2 id="Publishing_add-ons">Publishing add-ons</h2>

<p><a href="https://addons.mozilla.org">Addons.mozilla.org</a>, commonly known as "AMO," is Mozilla's official site for developers to list add-ons, and for users to discover them. By uploading your add-on to AMO, you can participate in our community of users and creators, and find an audience for your add-on.</p>

<p>You are not required to list your add-on on AMO, but your add-on must be signed by Mozilla or users won't be able to install it.</p>

<p>For an overview of the process of publishing your add-on, see <a href="https://developer.mozilla.org/en-US/Add-ons/Distribution">Signing and distributing your add-on</a>.</p>

<h2 id="Other_types_of_add-ons">Other types of add-ons</h2>

<p>Generally, when people speak of add-ons they're referring to extensions, but there are a few other add-on types that allow users to customize Firefox. Those add-ons include:</p>

<ul>
 <li><a href="https://developer.mozilla.org/Add-ons/Themes/Background">Lightweight themes</a> are a simple way to provide limited customization for Firefox.</li>
 <li><a href="/en-US/Add-ons/Firefox_for_Android">Mobile add-ons</a> are add-ons for&nbsp;Firefox for Android. Note, though, that we intend to deprecate some of the technology underlying these APIs. In the future, WebExtensions will be fully supported on Firefox for Android.</li>
 <li><a href="/en-US/docs/Creating_OpenSearch_plugins_for_Firefox">Search engine plugins</a> add new search engines to the browser's search bar.</li>
 <li><a href="/en-US/docs/Mozilla/Creating_a_spell_check_dictionary_add-on">User dictionaries</a> are add-ons that let you spell-check in different languages.</li>
 <li><a href="https://support.mozilla.org/kb/use-firefox-interface-other-languages-language-pack">Language packs</a> are add-ons that let you have more languages available for the user interface of Firefox.</li>
</ul>

<hr />
<h2 id="Contact_us">Contact us</h2>

<p>You can use the links below to get help, keep up to date with news around add-ons, and give us feedback.</p>

<h3 id="Add-ons_forum">Add-ons forum</h3>

<p>Use the <a href="https://discourse.mozilla-community.org/c/add-ons">Add-ons Discourse forum</a> to discuss all aspects of add-on development and to get help.</p>

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
 <li><a href="irc://irc.mozilla.org/webextensions">#webextensions</a> (discussion of WebExtensions in particular)</li>
</ul>

