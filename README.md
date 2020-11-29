# kottans-frontend
## Git and GitHub
Not quite clear at first, it became clear later. Absolutely like [gitbranching](https://learngitbranching.js.org/).  
Almost all the commands were new to me, Git is logical, understandable, surprisingly interesting. Can't wait using branches and resolving merge conflicts!

## Linux CLI, and HTTP
I was impressed to discover the command line capabilities. Command line is cool! Who needs UI?

[x] [Linux Survival](task_linux_cli/linux-survival.png)  
[x] Read the article "HTTP: The Protocol Every Web Developer Must Know"  
[ ] Good understanding of http:  

Absolutely need more info about The Protocol every developer must know.

## Git Collaboration
What's new:  
- multiple remote directories  
- difference between `git fetch` and `git pull`  
- contributing via forking repos  
- `git log --oneline --graph --decorate --all`  

To contribute  
- read CONTRIBUTING.md file  
- use topic branch
- make frequent, smaller commits
- be clear and polite

Here are my screenshots:  
[Version Control with Git, Udacity](task_git_collaboration/version-control-with-git.png)  
[GitHub & Collaboration, Udacity](task_git_collaboration/github-and-collaboration.png)  

Definitely going to make a lot of pull requests, hope to contribute in future))

## Intro to HTML and CSS 
What was new to me:
- fallback fonts
- adding local fonts to a document with the `@font-face` property
- `margin: 0 auto`
- vertical margins collapse
- HSL colors
- relative sizing unit — `fr`
- CSS transitions
- how `clear` property works

What surprised me - how much I liked it, not just learning new rulesets, but writing my own lines of code.

Interested in more practice with:
- CSS selectors
- `position` and `display` properties
- grids
- elegant flexboxes

Screenshots:  
[Intro to HTML & CSS, Udacity](task_html_css_intro/intro-to-html-css-udacity.png)  
[Learn HTML, codecademy](task_html_css_intro/learn-html-codecademy.png)  
[Learn CSS, codecademy](task_html_css_intro/learn-css-codecademy.png)  
[HTML & CSS free lesson on HTML Academy](task_html_css_intro/html-css-free-lesson-htmlacademy.png)  


## Responsive Web Design 
What became a useful discovery to me:
- media queries, breakpoints
- common responsive patterns: column drop, mostly fluid, layout shifter, off canvas
- responsive tables techniques
- the browser reports the width in DIPs (remember about a device pixel ratio)
- good to use: relative units, font-boosting, common sense

What surprised me? There is another big topic to learn - responsive images!
What do I intend to use in future? Any technique or tip that will help me to do the layout responsive and the site more user-friendly!

My screenshots:   
[Responsive Web Design Fundamentals, Udacity](task_responsive_web_design/responsive-web-design-fundamentals-udacity.png)  
[Flexbox Froggy](task_responsive_web_design/flexbox-froggy.png)  

## HTML & CSS practice: Hooli-style Popup
It was great!! I missed some instructions and spent a lot of time trying to make the popup look exactly like on the picture. Good lesson for me to be more attentive.   
I learned how to make a little triangle so that popup looks like going from definite icon. I trained to use flexbox, made my first real commits, understood they must be more frequent. It was pleasure to write code, so as rewrite.

## JS Basics
Notes I leave here (and what was new):
* JS - loosely typed programming language
* data types: boolean, null, undefined, number, string, symbol and Object
* use camelCase for variables
* ternary operator
* functions, powerful and complicated, callback
* `const`, `let`, `var` variables, block and global scope
* destructuring assignment
* Functional programming: pure, isolated functions, avoid mutations and side effects, always declare dependencies and stay calm!

Screenshots:  
[Intro to JS, Udacity](task_js_basics/intro-to-javascript-udacity.png)  
[Basic JS, freecodecapm](task_js_basics/basic-javascript-freecodecamp.png)  
[ES6, freecodecapm](task_js_basics/es6-freecodecamp.png)  
[Basic Data Srucrutes, freecodecapm](task_js_basics/basic-data-structures-freecodecamp.png)  
[Basic Algorithm Scripting, freecodecapm](task_js_basics/basic-algorithm-scripting-freecodecamp.png)  
[Functional Programming, freecodecapm](task_js_basics/functional-programming-freecodecamp.png)  
[Intermediate Algorithm Scripting, freecodecapm](task_js_basics/intermediate-algorithm-scripting-freecodecamp.png)  

## Document Object Model  
**What was new to me:**  
- what DOM is, as a representation of HTML  
- to access to DOM use a special object `document`, which is expected to already exist  
- `document` and `element` objects methods  
- use Document Fragment to create a DOM subtree within it and then append the DOM  
- reflow & repaint
- JS is single-threaded, uses The Call Stack (which basically a list of the functions that are running)  
- events: the target, the type, the listener  
- event delegation
- event loop, and queue

**What surprised me** was how easy we can make changes to html document using DOM methods.  
It would be good to minimize browser reflow, and get a clear understanding of synchronicity of JS.  
**What you intend to use in future** - DOM methods, events. Every single lesson of Udacity's DOM course made me close to understanding how JavaScript works.

My screenshots:  
[JS and the DOM, Udacity](task_js_dom/javascript-and-the-dom-udacity.png)  
[Intermediate Algorithm Scripting, freecodecapm](task_js_dom/intermediate-algorithm-scripting-freecodecamp.png)

## A tiny JS world  
What surprised me was how much debug could be needed in my project!

Not in vain I read the article about **copying objects in JS:**  
 - the assignment operator doesn't create a copy, but assigns a reference to copied object  
 - if you copy object by looping through it you are naive  
 - shallow copy `Object.assign()` duplicate top-level properties, but nested objects are shared between source and target  
 - deep copy speaks for itself, but it doesn't copy user-defined object methods  
 - shallow copy works for copying circular objects, deep copy doesn't
 - to copy object use `extend`, to copy a reference `Object.create()`

## Object-Oriented JavaScript  
I'm excited about Udacity course, I wish I had an eidetic memory to remember all the information I learn!
About course, things that surprised me, or which were new are countless. So I'll leave all my notes here.  
**About scopes:**  
- lexical scope - built as the code is written, curl braces `{}` make a new scope  
- there is a global scope, which includes all written code 
- curl braces `{}` of `if/loop` constructions don't create a new scope  
- execution contexts (in memory scope) are built as the code runs  
- to retain access to function from outer scope:
  - save that function to a global variable
  - return function from its outer function
  - pass to setTimeout  
**Keyword `this`:**  
- keyword `this` bound to the object found to the left of the dot where the containing function is called
- `this` as a parameter of the method indication
- use `.call` to bound `this` to needed object
- using `new` bounds `this` to brand new object
**Prototype chain:**  
- object which holds a link to another object is its prototype
- prototype chain makes objects look similar to other objects
- `instanceof` operator checks if the prototype property of a constructor appears anywhere in the prototype chain of an object
**Functional class pattern:**  
- the class **builds** the object that it's going to augment, whereas he decorator **accepts** the object that it's going to augment as an input
- to add methods to class make them **properties** of class function
**Prototypal class pattern:**  
- it is: function to make instances, the line inside to generate a new instance object, a prototype with properties and making instance delegate to that prototype
- keyword `prototype` to describe the methods container object
- someObj's prototype is `someObj.prototype`
- `prototype.constructor` property
**Pseudo-classical class pattern:**  
- magic keyword `new` for constructor mode
**Superclass and subclasses:**  
- it is good idea for avoiding duplicating code
- `.call` method to call the needed function (invoke class) in the right context with the parameter `this`
- to delegate from subclass `.prototype` object to superclass `.prototype` use `Object.create`
- set the subclass' constructor to the right constructor
- add additional extra functionality, and voila!

I intend to use prototype chain, pseudo-classical pattern, subclassing, keyword `this`, and every single bit of knowledge, which could be needed in writing good code. 
Absolutely love [codewars](https://www.codewars.com/), love math and this is the gift - the perfect way to spend free time for me)) 

Screenshots:  
[OOP, Udacity](task_js_oop/object-oriented-js-udacity.png)  
[My codewars progress](task_js_oop/codewars_7kyu.png), [my profile](https://www.codewars.com/users/Lu-sure)
