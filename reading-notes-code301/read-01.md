# Read-01, 12 Feb 2021, Code 301

## SMACSS and Responsive Web Design 

### RWD

Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.
We are going to learn how to make website suitable for all devices **Desktop**, **Mobile Phone** and all screen sizes.

Responsive web design is broken down into three main types:
* Flexible layouts
* Media Queries
* Flexible Media

#### Flexible Layout

is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.

**Relative Viewport Lengths**
CSS Relative length units
* vw: Viewports Width
* vh: Viewports Height
* vmin: Minimum of the viewport's height and width.
* vmax: Maximum of the viewport's height and width.

**formula to help identify the proportions of a flexible layout using relative values.**
```
target / context = result
```
code example:
```html
<div class="container">
  <section>...</section>
  <aside>...</aside>
</div>
```
```css
section,
aside {
  background: #2db34a;
  color: #fff;
  margin: 1.858736059%;
  padding: 20px 0;
  text-align: center;
}
section {
  float: left;
  width: 63.197026%;
}
aside {
  float: right;
  width: 29.3680297%;
}
```
#### Media Queries

Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example.

```css
/* @media Rule */
@media only screen and (max-width: 600px) {  
body  {  
background-color:  lightblue;  
}  
}
/* @import Rule */
@import url(styles.css) all and (max-width: 1024px) {...}
```
logical operator for media query are **and, not** and **only**.

#### Flexible Media

The ability to make the images, videos and other media type scalable.
```css
img, video, canvas{
max-width: 100%;
}
```

## Float

Float is a CSS positioning property.

![float](https://i1.wp.com/css-tricks.com/wp-content/csstricks-uploads/print-layout.png?resize=540%2C270&ssl=1)

```css
div {
	float: right;
}
```
There are four valid values:
* Left
* Right
* None (default)
* Inherit: take the value from the parent element.

we mostly used ``` clear``` property with ```float``` to control the layout of our site


## SMACSS

Scalable and Modular Architecture for CSS
**SMACSS** is more like a style guide for your project, SMACSS is a way to examine your design process and as a way to fit those rigid frameworks into a flexible thought process.

**SMACSS** is to keep CSS more organized and more structured, leading to code that is easier to build and easier to maintain.

