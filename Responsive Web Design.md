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