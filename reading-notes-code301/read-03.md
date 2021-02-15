# Read-03, 16 Feb 2021, Code 301

## Templating with Mustache

Basically it's technique to render client-side view templates with JavaScript by using a JSON data source.
Mustache is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.
![mustach](https://miro.medium.com/max/700/1*P9q0tkeaRY2l1JOXaVKAig.png)

```{{ name }}``` This is Mustache syntax to show that it is a **placeholder.**
when it render it will replace the Carley brackets with an Actual value like ```Omar```, it will act as objects.

![img](https://miro.medium.com/max/700/1*FRcL9NQHI7Cvi2ELLmzJGQ.png)


## Flex Box

The most beautiful thing that I learned so far, and the most convenient thing to deal with.
so basically we deal with two main things a **container** and the **Boxes** inside it.
what you can add to the container is :
```css
#container{
	/* you need to add this */
	display: flex;
	/* control the direction of the boxes */
	flex-direction: row | row-reverse | column | column-reverse;
	/* how the boxes wrap when the screen get smaller */
	flex-wrap: nowrap | wrap | wrap-reverse;
	/* short hand for the above property */
	flex-flow: column wrap;
	/* control the boxes horizantally */
	justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ...  + safe | unsafe;
	/* control the boxes vertically */
	align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end +  ... safe | unsafe;
	/* control the boxes vertically when there is multi-line-flexible */
	align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end | baseline | first baseline | last baseline +  ... safe | unsafe;  
}
```

* what you can add for the children:
```css
.box {
	/* control the order of the box */
	order: 5;

	/* control the flex box to grow if necessary */
	flex-gorw: 4;

	/* control the flex box to shrink if necessary */
	fles-shrink: 2;
	/*defines the default size of an element before the remaining space is distributed */
	flex-basis: |auto;
	/* shorthand for flex-grow, flex-shrink and flex-basis combined */
	flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
}
	/* align the box vertically */
	align-self: auto | flex-start | flex-end | center | baseline | stretch;  
	
```  

[GitHub Link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code301/read-03)