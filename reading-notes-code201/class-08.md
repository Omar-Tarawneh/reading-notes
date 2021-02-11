# Code 201, 5th Jan, Read-08

## HTML & CSS Layout

The website is consist usually of header, navigation bar, body or main content, side content, and footer from **CSS** you can control this using some properties.
![Layout](https://media.geeksforgeeks.org/wp-content/uploads/website_layout-300x268.png)
you can do the following:

* Controlling the position of elements 
* Creating site layouts  
* Designing for different sized screens

Here is an Example:

```css
/* The navbar container */  
.topnav {  
overflow:  hidden;  
background-color:  #333;  
}  
  
/* Navbar links */  
.topnav a {  
float:  left;  
display:  block;  
color:  #f2f2f2;  
text-align:  center;  
padding:  14px 16px;  
text-decoration:  none;  
}  
  
/* Links - change color on hover */  
.topnav a:hover {  
background-color:  #ddd;  
color:  black;  
}
```

## Footer

The footer is placed at the bottom of your page. It often contains information like copyright and contact info:

```css
.footer {  
background-color:  #F1F1F1;  
text-align:  center;  
padding:  10px;  
}
```

There is also a lot of thing you can do like placing the content in the side and something else.
Reference:
[HTML & CSS](https://wtf.tw/ref/duckett.pdf)