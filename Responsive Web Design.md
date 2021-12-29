## Syntax:

Color of Text:

```HTML
<h2 style = "color: colorname;"> Text </h2>
```

### Use a Rule For All Blocks:

```html
<style>
  h2 {
    color: red;
  }
</style>
<h2> Text Here </h2>
```
All of the text under h2 changes the color to red

### Use Classes For Styling
```html
<style>
  .blue-text {
    color: blue;
  }
</style>
```
 Then you can reuse the class as
 ```HTML
<h2 class = "blue-text"> Text </h2>
 ```

### Font Size:
```HTML
<style>
	h1{
		font-size: sizepx;
	}
</style>
```
Changed the font size of all elements specified

### Font Type
```HTML
<style>
	h2{
		font-family: sans-serif;
	}
</style>
```

### Import Google Font
```HTML
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
```
Replace *"https://fonts.googleapis.com/css?family=Lobster"* with URL for font to be exported

You can then use it as 

```css
font-family: FAMILY_NAME, GENERIC_NAME;
```
Quotation marks are needed for FAMILY_NAME if there is a space

### Degrade Fonts
```css
p {
  font-family: Helvetica, sans-serif;
}
```
Here the font will be degraded to sans-serif if Helvetica is not available

### Size Images (Using a Class)
```html
<style>
  .larger-image {
    width: 500px;
  }
</style>
```

### Borders Around Elements
```html
<style>
  .thin-red-border {
    border-color: red;
    border-width: 5px;
    border-style: solid;
  }
</style>
```

### Use Multiple Classes
```html
<img class="class1 class2">
```


### IDs for Elements
```html
<h2 id="cat-photo-app">
```

### Use ID To Style
```css
#cat-photo-element {
  background-color: green;
}
```

### Padding:
CSS allows you to control the `padding` of all four individual sides of an element with the `padding-top`, `padding-right`, `padding-bottom`, and `padding-left` properties.

Instead of specifying an element's `padding-top`, `padding-right`, `padding-bottom`, and `padding-left` properties individually, you can specify them all in one line, like this:

```css
padding: 10px 20px 10px 20px;
```


### Margin:
CSS allows you to control the `margin` of all four individual sides of an element with the `margin-top`, `margin-right`, `margin-bottom`, and `margin-left` properties.

Instead of specifying an element's `margin-top`, `margin-right`, `margin-bottom`, and `margin-left` properties individually, you can specify them all in one line, like this:

```css
margin: 10px 20px 10px 20px;
```

### Style Elements
```css
[type='radio'] {
  margin: 20px 0px 20px 0px;
}
```

### Relative Units/Measurements
The two main types of length units are absolute and relative. Absolute units tie to physical units of length. For example, `in` and `mm` refer to inches and millimeters, respectively. Absolute length units approximate the actual measurement on a screen, but there are some differences depending on a screen's resolution.

Relative units, such as `em` or `rem`, are relative to another length value. For example, `em` is based on the size of an element's font. If you use it to set the `font-size` property itself, it's relative to the parent's `font-size`.

