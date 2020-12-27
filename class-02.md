# Code 201, Class-02, 27th Dec

## HTML & CSS

### TEXT

When creating a **web page**, you add tags
(known as markup) to the contents of the
page. These tags provide extra meaning
and allow browsers to show users the
appropriate structure for the page.

There are two type of markup:

- Structural markup: the elements that you can use to
  describe both headings and paragraphs
- Semantic markup: which provides extra information; such
  as where emphasis is placed in a sentence, that something
  you have written is a quotation (and who said it), the
  meaning of acronyms, and so on

_*Heading*_ Example

```Html
<h1>This is a Main Heading</h1>
<h2>This is a Level 2 Heading</h2>
<h3>This is a Level 3 Heading</h3>
<h4>This is a Level 4 Heading</h4>
<h5>This is a Level 5 Heading</h5>
<h6>This is a Level 6 Heading</h6>
```

_*Paragraph*_

```Html
<p>Hello my name is Omar Tarawneh I'm using these tags to create a pragraph</p>
```

_*Bold & Italic tags*_

```html
<p>This is how we make a word appear <b>bold.</b></p>
<p>This is how we make a word appear <i>italic</i>.</p>
```

Those are example regarding the _Structural Markup_ you can read more about them in [HTML&CSS](https://wtf.tw/ref/duckett.pdf)

I will give you an code example that will contain both **Structural & Semantic Markup**

```HTML

<html>
<head>
 <title>Text</title>
</head>
<body>
 <h1>The Story in the Book</h1>
 <h2>Chapter 1</h2>
 <p>Molly had been staring out of her window for about
 an hour now. On her desk, lying between the copies
 of <i>Nature</i>, <i>New Scientist</i>, and all
 the other scientific journals her work had
 appeared in, was a well thumbed copy of <cite>On
 The Road</cite>. It had been Molly's favorite book
 since college, and the longer she spent in these
 four walls the more she felt she needed to be
 free.</p>
 <p>She had spent the last ten years in this room,
 sitting under a poster with an Oscar Wilde quote
 proclaiming that <q>Work is the refuge of
 people who have nothing better to do</q>. Although
 many considered her pioneering work, unraveling
 the secrets of the llama <abbr
 title="Deoxyribonucleic acid">DNA</abbr>, to be an
 outstanding achievement, Molly <em>did</em> think
 she had something better to do.</p>
</body
```

## JavaScript

A script is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
Statements should end with a **semicolon**.

- STATEMENTS ARE INSTRUCTIONS AND
  EACH ONE STARTS ON A NEW LINE
- STATEMENTS CAN BE ORGANIZED
  INTO CODE BLOCKS

Variable is place where you can store values
and they consisting of types like **Boolean, Strings, integer... etc**

```JavaScript
var price;
var quantity;
var total;
price = 5;
quantity = 14;
total = price * quantity;
c02/j s/numeri c-vari ab 1 e .j s
var el = document.getElementByid( ' cost ');
el .textContent = '$' +total;
```

## Decisions and Loops

#### loops

There are also many
occasions where you will
want to perform the same
set of steps repeatedly.

#### DECISIONS

Using the results of
evaluations, you can
decide which path your
script should go down.

#### EVALUATIONS

You can analyze values in
your scripts to determine
whether or note they
match expected results.

```JavaScript
var sum = 0;
var number = 1;
while (number <= 50) {  // -- condition
  sum += number;        // -- body
  number++;             // -- updater
}
alert("Sum = " + sum);  // => Sum = 1275
```
