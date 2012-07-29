#Job Interview Questionnaire

@version 1.0
 
## Resume Questions:

* For each job on their resume (or a handful if it’s packed):
	* How did you get this job?
	* Before you left, what did you like about it?
	* Why did you leave?

## General Questions:

* Are you on Twitter? 
	* If so, who do you follow on Twitter?
* Are you on Github? 
	* If so, what are some examples of repositories you follow  
* What blogs do you follow? 
* What version control systems have you used? 
* What is your preferred development enviroment? (OS, Editor, Browsers, Tools, etc.) 
* Can you describe your workflow when you create a web page? 
* Can you describe the difference between progressive enhancement and graceful degredation? 
	* Bonus points for knowing they are related but philosophically different
	* Which philosophy guides your work?
	* How do you integrate it?
		* Extra bonus points for describing feature detection  
* Explain what "Semantic HTML" means. 
* What does "minification" do? 
* Why is it better to serve site assets from multiple domains? 
	* How many resources will a browser download from a given domain at a time?  
* If you have 8 different stylesheets for a given design, how would you integrate them into the site? 
	* Looking for file concatenation.
	* Points off for `@import`, unless it works in conjunction with a build system.  
* If you jumped on a project and they used tabs and you used spaces, what would you do?
	* Bonus points for "check with the team’s standards guide and adapt accordingly"
* What tools do you use to test your code's performance? 
* If you could master one technology this year, what would it be? 
* Name 3 ways to decrease page load. (perceived or actual load time)
* Explain the importance of standards.  

## HTML-Specific Questions:

* What's a `doctype` do, and how many can you name? 
* What's the difference between "standards mode" and "quirks mode"? 
* How do you serve a page with content in multiple languages? 
* Can you use XHTML syntax in HTML5? How do you use XML in HTML5? 
* What are `data-` attributes good for? 
* What are the content models in HTML4 and are they different in HTML5? 
* Consider HTML5 as an open web platform. What are the building blocks of HTML5? 
* Describe the difference between cookies, sessionStorage and localStorage.  
* Explain the purpose of `class` and `id` attributes.

## CSS-Specific Questions:

* Describe what a "reset" CSS file does and how it's useful. 
* Describe CSS Floats and how they work. 
* Describe the various CSS positioning values and what they do.
* What are the various clearing techniques and which is appropriate for what context? 
* Explain CSS sprites, and how you would implement them on a page or site. 
* What are the differences between the IE box model and the W3C box model? 
	* Bonus points for knowing `box-sizing` lets you switch between the two (border and padding)
* What are your favourite image replacement techniques and which do you use when? 
* How do you manage your CSS hacks, filters and workarounds? CSS property hacks, conditionally included .css files, or... something else? 
* Have you used or implement media queries or mobile specific layouts/CSS? 
* How do you serve your pages for feature-constrained browsers? 
	* What techniques/processes do you use? 
	* Bonus points for mobile-first media queries
* What are the different ways to visually hide content (and make it available only for screen readers)? 
* Have you ever used a grid system, and if so, what do you prefer? 
* Any familiarity with styling SVG? 
* How do you optimize your web pages for print? 
* What are some of the "gotchas" for writing efficient CSS? 
* Do you use SASS/Compass or LESS? 
	* If you use LESS, do you compile in the browser?
		* Points off for yes.
* How would you implement a web design comp that uses non-standard fonts? (avoid mentioning webfonts so they can figure it out) 
* Explain how a browser determines what elements match a CSS selector.

## Basic JS-Specific Questions

* How is JavaScript different from Java? 
* Which JavaScript libraries have you used?
	* Which have you liked?
* Do you ascribe to a articular coding style?
* What are `undefined` and `undeclared` variables?
* How are `null` and `undefined` different?
* What is the difference between `==` and `===`? 
* What's the difference between host objects and native objects? 
* When do you optimize your code? 
* What is a closure, and how/why would you use one? 
	* Your favorite pattern used to create them?
* Difference between: 
```javascript
function Person(){}
var person = Person();
var person = new Person();
```
* When would you use `document.write()`? 
	* Correct answer: 1999 - time to weed out the junior devs  
* What's the difference between feature detection, feature inference, and using the UA string 
* What's the difference between an "attribute" and a "property"? 
* What is FOUC? How do you avoid FOUC? 
* Difference between document load event and document ready event? 
* Explain how you would get a query string parameter from the browser window's URL. 
* Describe event bubbling. 
* Explain event delegation. 
* What is a Ternary statement?
	* What does the word "Ternary" indicate? 

## Advanced JS-Specific Questions

* Explain AJAX in as much detail as possible 
* Explain how JSONP works (and how it's not really AJAX) 
* Explain the same-origin policy with regards to JavaScript. 
v* What's a typical use case for anonymous functions? 
* Can you explain how inheritance works in JavaScript? 
	* Bonus points for the funny answer: "no one can" 
	* Extra bonus points if they take a stab at explaining it  
* Explain the "JavaScript module pattern" and when you'd use it. 
	* Bonus points for mentioning clean namespacing. 
	* What if your modules are namespace-less?  
* How do you organize your code? (module pattern? classical inheritance?)
* What's the difference between `.call` and `.apply`? 
* explain `Function.prototype.bind`? 
* Have you ever used JavaScript templating, and if so, what/how? 
* Explain "hoisting". 
* Why is extending built in JavaScript objects not a good idea? 
	* Why is extending built ins a good idea? 
	* Make this work: 
	```javascript
	[1,2,3,4,5].duplicator(); // [1,2,3,4,5,1,2,3,4,5]
	```
* Describe inheritance patterns in JavaScript. 
* Describe a strategy for memoization (avoiding calculation repetition) in JavaScript. 
* What is the arity of a function?  

## JS-Code Examples:

```javascript
>~~3.14
```
Question: What value is returned from the above statement? 
**Answer: 3** 

```javascript
"i'm a lasagna hog".split("").reverse().join("");
```
Question: What value is returned from the above statement? 
**Answer: "goh angasal a m'i"** 

```javascript
( window.foo || ( window.foo = "bar" ) );
```
Question: What is the value of window.foo? 
**Answer: "bar"** 
if intially window.foo was false, undefined or zero else it will retain its value.

```javascript
var foo = "Hello";
(function() {
	var bar = " World";
	alert(foo + bar);
})();
alert(foo + bar);
```
Question: What is the outcome of the two alerts above? 
**Answer: "Hello World" & ReferenceError: bar is not defined** 

## jQuery-Specific Questions:

* Explain "chaining". 
* What does `.end()` do? 
* How, and why, would you namespace a bound event handler? 
* What is the effects (or fx) queue? 
* What is the difference between `.get()`, `[]`, and `.eq()`? 
* What is the difference between `.bind()`, `.live()`, and `.delegate()`? 
	* How does `.on()` factor in?
* What is the difference between `$` and `$.fn`? Or: What is `$.fn`?
* Optimize this selector: 
```javascript
$(".foo div#bar:eq(0)")
```

## Optional fun Questions:

* What's the coolest thing you've ever coded, what are you most proud of? 
* Are you now, or have you ever been, on a boat. 
* Tell me your favorite parts about Firebug / Webkit Inspector. Least favorite?
* Do you have any pet projects? What kind? 
* On a piece of paper, write down the letters A B C D E vertically. Now put these in descending order without writing one line of code. 
	* Wait and see if they turn the paper upside down
	* This should make the laugh and is a fine way to relieve some tension at the end of the interview.  
* Pirate or Ninja? 
	* Bonus if it's a combo and a good reason was given (+2 for zombie monkey pirate ninjas) 
* If not Web Development what would you be doing? 
* Complete this sentence: Brendan Eich and Doug Crockford are the __________ of javascript.


##Contributors

@bentruyman (http://bentruyman.com/), @roger_raymond (http://twitter.com/iansym), @ajpiano (http://ajpiano.com/), @paul_irish (http://paulirish.com/), @SlexAxton (http://alexsexton.com/), @boazsender (http://boazsender.com/), @miketaylr (http://miketaylr.com/), @vladikoff (http://vladfilippov.com/), @gf3 (http://gf3.ca/), @jon_neal (http://twitter.com/jon_neal), @wookiehangover (http://wookiehangover.com/) and @darcy_clarke (http://darcyclarke.me), Aaron Gustafson (@AaronGustafson)