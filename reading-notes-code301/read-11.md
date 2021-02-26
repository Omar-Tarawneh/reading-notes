# Read-11, 27 Feb 2021, Code 301

## EJS 

![ejs](https://miro.medium.com/max/3920/1*5xR5P6dzu4LpyMaR2QMphA.jpeg)

EJS is a simple templating language that lets you generate HTML markup with plain JavaScript. No religiousness about how to organize things. No reinvention of iteration and control-flow. It's just plain JavaScript.

#### Advantages

* Use plain JavaScript
* Fast development time
*  Simple syntax
* Speedy execution
*  Active development


#### Installing

```bash
$ npm install ejs
```

#### How to Use

```javascript
let ejs = require('ejs');
let people = ['geddy', 'neil', 'alex'];
let html = ejs.render('<%= people.join(", "); %>', {people: people});
```


## Google API

This document is intended for developers who want to write applications that can interact with the Books API.
```https://www.googleapis.com/auth/books```

You can perform a volumes search by sending an HTTP `GET` request to the following URI:
```https://www.googleapis.com/books/v1/volumes?q=search+terms```

This request has a single required parameter:

-   `[q](https://developers.google.com/books/docs/v1/using#q)`  - Search for volumes that contain this text string. There are special keywords you can specify in the search terms to search in particular fields


[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code301/read-11)