---
version: prototype1
revision_id: 1331699
locale: en-US
slug: Web/API/Web_Animations_API
tags: "API" "Landing" "Animation" "Reference" "Experimental" "Web Animations"
title: Web Animations API
summary: 
keywords: 
needs_technical_review: True
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>{{DefaultAPISidebar("Web Animations")}}{{ SeeCompatTable() }}</p>

<div class="summary">
<p>The Web Animations API allows for synchronizing and timing changes to the presentation of a Web page, i.e. animation of DOM elements. It does so by combining two models: the Timing Model and the Animation Model.</p>
</div>

<h2 id="Concepts_and_usage">Concepts and usage</h2>

<p>The Web Animations API provides a common language for browsers and developers to describe animations on DOM elements. To get more information on the concepts behind the API and how to use it, read <a href="/en-US/docs/Web/API/Web_Animations_API/Using_the_Web_Animations_API">Using the Web Animations API</a>.</p>

<h2 id="Web_Animations_interfaces">Web Animations interfaces</h2>

<dl>
</dl>

<dl>
 <dt>{{domxref("Animation")}}</dt>
 <dd>Provides playback controls and a timeline for an animation node or source. Can take an object created with the&nbsp;{{domxref("KeyframeEffect.KeyframeEffect", "KeyframeEffect()")}} constructor.</dd>
 <dt>{{domxref("KeyframeEffect")}}</dt>
 <dd>Describes sets of animatable properties and values, called&nbsp;<strong>keyframes </strong>and their <a href="/en-US/docs/Web/API/Web_Animations_API/Animation_timing_options">timing options</a><strong>.&nbsp;</strong>These can then be played using the {{domxref("Animation.Animation", "Animation()")}} constructor.</dd>
 <dt>{{domxref("AnimationTimeline")}}</dt>
 <dd>Represents the timeline of animation. This interface exists to define timeline features (inherited by {{domxref("DocumentTimeline")}} and future timeline objects) and is not itself accessed by developers.</dd>
 <dt>{{domxref("AnimationEvent")}}</dt>
 <dd>Actually part of CSS Animations.</dd>
 <dt>{{domxref("DocumentTimeline")}}</dt>
 <dd>Represents animation timelines, including the default document timeline (accessed using the {{domxref("Document.timeline")}} property).</dd>
 <dt>{{domxref("AnimationEffectTiming")}}</dt>
 <dd>An object containing&nbsp;timing properties returned by the {{domxref("KeyframeEffect.timing", "timing")}}&nbsp;attribute of a {{domxref("KeyframeEffect")}}. It inherits its properties from {{domxref("AnimationEffectTimingReadOnly")}}, but in a non-read only form.</dd>
 <dt>{{domxref("AnimationEffectTimingProperties")}}</dt>
 <dd>{{domxref("Element.animate()")}}, {{domxref("KeyframeEffectReadOnly.KeyframeEffectReadOnly()")}}, and {{domxref("KeyframeEffect.KeyframeEffect()")}} all accept an optional dictionary&nbsp;object of timing properties.</dd>
</dl>

<h2 id="Extensions_to_other_interfaces">Extensions to other interfaces</h2>

<p>The Web Animations API adds some new features to <strong style="font-size:14px; font-weight:700; line-height:1.5">{{domxref("document")}}</strong> and&nbsp;<strong style="font-size:14px; font-weight:700; line-height:1.5">{{domxref("element")}}.</strong></p>

<h3 id="Extensions_to_the_Document_interface">Extensions to the <code>Document</code> interface</h3>

<dl>
 <dt>{{domxref("document.timeline")}}</dt>
 <dd>The <code>DocumentTimeline</code> object representing the default document timeline.</dd>
 <dt>{{domxref("document.getAnimations()")}}</dt>
 <dd>Returns an Array of {{domxref("Animation")}}&nbsp;objects currently in effect on elements in the <code>document</code>.</dd>
 <dt>
 <h3 id="Extensions_to_the_Element_interface">Extensions to the <code>Element</code> interface</h3>
 </dt>
 <dt>{{domxref("Element.animate()")}}</dt>
 <dd>A shortcut method for creating and playing an animation on an element. It returns the created {{domxref("Animation")}} object instance.</dd>
</dl>

<dl>
</dl>

<h2 id="Web_Animations_read-only_interfaces">Web Animations read-only interfaces</h2>

<p>The following interfaces are included in the spec for purposes such as defining features used in multiple other places, or to serve as bases for multiple interfaces which can all be used as values of the same properties. You wouldn't directly use these in web development work, but they may be interesting for library authors to understand how the technology works so their implementations can be more effective, or for browser engineers looking for an easier reference than the spec provides.</p>

<dl>
 <dt>{{domxref("AnimationEffectTimingReadOnly")}}</dt>
 <dd>A dictionary object of&nbsp;timing properties, which are inherited by the mutable {{domxref("AnimationEffectTiming")}} interface associated with&nbsp;{{domxref("KeyframeEffect")}}.</dd>
 <dt>{{domxref("AnimationEffectReadOnly")}}</dt>
 <dd>Defines current and future "Animation Effects" like {{domxref("KeyframeEffect")}}, which can be passed to {{domxref("Animation")}} objects for playing, and {{domxref("KeyframeEffectReadOnly")}} which is used by {{domxref("KeyframeEffect")}}&nbsp;(inherited by <a href="/en-US/docs/Web/CSS/CSS_Animations">CSS Animations</a> and <a href="/en-US/docs/Web/CSS/CSS_Transitions">Transitions</a>). All values of {{domxref("Animation.effect")}} are of types based on <code>AnimationEffectReadOnly</code>.</dd>
 <dt>{{domxref("KeyframeEffectReadOnly")}}</dt>
 <dd>Describes sets of animatable properties and values that can be played using&nbsp;the&nbsp;{{domxref("Animation.Animation", "Animation()")}} constructor, and which are inherited by {{domxref("KeyframeEffect")}}.&nbsp;</dd>
</dl>

<h2 id="Specifications">Specifications</h2>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="col">Specification</th>
   <th scope="col">Status</th>
   <th scope="col">Comment</th>
  </tr>
  <tr>
   <td>{{SpecName('Web Animations')}}</td>
   <td>{{Spec2('Web Animations')}}</td>
   <td>Initial definition</td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<p>{{ CompatibilityTable() }}</p>

<div id="compat-desktop">
<table class="compat-table">
 <tbody>
  <tr>
   <th>Chrome</th>
   <th>Firefox (Gecko)</th>
   <th>Internet Explorer</th>
   <th>Opera</th>
   <th>Safari (WebKit)</th>
  </tr>
  <tr>
   <td>{{ CompatChrome(36.0) }}<sup>[1]</sup><br />
    &nbsp;</td>
   <td>{{ CompatGeckoDesktop(48)}}<sup>[1]</sup></td>
   <td>{{ CompatNo }}</td>
   <td>
    <p>29<br />
     28 behind pref</p>
   </td>
   <td>{{ CompatNo }}</td>
  </tr>
  <tr>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{ CompatNo }}<sup>[1]</sup></td>
   <td>{{ CompatNo }}</td>
   <td>{{ CompatNo }}</td>
   <td>{{ CompatNo }}</td>
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
   <th>Android Webview</th>
   <th>Firefox Mobile (Gecko)</th>
   <th>IE Phone</th>
   <th>Opera Mobile</th>
   <th>Safari Mobile</th>
   <th>Chrome for Android</th>
  </tr>
  <tr>
   <td>Basic support</td>
   <td>{{ CompatNo }}</td>
   <td>{{CompatChrome(42.0)}}</td>
   <td>{{ CompatGeckoMobile(48) }}</td>
   <td>{{ CompatNo }}</td>
   <td>{{ CompatNo }}</td>
   <td>{{ CompatNo }}</td>
   <td>{{ CompatChrome(42.0) }}</td>
  </tr>
 </tbody>
</table>
</div>

<p>[1] Only a subset of the API is enabled. See the individual API members for shipping status.</p>

<h2 id="See_also">See also</h2>

<ul>
 <li><a href="/en-US/docs/Web/API/Web_Animations_API/Using_the_Web_Animations_API">Using the Web Animations API</a></li>
 <li><a href="https://mozdevs.github.io/Animation-examples/">Web Animations demos</a></li>
 <li><a href="https://github.com/web-animations/web-animations-js">Polyfill</a></li>
 <li>Firefox's current implementation:&nbsp;<a href="https://birtles.github.io/areweanimatedyet/">AreWeAnimatedYet</a></li>
 <li>
  <p><a href="http://codepen.io/danwilson/pen/xGBKVq">Browser support test</a></p>
 </li>
</ul>

