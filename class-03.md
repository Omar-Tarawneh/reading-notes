# Code 201, 29th Dec, Read-03

## HTML list & Boxes

### Lists

HTML offers web authors three ways for specifying lists of information. All lists must contain one or more list elements. Lists may contain −

- `<ul>` − An unordered list. This will list items using plain bullets.
- `<ol>` − An ordered list. This will use different schemes of numbers to list your items.
- `<dl>` − A definition list. This arranges your items in the same way as they are arranged in a dictionary.

```HTML

<!DOCTYPE html>
  <html>
  <head>  <title>HTML Definition List</title>  </head>
  <body>
    <dl>
    <dt><b>HTML</b></dt>
    <dd>This stands for Hyper Text Markup Language</dd>
    <dt><b>HTTP</b></dt>
    <dd>This stands for Hyper Text Transfer Protocol</dd>
    </dl>
    </body>
```

### Boxes

All **HTML** elements can be considered as boxes. In **CSS**, the term "box model" is used when talking about design and layout.
![Box model](https://azahreba.gitbooks.io/html101/content/02_css/img/box-model.png)

## Switch Statement

A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value.

```Javascript
switch (level) {
 case 'One ':
 title= 'Level 1 ' ;
 break;
 case 'Two':
 title = ' Level 2 ' ;
 break;
 case ' Three' :
 title = 'Level 3' ;
 break ;
 default :
 title= 'Test';
 break;
 }

```
