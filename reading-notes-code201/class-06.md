# Code 201, 2 Jan, Read-06
### Object Literals
A **JavaScript object literal** is a comma-separated list of name-value pairs wrapped in curly braces. Object literals encapsulate data, enclosing it in a tidy package. This minimizes the use of global variables which can cause problems when combining code.
```javascript
var myObject = {
    sProp: 'some string value',
    numProp: 2,
    bProp: false
};
```
## Object Literal Syntax

Object literals are defined using the following syntax rules:

-   A colon separates property name  from value.
-   A comma separates each name-value pair from the next.
-   A comma after the last name-value pair is optional.
 ## Why and How We Use Object Literals
 
Object literals enable us to write code that supports lots of features yet still provide a relatively straightforward process for implementers of our code. No need to invoke constructors directly or maintain the correct order of arguments passed to functions. Object literals are also useful for unobtrusive event handling; they can hold the data that would otherwise be passed in function calls from HTML event handler attributes.
```javascript
var museam = {
    // an array literal
    images: ["leo.gif", "mikel.gif"],
    onSwap: function() { // function
        // code here
    }
};
```

## DOM Document Object Model

The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.

- The DOM specifies the way in which the browser should structure this model using a DOM tree.
- Each object represents a different part of the page loaded in the browser window.

![](https://cf.ppt-online.org/files/slide/l/lG6hjyFR8carDYH7oVAtPW3exEOg0sSpQ1JKfm/slide-4.jpg)
#### Three common ways to select an individual element:
- ```getElementByld ()```
- ```querySelector ()```
- You can also select individual elements by traversing from one element to another within the DOM tree (see third column).

####  Three common ways to select multiple elements.
- ```getElementsByClassName()```
- ```getElementsByTagName()```
- ```querySelectorAll()```

#### You can move from one element node to a related element node.
- ```parentNode```
- ```previousSibl ing / nextSibl ing```
- ```firstChild / lastChild```