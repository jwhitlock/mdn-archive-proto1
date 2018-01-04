---
version: prototype1
revision_id: 1342330
locale: en-US
slug: Learn/Getting_started_with_the_web/JavaScript_basics
tags: "Web" "Learn" "Beginner" "JavaScript" "l10n:priority" "CodingScripting"
title: JavaScript basics
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{LearnSidebar}}</div>

<div>{{PreviousMenuNext("Learn/Getting_started_with_the_web/CSS_basics", "Learn/Getting_started_with_the_web/Publishing_your_website", "Learn/Getting_started_with_the_web")}}</div>

<div class="summary">
<p>JavaScript is a&nbsp;programming language that adds interactivity to your website (for example: games, responses when buttons are pressed or data entered in forms, dynamic styling, animation). This article helps you get started with this exciting language and gives you an idea of what is possible.</p>
</div>

<h2 id="What_is_JavaScript_really">What is JavaScript, really?</h2>

<p>{{Glossary("JavaScript")}} ("JS" for short) is a full-fledged {{Glossary("Dynamic programming language", "dynamic programming language")}} that, when&nbsp;applied to an {{Glossary("HTML")}} document, can provide&nbsp;dynamic interactivity on websites. It was invented by Brendan Eich, co-founder of the Mozilla project, the Mozilla Foundation, and the Mozilla Corporation.</p>

<p>JavaScript is incredibly versatile. You can start small, with carousels, image galleries, fluctuating layouts, and responses to button clicks. With more experience, you'll be able to create games, animated 2D and 3D graphics, comprehensive database-driven apps, and much more!</p>

<p>JavaScript itself is fairly compact yet very flexible. Developers have written a large variety of tools on top of the core JavaScript language, unlocking a vast amount of extra functionality with minimum effort. These include:</p>

<ul>
 <li>Browser Application Programming Interfaces ({{Glossary("API","APIs")}}) — APIs built into web browsers, providing functionality&nbsp;like&nbsp;dynamically creating&nbsp;HTML and setting CSS styles, collecting and manipulating&nbsp;a video stream from the user's webcam, or generating&nbsp;3D graphics and audio samples.</li>
 <li>Third-party APIs to allow developers to incorporate functionality in their sites from other content providers, such as Twitter or Facebook.</li>
 <li>Third-party frameworks and libraries you can apply to your HTML to allow you to rapidly build up sites and applications.</li>
</ul>

<p>Because this article is only supposed to be a light introduction to JavaScript, we are not going to confuse you at this stage by talking in detail about what the difference is between the core JavaScript language and the different tools listed above. You can learn all that in detail later on, in our <a href="/en-US/docs/Learn/JavaScript">JavaScript learning area</a>, and in the rest of MDN.</p>

<p>Below we will introduce you to some aspects of the core language, and you'll also play with a few browser API features too. Have fun!</p>

<h2 id="A_hello_world_example">A "hello world" example</h2>

<p>The above section might sound really exciting, and so it should — JavaScript is one of the most lively web technologies, and as you start to get good at using it, your websites will enter a new dimension of power and creativity.</p>

<p>However, becoming comfortable with JavaScript is a little harder than becoming comfortable with HTML and CSS. You may have to start small and keep working in small consistent steps. To start, we'll show how to add some basic JavaScript to your page, creating a <em>"hello world!"</em> example (<a href="https://en.wikipedia.org/wiki/%22Hello,_World!%22_program">the standard in basic programming examples</a>).</p>

<div class="warning">
<p><strong>Important</strong>: If you haven't been following along with the rest of our course, <a href="https://github.com/mdn/beginner-html-site-styled/archive/gh-pages.zip">download this example code</a> and use it as a starting point.</p>
</div>

<ol>
 <li>First, go to your test site and create a new folder named 'scripts' (without the quotes). Then, within the new scripts folder you just created, create a new file called <code>main.js</code>. Save it in your <code>scripts</code> folder.</li>
 <li>Next, in your <code>index.html</code> file enter the following element on a new line just before the closing <code>&lt;/body&gt;</code> tag:
  <pre class="brush: html">
&lt;script src="scripts/main.js"&gt;&lt;/script&gt;</pre>
 </li>
 <li>This is basically doing the same job as the {{htmlelement("link")}} element for CSS — it applies the JavaScript to the page, so it can have an effect on the HTML (along with the CSS, and anything else on the page).</li>
 <li>Now add the following code to the <code>main.js</code> file:
  <pre class="brush: js">
var myHeading = document.querySelector('h1');
myHeading.textContent = 'Hello world!';</pre>
 </li>
 <li>Finally,&nbsp;make sure the HTML and JavaScript files are saved, then load <code>index.html</code> in the browser. You should see something like the following:<img alt="" src="https://mdn.mozillademos.org/files/9543/hello-world.png" style="display:block; height:236px; margin:0px auto; width:806px" /></li>
</ol>

<div class="note">
<p><strong>Note</strong>: The reason we've put the {{htmlelement("script")}} element near the bottom of the HTML file is that HTML is loaded by the browser in the order it appears in the file. If the JavaScript is loaded first and it is supposed to affect the HTML below it, it might not work, as the JavaScript would be loaded before the HTML it is supposed to work on. Therefore, putting JavaScript near the bottom of the HTML page is often the best strategy.</p>
</div>

<h3 id="What_happened">What happened?</h3>

<p>Your heading text has now been changed to "Hello world!" using JavaScript. You did this by first using a function called <code>{{domxref("Document.querySelector", "querySelector()")}}</code> to grab a reference to your heading, and store it in a variable called <code>myHeading</code>. This is very similar to what we did using CSS selectors. When wanting to do something to an element, you first need to&nbsp;select it.</p>

<p>After that, you set the value of the <code>myHeading</code> variable's <code>{{domxref("Node.textContent", "textContent")}}</code> property (which represents the content of the heading) to "Hello world!".</p>

<div class="note">
<p><strong>Note</strong>: Both of the features you used above are parts of the <a href="/en-US/docs/Web/API/Document_Object_Model">Document Object Model (DOM) API</a>, which allows you to manipulate documents.</p>
</div>

<h2 id="Language_basics_crash_course">Language basics crash course</h2>

<p>Let's explain some of the core features of the JavaScript language, to give you a better understanding&nbsp;of how it all works. It is worth noting that these features are common to all programming languages, so if you master these fundamentals, you're well on your way to being able to program just about anything!</p>

<div class="warning">
<p><strong>Important</strong>: In this article, try entering the example code lines into your JavaScript console to see what happens. For more details on JavaScript consoles, see <a href="/en-US/Learn/Discover_browser_developer_tools">Discover browser developer tools</a>.</p>
</div>

<h3 id="Variables">Variables</h3>

<p>{{Glossary("Variable", "Variables")}} are containers that you can store values in. You start by declaring a variable with the <code>var</code> keyword, followed by any name you want to call it:</p>

<pre class="brush: js">
var myVariable;</pre>

<div class="note">
<p><strong>Note</strong>: A semicolon at the end of a line indicates where a statement ends; it is only absolutely required when you need to separate statements on a single line. However,&nbsp;some people&nbsp;believe that&nbsp;it is a good practice to put them in at the end of each statement. There are other rules for when you should and shouldn't use them — see <a href="http://news.codecademy.com/your-guide-to-semicolons-in-javascript/">Your Guide to Semicolons in JavaScript</a> for more details.</p>
</div>

<div class="note">
<p><strong>Note</strong>: You can name a variable nearly anything, but there are some name restrictions (see <a href="http://www.codelifter.com/main/tips/tip_020.shtml">this article on variable naming rules</a>). If you are unsure, you can <a href="https://mothereff.in/js-variables">check your variable name</a> to see if it is valid.</p>
</div>

<div class="note">
<p><strong>Note</strong>: JavaScript is case sensitive — <code>myVariable</code> is a different variable to <code>myvariable</code>. If you are getting problems in your code, check the casing!</p>
</div>

<p>After declaring a variable, you can give it a value:</p>

<pre class="brush: js">
myVariable = 'Bob';</pre>

<p>You can do both these operations on the same line if you wish:</p>

<pre class="brush: js">
var myVariable = 'Bob';</pre>

<p>You can retrieve the value by just calling the variable by name:</p>

<pre class="brush: js">
myVariable;</pre>

<p>After giving a variable a value, you can later choose to change it:</p>

<pre>
var myVariable = 'Bob';
myVariable = 'Steve';</pre>

<p>Note that variables may hold values that have different <a href="/en-US/docs/Web/JavaScript/Data_structures">data types</a>:</p>

<table class="standard-table">
 <thead>
  <tr>
   <th scope="row">Variable</th>
   <th scope="col">Explanation</th>
   <th scope="col">Example</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <th scope="row">{{Glossary("String")}}</th>
   <td>A sequence of text known as a string. To signify that the value is a string, you must enclose it in quote marks.</td>
   <td><code>var myVariable = 'Bob';</code></td>
  </tr>
  <tr>
   <th scope="row">{{Glossary("Number")}}</th>
   <td>A number. Numbers don't have quotes around them.</td>
   <td><code>var myVariable = 10;</code></td>
  </tr>
  <tr>
   <th scope="row">{{Glossary("Boolean")}}</th>
   <td>A True/False value. The words <code>true</code> and <code>false</code> are special keywords in JS, and don't need quotes.</td>
   <td><code>var myVariable = true;</code></td>
  </tr>
  <tr>
   <th scope="row">{{Glossary("Array")}}</th>
   <td>A structure that allows you to store multiple values in one single reference.</td>
   <td><code>var myVariable = [1,'Bob','Steve',10];</code><br />
    Refer to each member of the array like this:<br />
    <code>myVariable[0]</code>, <code>myVariable[1]</code>, etc.</td>
  </tr>
  <tr>
   <th scope="row">{{Glossary("Object")}}</th>
   <td>Basically, anything. Everything in JavaScript is an object, and can be stored in a variable. Keep this in mind as you learn.</td>
   <td><code>var myVariable = document.querySelector('h1');</code><br />
    All of the above examples too.</td>
  </tr>
 </tbody>
</table>

<p>So why do we need variables? Well, variables are needed to do anything interesting in programming. If values couldn't change, then you couldn't do anything dynamic, like personalize a greeting message&nbsp;or change the image displayed in an image gallery.</p>

<h3 id="Comments">Comments</h3>

<p>You can put comments into JavaScript code, just as you can in CSS:</p>

<pre class="brush: js">
/*
Everything in between is a comment.
*/</pre>

<p>If your comment contains no line breaks,&nbsp;it's often easier to put it behind two slashes like this:</p>

<pre class="brush: js" style="font-size: 14px;">
// This is a comment
</pre>

<h3 id="Operators">Operators</h3>

<p>An <code>{{Glossary("operator")}}</code> is a mathematical symbol which produces a result based on&nbsp;two values (or variables). In the following table you can see some of the simplest operators, along with some examples to try out in the JavaScript console.</p>

<table class="standard-table">
 <thead>
  <tr>
   <th scope="row">Operator</th>
   <th scope="col">Explanation</th>
   <th scope="col">Symbol(s)</th>
   <th scope="col">Example</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <th scope="row">Addition</th>
   <td>Used to add two numbers together or glue two strings together.</td>
   <td><code>+</code></td>
   <td><code>6 + 9;<br />
    "Hello " + "world!";</code></td>
  </tr>
  <tr>
   <th scope="row">Subtraction, Multiplication, Division</th>
   <td>These do what you'd expect them to do in basic math.</td>
   <td><code>-</code>, <code>*</code>, <code>/</code></td>
   <td><code>9 - 3;<br />
    8 * 2; // multiply in JS is an asterisk<br />
    9 / 3;</code></td>
  </tr>
  <tr>
   <th scope="row">Assignment</th>
   <td>You've seen this already: it assigns a value to a variable.</td>
   <td><code>=</code></td>
   <td><code>var myVariable = 'Bob';</code></td>
  </tr>
  <tr>
   <th scope="row">Equality</th>
   <td>Does a test to see if two values are equal to one another and returns a <code>true</code>/<code>false</code> (Boolean) result.</td>
   <td><code>===</code></td>
   <td><code>var myVariable = 3;<br />
    myVariable === 4;</code></td>
  </tr>
  <tr>
   <th scope="row">Not, Does-not-equal</th>
   <td>Returns the logically opposite value of what it precedes; it turns a <code>true</code> into a <code>false</code>, etc. When it is used alongside the Equality operator, the negation operator tests whether two values are <em>not</em> equal.</td>
   <td><code>!</code>, <code>!==</code></td>
   <td>
    <p>The basic expression is <code>true</code>, but the comparison returns <code>false</code> because we've negated it:</p>

    <p><code>var myVariable = 3;<br />
     !(myVariable === 3);</code></p>

    <p>Here we are testing "is <code>myVariable</code> NOT equal to 3". This returns<code> false</code> because <code>myVariable</code> IS equal to 3.</p>

    <p><code><code>var myVariable = 3;</code><br />
     myVariable !== 3;</code></p>
   </td>
  </tr>
 </tbody>
</table>

<p>There are a lot more operators to explore, but this is enough for now. See <a href="/en-US/docs/Web/JavaScript/Reference/Operators">Expressions and operators</a> for a complete list.</p>

<div class="note">
<p><strong>Note</strong>: Mixing data types can lead to some strange results when performing calculations, so be careful that you are referring to your variables correctly, and getting the results you expect. For example, enter <code>"35" + "25"</code> into your console. Why don't you&nbsp;get the result you expected? Because the quote marks turn the numbers into strings, so&nbsp;you've ended up concatenating strings rather than adding numbers. If you enter, <code>35 + 25</code> you'll get the correct result.</p>
</div>

<h3 id="Conditionals">Conditionals</h3>

<p>Conditionals are code structures which allow you to test if an expression returns true or not, running alternative code revealed by its result. A very common form of conditionals is the&nbsp;<code>if ... else</code>&nbsp;statement. For example:</p>

<pre class="brush: js">
var iceCream = 'chocolate';
if (iceCream === 'chocolate') {
  alert('Yay, I love chocolate ice cream!');    
} else {
  alert('Awwww, but chocolate is my favorite...');    
}</pre>

<p>The expression inside the <code>if ( ... )</code> is the test — this uses the identity operator (as described above) to compare the variable <code>iceCream</code> with the string <code>chocolate</code> to see if the two are equal. If this comparison returns <code>true</code>, the first block of code is run. If the comparison is not true, the first block is skipped and the second code block, after the <code>else</code> statement, is run instead.</p>

<h3 id="Functions">Functions</h3>

<p>{{Glossary("Function", "Functions")}} are a way of packaging&nbsp;functionality that you wish to reuse. When you need the procedure you can call a function, with the&nbsp;function name, instead of rewriting the entire code each time.&nbsp;You have already seen some uses of functions above, for example:</p>

<ol>
 <li>
  <pre class="brush: js">
var myVariable = document.querySelector('h1');</pre>
 </li>
 <li>
  <pre class="brush: js">
alert('hello!');</pre>
 </li>
</ol>

<p>These functions, <code>document.querySelector</code> and <code>alert</code>, are built into the browser for you to use whenever you desire.</p>

<p>If you see something which looks like a variable name, but has parentheses — <code>()</code> — after it, it is likely a function. Functions often take {{Glossary("Argument", "arguments")}} — bits of data they need to do their job. These go&nbsp;inside the parentheses, separated by commas if there is more than one argument.</p>

<p>For example, the <code>alert()</code> function makes a pop-up box appear inside the browser window, but we need to give it a string as an argument to tell the function&nbsp;what to&nbsp;write in the pop-up box.</p>

<p>The good news is you can define your own functions — in this next example we write a simple function which takes two numbers as arguments and multiplies them:</p>

<pre class="brush: js">
function multiply(num1,num2) {
  var result = num1 * num2;
  return result;
}</pre>

<p>Try running the above function in the console, then test with several arguments. For example:</p>

<pre class="brush: js">
multiply(4,7);
multiply(20,20);
multiply(0.5,3);</pre>

<div class="note">
<p><strong>Note</strong>: The <a href="/en-US/docs/Web/JavaScript/Reference/Statements/return"><code>return</code></a> statement tells the browser to return the <code>result</code> variable out of the function so it is available to use. This is necessary because variables defined inside functions are only available inside those functions. This is called variable {{Glossary("Scope", "scoping")}}. (Read <a href="/en-US/docs/Web/JavaScript/Guide/Values,_variables,_and_literals#Variable_scope">more on variable scoping</a>.)</p>
</div>

<h3 id="Events">Events</h3>

<p>Real interactivity on a website needs events. These are code structures which listen for things happening in browser, running code in response. The most obvious example is the <a href="/en-US/docs/Web/Events/click">click event</a>, which is fired by the browser when you click on something with your mouse. To demonstrate this, enter the following into your console, then click on the current webpage:</p>

<pre class="brush: js">
document.querySelector('html').onclick = function() {
    alert('Ouch! Stop poking me!');
}</pre>

<p>There are many ways to attach an event to an element. Here&nbsp;we select the {{htmlelement("html")}} element, setting its <code><a href="/en-US/docs/Web/API/GlobalEventHandlers.onclick">onclick</a></code> handler property equal to an anonymous (i.e. nameless) function, which contains the code we want the click event to run.</p>

<p>Note that</p>

<pre class="brush: js">
document.querySelector('html').onclick = function() {};</pre>

<p>is equivalent to</p>

<pre class="brush: js">
var myHTML = document.querySelector('html');
myHTML.onclick = function() {};</pre>

<p>It's just shorter.</p>

<h2 id="Supercharging_our_example_website">Supercharging our example website</h2>

<p>Now we've gone over&nbsp;a few JavaScript basics, let's add a few cool features to our example site to see what is possible.</p>

<h3 id="Adding_an_image_changer">Adding an image changer</h3>

<p>In this section, we'll add an additional image to our site using some more DOM API features, using some JavaScript to switch between the two when the image is clicked.</p>

<ol>
 <li>First of all, find another image you'd like to feature on your site. Be sure it is the same size as the first image, or as close as possible.</li>
 <li>Save this image in your <code>images</code> folder.</li>
 <li>Rename this image 'firefox2.png' (without quotes).</li>
 <li>Go to your <code>main.js</code> file, and enter the following JavaScript. (If your "hello world" JavaScript is still there, delete it.)
  <pre class="brush: js">
var myImage = document.querySelector('img');

myImage.onclick = function() {
    var mySrc = myImage.getAttribute('src');
    if(mySrc === 'images/firefox-icon.png') {
      myImage.setAttribute ('src','images/firefox2.png');
    } else {
      myImage.setAttribute ('src','images/firefox-icon.png');
    }
}</pre>
 </li>
 <li>Save all files and load <code>index.html</code> in the browser. Now when you click the image, it should change to the other one!</li>
</ol>

<p>You store a reference to your {{htmlelement("img")}} element in the <code>myImage</code> variable. Next, you make this variable's <code>onclick</code> event handler property equal to a function with no name (an "anonymous" function). Now, every time this&nbsp;element is clicked:</p>

<ol>
 <li>You retrieve the value of the image's <code>src</code> attribute.</li>
 <li>You use a conditional to check whether the <code>src</code> value is equal to the path to the original image:
  <ol>
   <li>If it is, you change the <code>src</code> value to the path to the 2nd image, forcing the other image to be loaded inside the {{htmlelement("img")}} element.</li>
   <li>If it isn't (meaning it must already have changed), the <code>src</code> value swaps back to the original image path, to the original state.</li>
  </ol>
 </li>
</ol>

<h3 id="Adding_a_personalized_welcome_message">Adding a personalized welcome message</h3>

<p>Next we will add another bit of code, changing the page's title to a personalized welcome message when the user first navigates to the site. This welcome message will persist, should the user leave the site and later return — we will save it using the <a href="/en-US/docs/Web/API/Web_Storage_API">Web Storage API</a>. We will also include an option to change the user and, therefore, the welcome message anytime it is required.</p>

<ol>
 <li>In <code>index.html</code>, add the following line just before the {{htmlelement("script")}} element:

  <pre class="brush: html">
&lt;button&gt;Change user&lt;/button&gt;</pre>
 </li>
 <li>In <code>main.js</code>, place the following code at the bottom of the file, exactly as written — this takes references to the new button and the heading, storing them inside variables:
  <pre class="brush: js">
var myButton = document.querySelector('button');
var myHeading = document.querySelector('h1');</pre>
 </li>
 <li>Now add the following function to set the personalized greeting — this won't do anything yet, but we'll fix this in a moment:
  <pre class="brush: js">
function setUserName() {
  var myName = prompt('Please enter your name.');
  localStorage.setItem('name', myName);
  myHeading.textContent = 'Mozilla is cool, ' + myName;
}</pre>
  This function contains a <a href="/en-US/docs/Web/API/Window.prompt"><code>prompt()</code></a> function, which brings up a dialog box, a bit like <code>alert()</code>. This <code>prompt()</code>, however, asks the user to enter some data, storing it in a variable after the user presses <strong>OK</strong><em>.</em>&nbsp;In this case, we are asking the user to enter their name. Next, we call on an API called <code>localStorage</code>, which allows us to store data in the browser&nbsp;and later retrieve it. We use localStorage's <code>setItem()</code> function to create and store a data item called <code>'name'</code>, setting its value to the <code>myName</code> variable which contains the data the user entered. Finally, we set the <code>textContent</code> of the heading to a string, plus the user's newly stored name.</li>
 <li>Next, add this <code>if ... else</code> block — we could call this the initialization code, as it structures the app when it first loads:
  <pre class="brush: js">
if(!localStorage.getItem('name')) {
  setUserName();
} else {
  var storedName = localStorage.getItem('name');
  myHeading.textContent = 'Mozilla is cool, ' + storedName;
}</pre>
  This block first uses the negation operator (logical NOT, represented by the !) to check whether the <code>name</code> data exists. If not,&nbsp;the <code>setUserName()</code> function is run to create it. If it exists (that is, the user set it during a previous visit), we retrieve the stored name using <code>getItem()</code> and set the <code>textContent</code> of the heading to a string, plus the user's name, as we did inside <code>setUserName()</code>.</li>
 <li>Finally, put the below <code>onclick</code> event handler on the button. When clicked, the <code>setUserName()</code> function is run. This allows the user to set a new name, when they wish, by pressing the button:
  <pre class="brush: js">
myButton.onclick = function() {
&nbsp; setUserName();
}
</pre>
 </li>
</ol>

<p>Now when you first visit the site, it will ask you for your username, then give you a personalized message. You can change the name any time you like by pressing the button. As an added bonus, because the name is stored inside localStorage, it persists after the site is closed down, keeping the personalized message there when you next open the site!</p>

<h2 id="Conclusion">Conclusion</h2>

<p>If you have followed all the instructions in this article, you should end up with a page that looks something like this (you can also <a href="https://mdn.github.io/beginner-html-site-scripted/">view our version here</a>):</p>

<p><img alt="" src="https://mdn.mozillademos.org/files/9539/website-screen-scripted.png" style="display:block; height:995px; margin:0px auto; width:800px" /></p>

<p>If you get stuck, you can compare your work with our <a href="https://github.com/mdn/beginner-html-site-scripted/blob/gh-pages/scripts/main.js">finished example code on GitHub</a>.</p>

<p>We have barely scratched the surface of JavaScript. If you have enjoyed playing, and wish to advance even further, head to our <a href="/en-US/docs/Learn/JavaScript">JavaScript learning topic</a>.</p>

<p>{{PreviousMenuNext("Learn/Getting_started_with_the_web/CSS_basics", "Learn/Getting_started_with_the_web/Publishing_your_website", "Learn/Getting_started_with_the_web")}}</p>

<p>&nbsp;</p>

<h2 id="In_this_module">In this module</h2>

<ul>
 <li id="Installing_basic_software"><a href="/en-US/Learn/Getting_started_with_the_web/Installing_basic_software">Installing basic software</a></li>
 <li id="What_will_your_website_look_like"><a href="/en-US/Learn/Getting_started_with_the_web/What_will_your_website_look_like">What will your website look like?</a></li>
 <li id="Dealing_with_files"><a href="/en-US/Learn/Getting_started_with_the_web/Dealing_with_files">Dealing with files</a></li>
 <li id="HTML_basics"><a href="/en-US/Learn/Getting_started_with_the_web/HTML_basics">HTML basics</a></li>
 <li id="CSS_basics"><a href="/en-US/Learn/Getting_started_with_the_web/CSS_basics">CSS basics</a></li>
 <li id="JavaScript_basics"><a href="/en-US/Learn/Getting_started_with_the_web/JavaScript_basics">JavaScript basics</a></li>
 <li id="Publishing_your_website"><a href="/en-US/Learn/Getting_started_with_the_web/Publishing_your_website">Publishing your website</a></li>
 <li id="How_the_web_works"><a href="/en-US/Learn/Getting_started_with_the_web/How_the_Web_works">How the web works</a></li>
</ul>

<p>&nbsp;</p>

