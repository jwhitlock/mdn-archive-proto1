---
version: prototype1
revision_id: 1264273
locale: en-US
slug: Web/API/Web_Animations_API/Using_the_Web_Animations_API
tags: "CSS" "Alice" "Guide" "play" "Timing" "pause" "Beginner" "Tutorial" "animate" "reverse" "JavaScript" "duration" "Animations" "keyframes" "web animations api"
title: Using the Web Animations API
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: True
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>{{DefaultAPISidebar("Web Animations")}}</p>

<p class="summary">The Web Animations API lets us construct animations and control their playback with JavaScript. This article will start you off in the right direction with fun demos and tutorials featuring Alice in Wonderland.</p>

<h2 id="Meet_the_Web_Animations_API">Meet the Web Animations API</h2>

<p>The <a href="/en-US/docs/Web/API/Web_Animations_API">Web Animations API</a> opens the browser’s animation engine to developers&nbsp;and manipulation by JavaScript. This API was designed to underlie implementations of both <a href="/en-US/docs/Web/CSS/CSS_Animations">CSS Animations</a> and <a href="/en-US/docs/Web/CSS/CSS_Transitions">CSS Transitions</a>, and leaves the door open to future animation effects. It is one of the most performant ways to animate on the Web where supported, letting the browser make its own internal optimizations without hacks, coercion, or {{domxref("Window.requestAnimationFrame()")}}.</p>

<p>With the Web Animations API, we&nbsp;can move interactive animations from stylesheets to JavaScript, separating presentation from behavior. We no longer need to rely on DOM-heavy techniques like writing CSS properties and scoping&nbsp;classes onto elements to control playback direction. And unlike pure, declarative CSS,&nbsp;JavaScript also lets us dynamically set values from properties to durations. For building custom animation libraries and creating interactive animations, the Web Animations API might be the perfect tool for the job. Let's see what it can do!</p>

<h2 id="Browser_Support">Browser Support</h2>

<p>The basic Web Animations API features discussed in this article are available by default in Firefox 48+ and Chrome 36+. Webkit and Edge have moved the API onto their respective to-do lists, but until we see full support across all&nbsp;browsers, there’s a <a href="https://github.com/web-animations/web-animations-js">handy maintained polyfill</a>&nbsp;that tests for feature support and adds it where necessary.</p>

<h2 id="Writing_CSS_Animations_with_the_Web_Animations_API">Writing CSS Animations with the Web Animations API</h2>

<p>One of the more familiar ways to approach learning the Web Animations API is to start with something most web developers have played with before: CSS Animations. CSS Animations have a familiar syntax that breaks down nicely for demonstration purposes.</p>

<h3 id="The_CSS_version">The CSS version</h3>

<p>Here’s a tumbling animation written in CSS showing Alice falling down the rabbit hole that leads to Wonderland (see the full&nbsp;<a href="http://codepen.io/rachelnabors/pen/QyOqqW">code on Codepen</a>):</p>

<p><a href="http://codepen.io/rachelnabors/pen/rxpmJL" target="_blank"><img alt="Alice Tumbling down the rabbit's hole." src="https://mdn.mozillademos.org/files/13843/tumbling-alice_optimized.gif" style="display:block; height:374px; margin-left:auto; margin-right:auto; width:700px" /></a></p>

<p>Notice that the background moves, Alice spins, and her color changes at an offset from her spinning. We’re going to focus on just Alice for this tutorial. Here’s the simplified CSS that controls Alice’s animation:</p>

<pre class="brush: css">
#alice {
  animation: aliceTumbling infinite 3s linear;
}

@keyframes aliceTumbling {
  0% {
    color: #000;
    transform: rotate(0) translate3D(-50%, -50%, 0);    
  }
  30% {
    color: #431236;
  }
  100% {
    color: #000;
    transform: rotate(360deg) translate3D(-50%, -50%, 0);
  }
}</pre>

<p>This changes Alice’s color and her transform’s rotation over 3 seconds at a constant (linear) rate and loops infinitely. In the <a href="/en-US/docs/Web/CSS/@keyframes">@keyframes</a> block we can see that 30% of the way through each loop (about .9 seconds in), Alice’s color changes from black to a deep burgundy then back again by the end of the loop.</p>

<h3 id="Moving_it_to_JavaScript">Moving it to JavaScript</h3>

<p>Now let’s try creating the same animation with the Web Animations API.</p>

<h4 id="Representing_keyframes">Representing keyframes</h4>

<p>The first thing we need is to create a <a href="/en-US/docs/Web/API/Web_Animations_API/Keyframe_Formats">Keyframe Object</a> corresponding to our CSS <a href="/en-US/docs/Web/CSS/@keyframes">@keyframes</a> block:</p>

<pre class="brush: js">
var aliceTumbling = [
  { transform: 'rotate(0) translate3D(-50%, -50%, 0)', color: '#000' },
  { color: '#431236', offset: 0.3},
  { transform: 'rotate(360deg) translate3D(-50%, -50%, 0)', color: '#000' }
];</pre>

<p>Here we’re using an array containing multiple objects. Each object represents a key from the original CSS. However, unlike CSS, the Web Animations API doesn’t need to explicitly be told the percentages along the animation for each key to appear at. It will automatically divide the animation into equal parts based on the number of keys you give it. This means that a Keyframe object with three keys will play the middle key 50% of the way through each loop of the animation unless told otherwise.</p>

<p>When we want to explicitly set a key’s offset from the other keys, we can specify an offset directly in the object, separated from the declaration with a comma. In the above example, to make sure that Alice’s color changes at 30% not 50% for the color change, we are giving it <code>offset: 0.3</code>.</p>

<p>There must be at least two keyframes specified (representing the starting and ending states of the animation sequence). If your keyframe list only has one entry, {{domxref("Element.animate()")}} will throw a <code>NotSupportedError</code> exception.</p>

<p>So to recap, the keys are equally spaced by default unless you specify an offset on a key. Handy, no?</p>

<h4 id="Representing_timing_properties">Representing timing properties</h4>

<p>We’ll also need to create an object of timing properties (an {{domxref("AnimationEffectTimingProperties")}} object) corresponding to the values in Alice’s animation:</p>

<pre class="brush: js">
var aliceTiming = {
  duration: 3000,
  iterations: Infinity
}</pre>

<p>You’ll notice a few differences here from how equivalent values are represented in CSS:</p>

<ul>
 <li>For one, the duration is in milliseconds as opposed to seconds — 3000 not 3s. Like {{domxref("WindowTimers.setTimeout()")}} and {{domxref("Window.requestAnimationFrame()")}}, the Web Animations API only takes milliseconds.</li>
 <li>The other thing you’ll notice is that it’s <code>iterations</code>, not <code>iteration-count</code>.</li>
</ul>

<div class="note">
<p>There are a number of small differences between the terminology used in CSS animations and the terminology used in Web Animations. For instance, Web Animations doesn't use the string <code>"infinite"</code>, but instead uses the JavaScript keyword <code>Infinity</code>. And instead of <code>timing-function</code> we use <code>easing</code>. We aren’t listing an <code>easing</code> value here because, unlike CSS Animations where the default <a href="/en-US/docs/Web/CSS/animation-timing-function">animation-timing-function</a> is <code>ease</code>, in the Web Animations API the default easing is <code>linear</code> — which is what we want here.</p>
</div>

<h4 id="Bring_the_pieces_together">Bring the pieces together</h4>

<p>Now it’s time to bring them both together with the {{domxref("Element.animate()")}} method:</p>

<pre class="brush: js">
document.getElementById("alice").animate(
  aliceTumbling,
  aliceTiming
)</pre>

<p>And boom: the animation starts playing (see the finished <a href="http://codepen.io/rachelnabors/pen/rxpmJL">version on Codepen</a>).</p>

<p>The <code>animate()</code> method can be called on any DOM element that could be animated with CSS. And it can be written in several ways. Instead of making objects for keyframes and timing properties, we could just pass their values in directly like so:</p>

<pre class="brush: js">
document.getElementById("alice").animate(
  [
    { transform: 'rotate(0) translate3D(-50%, -50%, 0)', color: '#000' },
    { color: '#431236', offset: 0.3},
    { transform: 'rotate(360deg) translate3D(-50%, -50%, 0)', color: '#000' }
  ], {
    duration: 3000,
    iterations: Infinity
  }
);</pre>

<p>What’s more, if we only wanted to specify the duration of the animation and not its iterations (by default animations iterate once), we could pass in the milliseconds alone:</p>

<pre class="brush: js">
document.getElementById("alice").animate(
  [
    { transform: 'rotate(0) translate3D(-50%, -50%, 0)', color: '#000' },
    { color: '#431236', offset: 0.3},
    { transform: 'rotate(360deg) translate3D(-50%, -50%, 0)', color: '#000' }
  ], 3000);</pre>

<h2 id="Controlling_playback_with_play()_pause()_reverse()_and_playbackRate">Controlling playback with play(), pause(), reverse() and playbackRate</h2>

<p>While we can write CSS Animations with the Web Animations API, where the API really comes in handy is manipulating the animation’s playback. The Web Animations API provides several useful methods for controlling playback. Let’s take a look at pausing and playing animations in the Growing/Shrinking Alice game (check out the <a href="http://codepen.io/rachelnabors/pen/PNYGZQ">full code on Codepen</a>):</p>

<p><a href="http://codepen.io/rachelnabors/pen/PNYGZQ?editors=0010" target="_blank"><img alt="Playing the growing and shrinking game with Alice." src="https://mdn.mozillademos.org/files/13845/growing-shrinking_article_optimized.gif" style="display:block; height:374px; margin-left:auto; margin-right:auto; width:700px" /></a></p>

<p>In this game, Alice has an animation that causes her to go from small to big which we control via a bottle and a cupcake. Both of these have their own animations.</p>

<h3 id="Pausing_and_playing_animations">Pausing and playing animations</h3>

<p>We’ll talk more about Alice’s animation later, but for now, let’s look closer at the cupcake’s animation:</p>

<pre class="brush: js">
var nommingCake = document.getElementById('eat-me_sprite').animate(
[
  { transform: 'translateY(0)' },
  { transform: 'translateY(-80%)' }   
], {
  fill: 'forwards',
  easing: 'steps(4, end)',
  duration: aliceChange.effect.timing.duration / 2
});</pre>

<p>The {{domxref("Element.animate()")}} method will immediately run after it is called. To prevent the cake from eating itself up before the user has had the chance to click on it, we call {{domxref("Animation.pause()")}} on it immediately after it is defined, like so:</p>

<pre class="brush: js">
nommingCake.pause();</pre>

<p>We can now use the {{domxref("Animation.play()")}} method to run it whenever we’re ready:</p>

<pre class="brush: js">
nommingCake.play();</pre>

<p>Specifically, we want to link it to Alice’s animation, so she gets bigger as the cupcake gets eaten. We can achiveve this via the following function:</p>

<pre class="brush: js">
var growAlice = function() {

  // Play Alice's animation.
  aliceChange.play();

  // Play the cake's animation.
  nommingCake.play();

}</pre>

<p>When a user holds their mouse down or presses their finger on the cake on a touch screen, we can now call <code>growAlice</code> to make all the animations play:</p>

<pre class="brush: js">
cake.addEventListener("mousedown", growAlice, false);
cake.addEventListener("touchstart", growAlice, false);</pre>

<h3 id="Other_useful_methods">Other useful methods</h3>

<p>In addition to pausing and playing, we can use the following Animation methods:</p>

<ul>
 <li>{{domxref("Animation.finish()")}} skips to the end of the animation.</li>
 <li>{{domxref("Animation.cancel()")}} aborts the animation and removes its effects.</li>
 <li>{{domxref("Animation.reverse()")}} sets the animation’s playback rate ({{domxref("Animation.playbackRate")}} to a negative value so it runs backwards.</li>
</ul>

<p>Let’s take a look at <code>playbackRate</code> first — a negative playbackRate will cause an animation to run in reverse. When Alice drinks from the bottle, she grows smaller. This is because the bottle changes her animation’s playbackRate from 1 to -1:</p>

<pre class="brush: js">
var shrinkAlice = function() {
  aliceChange.playbackRate = -1;
  aliceChange.play();
}

bottle.addEventListener("mousedown", shrinkAlice, false);
bottle.addEventListener("touchstart", shrinkAlice, false);</pre>

<p>In <a href="https://en.wikipedia.org/wiki/Through_the_Looking-Glass">Through the Looking-Glass</a>, Alice travels to a world where she must run to stay in place — and run twice as fast to move forward! In the Red Queen’s Race example, Alice and the Red Queen are running to stay in place (check out the <a href="http://codepen.io/rachelnabors/pen/PNGGaV">full code on Codepen</a>):</p>

<p><a href="http://codepen.io/rachelnabors/pen/PNGGaV" target="_blank"><img alt="Alice and the Red Queen race to get to the next square in this game." src="https://mdn.mozillademos.org/files/13847/red-queen-race_optimized.gif" style="display:block; height:342px; margin-left:auto; margin-right:auto; width:640px" /></a></p>

<p>Because small children tire out easily, unlike automaton chess pieces, Alice is constantly slowing down. We've done this in the code by setting a decay on her animation’s <code>playbackRate</code>:</p>

<pre class="brush: js">
setInterval( function() {

  // Make sure the playback rate never falls below .4
  if (redQueen_alice.playbackRate &gt; .4) {
    redQueen_alice.playbackRate *= .9;    
  }

}, 3000);</pre>

<p>But urging them on by clicking or tapping causes them to speed up by multiplying their playbackRate:</p>

<pre class="brush: js">
var goFaster = function() {

  redQueen_alice.playbackRate *= 1.1;

}

document.addEventListener("click", goFaster);
document.addEventListener("touchstart", goFaster);</pre>

<p>The background elements also have <code>playbackRate</code>s that are impacted when you click or tap. What happens when you make Alice and the Red Queen run twice as fast? What happens when you let them slow down?</p>

<h2 id="Getting_information_out_of_animations">Getting information out of animations</h2>

<p>Imagine other ways we could use playbackRate, like improving accessibility for users with vestibular disorders by letting them slow down animations across an&nbsp;entire site. That’s impossible to do with CSS without recalculating durations in every CSS rule, but with the Web Animations API, we could use the upcoming (not supported in browsers yet!) {{domxref("document.getAnimations()")}} method to loop over each animation on the page and halve their <code>playbackRate</code>s like so:</p>

<pre class="brush: js">
document.getAnimations().forEach(
  function (animation) {
    animation.playbackRate *= .5;
  }
);</pre>

<p>With the Web Animations API, all you need to change is just one little property!</p>

<p>Another thing that’s tough to do with CSS Animations alone is creating dependencies on values provided by other animations. For instance, in the Growing and Shrinking Alice game example, you might have noticed something odd about the cake’s duration:</p>

<pre class="brush: js">
duration: aliceChange.effect.timing.duration / 2</pre>

<p>To understand what’s happening here, let’s take a look at Alice’s animation:</p>

<pre class="brush: js">
var aliceChange = document.getElementById('alice').animate(
  [
    { transform: 'translate(-50%, -50%) scale(.5)' },
    { transform: 'translate(-50%, -50%) scale(2)' }   
  ], {
    duration: 8000,
    easing: 'ease-in-out',
    fill: 'both'
  });</pre>

<p>Alice’s animation has her going from half her size to twice her size over 8 seconds. Then we pause her:</p>

<pre class="brush: js">
aliceChange.pause();</pre>

<p>If we had left her paused at the beginning of her animation, she’d start at half her full size, like she’d drunk the entire bottle already! We want to set her animation’s “playhead” in the middle, so she’s already halfway done. We could do that by setting her {{domxref("Animation.currentTime")}} to 4 seconds like so:</p>

<pre class="brush: js">
aliceChange.currentTime = 4000;</pre>

<p>But while working on this animation, we might change Alice’s duration a lot. Wouldn’t it be better if we set her <code>currentTime</code> dynamically, so we don’t have to make two updates at a time? We can in fact do so by referencing aliceChange’s {{domxref("Animation.effect")}} property, which returns an object containing all the details of the effect(s) active on Alice:</p>

<pre class="brush: js">
aliceChange.currentTime = aliceChange.effect.timing.duration / 2;</pre>

<p><code>effect</code> lets us access the animation’s <code>keyframe</code> and <code>timing</code> objects — <code>aliceChange.effect.timing</code> points to Alice’s timing object (which is of type {{domxref("AnimationEffectTimingReadOnly")}}) — this contains her {{domxref("AnimationEffectTimingReadOnly.duration")}}. We can divide her duration in half to get the midpoint for her animation’s timeline, setting her to be normal height. Now we can reverse and play her animation in either direction to make her grow smaller or larger!</p>

<p>And we can do the same thing when setting the cake and bottle durations:</p>

<pre class="brush: js">
var drinking = document.getElementById('liquid').animate(
[
  { height: '100%' },
  { height: '0' }   
], {
  fill: 'forwards',
  duration: aliceChange.effect.timing.duration / 2
});
drinking.pause();</pre>

<p>Now all three animations are linked to just one duration, which we can change easily from one place.</p>

<p>We can also use the Web Animations API to figure out the animation's current time. The game ends when you run out of cake to eat or empty the bottle. Which vignette players are presented with depends on how far along Alice was in her animation, whether she grew too big and can't get in the tiny door anymore&nbsp;or too small and cannot reach the key to open the door. We can figure out whether she's on the large end or small end of her animation by getting her animation's <code><a href="/en-US/docs/Web/API/Animation/currentTime">currentTime</a></code>&nbsp;and dividing it by her <code>activeDuration</code>:</p>

<pre class="brush: js">
var endGame = function() {
  
  // get Alice's timeline's playhead location
  var alicePlayhead = aliceChange.currentTime;
  var aliceTimeline = aliceChange.effect.activeDuration;

  // stops Alice's and other animations
  stopPlayingAlice();

  // depending on which third it falls into
  var aliceHeight = alicePlayhead/aliceTimeline;

  if (aliceHeight &lt;= .333){
    // Alice got smaller!
    ...

  } else if (aliceHeight &gt;= .666) {
    // Alice got bigger!
    ...

  } else {
    // Alice didn't change significantly    
    ...

  }
}
</pre>

<div class="note">
<p><strong>Note:</strong>&nbsp;<code>getAnimations()</code> and <code>effect</code> are not fully supported as of this writing, but the polyfill does support them today.</p>
</div>

<h2 id="Callbacks_and_promises">Callbacks and promises</h2>

<p>CSS Animations and Transitions have their own event listeners, and these are also possible with the Web Animations API:</p>

<ul>
 <li><code><a href="/en-US/docs/Web/API/Animation/onfinish">onfinish</a></code> is the event handler for the <code>finish</code> event and can be triggered manually with&nbsp;<code><a href="/en-US/docs/Web/API/Animation/finish">finish()</a></code>.</li>
 <li><code><a href="/en-US/docs/Web/API/Animation/oncancel">oncancel</a></code> is the event handler for the <code>cancel</code> event and can be triggers with <code><a href="/en-US/docs/Web/API/Animation/cancel">cancel()</a></code>.</li>
</ul>

<p>Here we set the callbacks for&nbsp;the cake, bottle, and Alice to fire the <code>endGame</code> function:</p>

<pre class="brush: js">
// When the cake or runs out...&nbsp;
nommingCake.onfinish = endGame;
drinking.onfinish = endGame;

// ...or Alice reaches the end of her animation
aliceChange.onfinish = endGame;

</pre>

<p>Prefer promises? The Web Animations&nbsp;API also specifies two promises:&nbsp;<code><a href="/en-US/docs/Web/API/Animation/onfinish">onfinish</a></code> and <code><a href="/en-US/docs/Web/API/Animation/oncancel">oncancel</a></code>.</p>

<div class="note">
<p>These promises are not fully supported as of this writing.</p>
</div>

<h2 id="Conclusion">Conclusion</h2>

<p>These are the basic features of the Web Animations API, most of which are already supported across the latest release versions of Firefox and Chrome. By now you should be ready to "jump down the rabbit hole" of animating in the browser&nbsp;and ready to write your own animation experiments! If you're using the&nbsp;API and want to share, try&nbsp;using the&nbsp;#WAAPI hashtag. We will be watching and will write more tutorials to cover further features as support spreads!&nbsp;</p>

<h2 id="See_also">See also</h2>

<ul>
 <li class="post__title">The <a href="http://codepen.io/collection/bpEza/">full suite of Alice in Wonderland demos</a>&nbsp;on CodePen for you to play with, fork, and share</li>
 <li class="post__title"><a href="https://hacks.mozilla.org/2016/08/animating-like-you-just-dont-care-with-element-animate/">Animating like you just don’t care with Element.animate</a> — a great article to read that explains more on the background of the Web Animations API, and why it is more performant than other web animation methods</li>
 <li class="post__title"><a href="https://github.com/web-animations/web-animations-js">web-animations-js</a> — the&nbsp;Web Animations API polyfill</li>
</ul>
