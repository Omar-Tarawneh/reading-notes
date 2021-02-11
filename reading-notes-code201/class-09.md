# Code 201, 6th Jan, Read-09

## HTML & CSS Forms

Forms basically allow you to collect data from the users.
and that can happen by providing the users of input field 
> The **HTML  `<form>`  element** represents a document section containing interactive controls for submitting information.

![form](https://i2.wp.com/www.tutorialbrain.com/wp-content/uploads/2019/01/HTML-Form.jpg?fit=1920%2C1080&ssl=1)

Here is an example of forms using **HTML**:

```html
<form action="" method="get" class="form-example">
  <div class="form-example">
    <label for="name">Enter your name: </label>
    <input type="text" name="name" id="name" required>
  </div>
  <div class="form-example">
    <label for="email">Enter your email: </label>
    <input type="email" name="email" id="email" required>
  </div>
  <div class="form-example">
    <input type="submit" value="Subscribe!">
  </div>
</form>
```

**Forms** used along with **Input**
you can use form to several things like:

* password field
* text entry
* Uploading Files
* Making Choices

## Lists, Tables & Forms

Using CSS you can change the style of lists, table and forms using specific property that has specific values for example:

* Bullet Point Styles
	* ```list-style-type```

* Positioning the Marker
	* ```list-style-position```


## Events in JS

Events is basically **things** that happen when you browsing the internet something like double click, scroll down, click, and everything you can think out. and how you website JS respond to it.
here is some example on JS events in Html file:

```java script
<button onclick="document.getElementById('demo').innerHTML = Date()">The time is?</button>
<_element_ _event_=**"**_**some JavaScript**_**"**>
```

Reference
[Html&Css](https://wtf.tw/ref/duckett.pdf)

[My GitHub Page](https://omar-tarawneh.github.io/reading-notes/class-09)
