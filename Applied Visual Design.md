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

