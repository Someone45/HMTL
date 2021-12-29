### Bold Text
To make text bold, you can use the `strong` tag. This is often used to draw attention to text and symbolize that it is important. With the `strong` tag, the browser applies the CSS of `font-weight: bold;` to the element.

```HTML
<strong> Text </strong>
```

### Underline Text
To underline text, you can use the `u` tag. This is often used to signify that a section of text is important, or something to remember. With the `u` tag, the browser applies the CSS of `text-decoration: underline;` to the element.

```HTML
<u> Text </u>
```

### Italicize Text
To emphasize text, you can use the `em` tag. This displays text as italicized, as the browser applies the CSS of `font-style: italic;` to the element.

```HTML
<em> Text </em>
```

### Strikethrough Text

To strikethrough text, which is when a horizontal line cuts across the characters, you can use the `s` tag. It shows that a section of text is no longer valid. With the `s` tag, the browser applies the CSS of `text-decoration: line-through;` to the element.

```HTML
<s>Text </s>
```

### Horizontal Lines
You can use the `hr` tag to add a horizontal line across the width of its containing element. This can be used to define a change in topic or to visually separate groups of content.
```HTML
<hr>
```

### Box Shadow
The `box-shadow` property applies one or more shadows to an element.

The `box-shadow` property takes values for

-   `offset-x` (how far to push the shadow horizontally from the element),
-   `offset-y` (how far to push the shadow vertically from the element),
-   `blur-radius`,
-   `spread-radius` and
-   `color`, in that order.

The `blur-radius` and `spread-radius` values are optional.

Multiple box-shadows can be created by using commas to separate properties of each `box-shadow` element.

```css
box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0 6px 6px rgba(0,0,0,0.23);
```

### Opacity
```HTML
<style>
	opacity: 0-1
</style>
```

### Text Transform
```HTML
<style>
	h4{
		text-transform: lowercase;
	}
</style>
```
### Text Size
---

In the `style` tags, set the `font-size` of the:

-   `h1` tag to 68px.
-   `h2` tag to 52px.
-   `h3` tag to 40px.
-   `h4` tag to 32px.
-   `h5` tag to 21px.
-   `h6` tag to 14px.

<hr> 

### Font Weight:
You set the `font-size` of each heading tag in the last challenge, here you'll adjust the `font-weight`.

The `font-weight` property sets how thick or thin characters are in a section of text.

```HTML
<style>
	p{
	font-weight: x;
	}
</style>
```

### Line Height / Paragraph Spacing
```HTML
<style>
	p{
	line-height: #px;
	}
</style>
```

### Hover State
For example, the styling of an anchor tag can be changed for its hover state using the `:hover` pseudo-class selector. Here's the CSS to change the `color` of the anchor tag to red during its hover state:

```CSS
<style>

 a {

 color: #000;

 }

a:hover{

 color: blue;

}

</style>
```

### Relative Position
Used to move items while maintaining the same position for all other items
```CSS
<style>

 h2 {

position: relative;

top: 15px;

 }

</style>
```
You can use:
`top`, `bottom`, `right`, `left`
These move the item to the opposite side

### Lock an Element / Absolute Positioning
```HTML
<style>
 #searchbar {
 position: absolute;
 top: 50px;
 right: 50px;
 }
</style>
```
Locks the element in place relative to its parent container.

### Fixed Position
A type of absolute positioning that locks an element relative to the browser window. One key difference between the `fixed` and `absolute` positions is that an element with a fixed position won't move when the user scrolls.

```HTML
<style>
 #searchbar {
 position: fixed;
 top: 50px;
 right: 50px;
 }
</style>
```

### Push Elements Left or Right with the float Property
Floating elements are removed from the normal flow of a document and pushed to either the `left` or `right` of their containing parent element.

## Overlapping Elements
Use the `z-index` to change the order of elements that overlap each other after positioning them using `position: absolute | relative | fixed | sticky`. 

```HTML
<style>
	#box{
		z-index: #;
	}
</style>
```

### Center Element / Margin
Another positioning technique is to center a block element horizontally. One way to do this is to set its `margin` to a value of auto.

`margin: auto`

### Hue of a Color
`hsl(hue, saturation, lightness)`

**Hue** is what people generally think of as 'color'. If you picture a spectrum of colors starting with red on the left, moving through green in the middle, and blue on right, the hue is where a color fits along this line. In `hsl()`, hue uses a color wheel concept instead of the spectrum, where the angle of the color on the circle is given as a value between 0 and 360.

**Saturation** is the amount of gray in a color. A fully saturated color has no gray in it, and a minimally saturated color is almost completely gray. This is given as a percentage with 100% being fully saturated.

**Lightness** is the amount of white or black in a color. A percentage is given ranging from 0% (black) to 100% (white), where 50% is the normal color.
 

### Linear Gradient
```css
background: linear-gradient(gradient_direction, color 1, color 2, color 3, ...);
```

The first argument specifies the direction from which color transition starts - it can be stated as a degree, where `90deg` makes a horizontal gradient (from left to right) and `45deg` makes a diagonal gradient (from bottom left to top right).  The following arguments specify the order of colors used in the gradient.

```CSS
background: linear-gradient(35deg, #CCFFFF, #FFCCCC)
```

#### Repeated Linear Gradient:
```CSS
 background: repeating-linear-gradient(

 90deg,

 yellow 0px,

 blue 40px,

 green 40px,

 red 80px

 );
```

### Custom Background
```CSS
<style>

 body {

 background: url(image-link)

 }

</style>
```

### Transform to Change Element Size
```css
p {
  transform: scale(2);
}
```

This doubles the size of all paragraph elements

### Scale Elements on Mouse Hover
Simply set the CSS modification as :hover
```css
p:hover {
  transform: scale(2.1);
}
```

### Skew Elements
Along X-Axis:
```css
p {
  transform: skewX(-32deg);
}
```

Along Y-Axis:
```css
p {
  transform: skewY(-32deg);
}
```

### Create a Graphic Using CSS

`box-shadow` property takes values for `offset-x`, `offset-y`, `blur-radius`, `spread-radius` and a color value in that order. The values for `blur-radius` and `spread-radius are optional`

Crescent Moon:

```CSS
<style>
 .center {
 position: absolute;
 margin: auto;
 top: 0;
 right: 0;
 bottom: 0;
 left: 0;
 width: 100px;
 height: 100px;
 background-color: transparent;
 border-radius: 50%;
 box-shadow: 25px 10px 0 0 blue;
 }
</style>
<div class="center"></div>
```

### More Complex Shape Using CSS & HTML
`::before` creates a pseudo-element that is the first child of the selected element; `::after` creates a pseudo-element that is the last child of the selected element.

For the `::before` and `::after` pseudo-elements to function properly, they must have a defined `content` property. This property is usually used to add things like a photo or text to the selected element. When the `::before` and `::after` pseudo-elements are used to make shapes, the `content` property is still required, but it's set to an empty string.

HEART CSS:
```CSS
<style>

 .heart {

 position: absolute;

 margin: auto;

 top: 0;

 right: 0;

 bottom: 0;

 left: 0;

 background-color: pink;

 height: 50px;

 width: 50px;

 transform: ;

 }

 .heart::after {

 background-color: blue;

 content: "";

 border-radius: 25%;

 position: absolute;

 width: 50px;

 height: 50px;

 top: 0px;

 left: 25px;

 }

 .heart::before {

 content: ;

 background-color: pink;

 border-radius: 50%;

 position: absolute;

 width: 50px;

 height: 50px;

 top: -25px;

 left: 0px;

 }

</style>

<div class="heart"></div>
```

### Animation and Keyframes
`animation-name` sets the name of the animation, which is later used by `@keyframes` to tell CSS which rules go with which animations.
`animation-duration` sets the length of time for the animation.

### Modify Fill Mode of an Animation
Notice how the animation resets after `500ms` has passed, causing the button to revert back to the original color. You want the button to stay highlighted.

This can be done by setting the `animation-fill-mode` property to `forwards`. The `animation-fill-mode` specifies the style applied to an element when the animation has finished.
```css
animation-fill-mode: forwards;
```

### Animate Movement in CSS
Moving Colorful Bar:
```CSS
<style>

 div {

 height: 40px;

 width: 70%;

 background: black;

 margin: 50px auto;

 border-radius: 5px;

 position: relative;

 }

 #rect {

 animation-name: rainbow;

 animation-duration: 4s;

 }

 @keyframes rainbow {

 0% {

 background-color: blue;

 top: 0px;

 }

 50% {

 background-color: green;

 top: 50px;

 }

 100% {

 background-color: yellow;

 top: 0px;

 }

 }

</style>

<div id="rect"></div>
```

### Choose Number of Iterations to Animate
```css
animation-iteration-count: 3;
```
Example Usage:
```CSS
animation-name: backdiv;

animation-duration: 1s;

animation-iteration-count: infinite;
```

### Animate at Different Rates
To change the animation rate of an object, change it's `@keyframe` rule bya %

Alternative:

Manipulate the elements `animation-duration` to speed up or slow down the rate of animation.

### Change Animation Timing with Keywords

In CSS animations, the `animation-timing-function` property controls how quickly an animated element changes over the duration of the animation. If the animation is a car moving from point A to point B in a given time (your `animation-duration`), the `animation-timing-function` says how the car accelerates and decelerates over the course of the drive.

There are a number of predefined keywords available for popular options. For example, the default value is `ease`, which starts slow, speeds up in the middle, and then slows down again in the end. Other options include `ease-out`, which is quick in the beginning then slows down, `ease-in`, which is slow in the beginning, then speeds up at the end, or `linear`, which applies a constant animation speed throughout.

### Bezier Curves
In CSS animations, Bezier curves are used with the `cubic-bezier` function. The shape of the curve represents how the animation plays out. The curve lives on a 1 by 1 coordinate system. The X-axis of this coordinate system is the duration of the animation (think of it as a time scale), and the Y-axis is the change in the animation.

The `cubic-bezier` function consists of four main points that sit on this 1 by 1 grid: `p0`, `p1`, `p2`, and `p3`. `p0` and `p3` are set for you - they are the beginning and end points which are always located respectively at the origin (0, 0) and (1, 1). You set the x and y values for the other two points, and where you place them in the grid dictates the shape of the curve for the animation to follow. This is done in CSS by declaring the x and y values of the `p1` and `p2` "anchor" points in the form: `(x1, y1, x2, y2)`.

```css
animation-timing-function: cubic-bezier(0.25, 0.25, 0.75, 0.75);
```