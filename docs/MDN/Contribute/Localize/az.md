---
version: prototype1
revision_id: 1127943
locale: az
slug: MDN/Contribute/Localize
tags: "l10n" "MDN Meta" "Landing" "TopicStub" "Localization" "NeedsTranslation"
title: Localizing MDN
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: 07731a7bde40a4ad8f5a95ca98e361c3f44680ce
---
<div>{{IncludeSubnav("/en-US/docs/MDN")}}</div>

<p>MDN is used by people all over the world as a reference and guide to Web technologies, as well as to the internals of Firefox itself. Our localization communities are a key part of the Mozilla project; their work in translating and localizing our documentation helps people around the world develop for the open Web. If you'd like to learn more about localization, or even start a new localization, this is the place to begin.</p>

<h2 id="Types_of_localization_on_MDN">Types of localization on MDN</h2>

<p>Localization on MDN comprises three aspects, which require different systems or access privileges.</p>

<dl>
 <dt>MDN site user interface</dt>
 <dd>The strings that appear on every MDN page (or most pages) to frame the main article content and provide navigation and user controls. These strings are translated using Mozilla’s <a href="/en-US/docs/Mozilla/Localization/Localizing_with_Pontoon">Pontoon</a> system. If your locale is not available for MDN, a Pontoon administrator must enable it.</dd>
 <dt>MDN content</dt>
 <dd>The main body of MDN pages, consisting of reference, guide, or tutorial articles. Articles can be translated using the <a href="/en-US/docs/MDN/Contribute/Localize/Translating_pages">built-in translation interface of MDN</a>. If your locale is not available in the list of locales to translate into, see <a href="/en-US/docs/MDN/Contribute/Localize/Starting_a_localization">Starting a new MDN localization</a>.</dd>
</dl>

<dl>
 <dt>Macro strings</dt>
 <dd>These strings are output by <a href="/en-US/docs/MDN/Contribute/Structures/Macros">macro templates</a> that construct certain kinds of navigation, messages, or generated structures. Because templates can have pervasive and potentially destructive effects, editing templates requires <a href="/en-US/docs/MDN/Contribute/Tools/Template_editing">a special access privilege</a>. If you do not have that access privilege, you will need to provide translated macro strings to someone who does have that privilege.</dd>
</dl>

<p>The following pages provide more details about localizing on MDN:</p>

<p>{{LandingPageListSubpages}}</p>

<h2 id="Localization_communities_on_MDN">Localization communities on MDN</h2>

<p>Localization activities on MDN are done both by individuals acting independently, and by groups working together, possibly as part of a larger Mozilla localization community. Localization projects on MDN are led by <strong>Localization drivers</strong>.</p>

<ul>
 <li><a href="/en-US/docs/MDN/Community/Roles/Localization_projects">Localization projects</a></li>
 <li><a href="/en-US/docs/MDN/Community/Roles/Localization_driver_role">Localization driver role</a></li>
</ul>

<h2 id="Localization_tools">Localization tools</h2>

<p>There are several useful tools that you'll use during localization work:</p>

<dl>
 <dt><a href="/en-US/docs/Mozilla/Localization/Localizing_with_Pontoon" title="/en-US/docs/Mozilla/Localization/Localizing_with_Verbatim">Pontoon</a></dt>
 <dd>Used for translation of strings across multiple Mozilla projects, including the MDN user interface (as well as the Firefox user interface).</dd>
 <dt><a href="http://transvision.mozfr.org/" title="http://transvision.mozfr.org/">Transvision</a></dt>
 <dd>A utility provided by Mozilla France, which lets you search for occurrences of an English string, finding all the various translations into a target locale that are used throughout Mozilla code. Useful for finding the preferred translations for words or phrases.</dd>
</dl>

<h2 id="See_also">See also</h2>

<ul>
 <li><a href="/en-US/docs/Mozilla/Localization" title="/en-US/docs/Mozilla/Localization">Localization at Mozilla</a></li>
</ul>

