# Code 201, 30th Dec, Read-05

## Html Images, Color and text

### Images

Images are very important to beautify as well as to depict many complex concepts in simple way on your web page. This tutorial will take you through simple steps to use images in your web pages.

```html
<img src="Image URL" ... attributes-list />
```

**Images** have also the _alt_ attribute and _title_ attribute to provide more information about them.

```Html
<!DOCTYPE html>
<html>
<head>
<title>Using Image in Webpage</title>
</head>
<body>
<p>Simple Image Insert</p>
<img  src="/html/images/test.png"  alt="Test Image"  />
</body>
</html>
```

### Colors

you can add color by three different way:

- RGB Value
- Hex Code
- Color Name

```CSS
body {
background-color: rgb(200,200,200);
}
h1 {
background-color: DarkCyan;
}
h2 {
background-color: #ee3e80;
}
p {
background-color: white;
}
```

we also learn about the color wheel using adobe that will help you to choose the right colors to make your website more beautiful.
There also new concept called **opacity**:
is like adding a shadow to your color

```css
p.one {
  background-color: rgb(0, 0, 0);
  opacity: 0.5;
}
p.two {
  background-color: rgb(0, 0, 0);
  background-color: rgba(0, 0, 0, 0.5);
}
```

There also another one used in **CSS3** called _**hsl**_/_**hsla**_
accept tree values:

- Hue
- Saturation
- Lightness
  and for _**hsla**_ accept also the opacity value

### Text

For text there are many styles you can do I actually use _**Google Font**_ that help me to choose one of the styles that suite my web site.
**Typeface Terminology**:

- Serif
- Sans-Serif
- Monospace
- Weight
- Style
- Stretch

```css
p {
  width: 600px;
  margin: 0 auto;
  font-family: "Helvetica Neue", "Arial", sans-serif;
  font-style: italic;
  font-weight: 100;
  font-variant-ligatures: normal;
  font-size: 2rem;
  letter-spacing: 1px;
}
```

Reference: [Html & CSS](https://wtf.tw/ref/duckett.pdf)
