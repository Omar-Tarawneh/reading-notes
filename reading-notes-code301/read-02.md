# Read-02, 14 Feb 2021, Code 301

## PAIR PROGRAMMING

![pair](https://martinfowler.com/articles/on-pair-programming/driver_navigator.png)

When you do **pair programming** the chance you make and error is less, and debugging become more easier so you can be more productive in writing code and finish you project sooner.

Also It's fun that you can work with your colleagues and that not occurring too much on other industries.

How It's work?
pair programming involves two roles: the Driver and the Navigator.
we experience this during code 201 and 102

* The Driver is the programmer who is typing and the only one whose hands are on the keyboard.
 * The Navigator uses their words to guide the Driver but does not provide any direct input to the computer.

## jQuery 

It's used to be the most popular framework in **JS**.
 jQuery offers a simple way to achieve a variety of common JavaScript tasks quickly and consistently, across all major browsers and without any fallback code needed.
* It' simpler to access elements using jQuery CSS-style selector
* Having method let you update the DOM tree, animate elements with one line of code.
* Handling Events in much easier way than DOM.

The jQuery library contains the following features:

-   HTML/DOM manipulation
-   CSS manipulation
-   HTML event methods
-   Effects and animations
-   AJAX
-   Utilities

The way you can insert jQuery:
-   Download the jQuery library from jQuery.com
-   Include jQuery from a CDN, like Google

Syntax:**$(_selector_)._action_()**


example:
`$(this).hide()`  - hides the current element.

`$("p").hide()`  - hides all `<p>` elements.

`$(".test").hide()`  - hides all elements with class="test".

`$("#test").hide()`  - hides the element with id="test".


```javascript
$(document).ready(function(){  
$("p").click(function(){  
$(this).hide();  
});  
});
```

My GitHub Page Link: [Read02 Link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code301/read-02)