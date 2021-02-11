# Code 201, 12th Jan, Read-14a

## CSS Transform

It's an alternative ways to size, position, and change elements. 
and all of these can be happen using ```transform``` property.

```css
div {
-webkit-transform: scale(1.5);
-moz-transform: scale(1.5);
-o-transform: scale(1.5);
transform: scale(1.4);
}
```

`transform` property includes multiple vendor prefixes to gain the best support across all browsers.

## 2D  & 3D Transform

2D transform works in x & y axis or as known horizontal and vertical axis, where as 3D transform works in x, y & z axis.

#### 2D example

```css
.box {
transform: rotate(20deg);
}
.box-2{
transform: rotate(-55deg);
}
```

#### 3D example

```css
.box-1{
	transform: prespective(200px) rotate(45deg);
}
.box-2{
	transform: prespective(200px) rotate(45deg);
}
.box-3{
	transform: prespective(200px) rotate(45deg);
}
```

## CSS Transition 
Transition have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.
element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the `:hover`, `:focus`, `:active`, and `:target` pseudo-classes.

#### Transition example
```css
.box{
background: blue;
transition-property: backgournd;
transition-duration: 1s;
transition-timing-function: linear;
}
.box:hover{
background: saddlebrown;
}
```


## CSS Animation
when more control is required, transitions need to have multiple states. This where the animation take a part.

#### Animation example

```css
@keyframe slide{
0% {
	left: 0;
	top: 0;
}

50%{
	left: 244px;
	top: 100px;
}
100%{
	left: 488px
	top: 0;
}
}
```

[My GitHub Page](https://omar-tarawneh.github.io/reading-notes/class-14a)