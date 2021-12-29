## Types of Headings:
h1 - Main Headings

h2 - Subheadings
 
h3, h4, h5, h6 - Different levels of subheadings

p - Paragraph

## Syntax:

Comments: 
```HTML
<--! text -->
```


img - element used to add images

alt - attribute for img element incase the image does not load this text is displayed. This also helps increase accessibility to screen readers.

Format:
```HTML
<img src="https://www.freecatphotoapp.com/your-image.jpg" alt="A business cat wearing a necktie.">
```

src - source of an element

Hyperlink:

Anchor element (a)

```HTML
<a href = "link"> text to be hyperlinked </a>
```

Internal Hyperlink:
```HTML
<a href = "#id"> Text to be hyperlinked </a>
```

Open in New Tab: 
```HTML
target="_blank"
```

Dead Link:

```HTML
target="#"
```

Unordered List:
```HTML
<ul> 
  <li> Item 1 </li>
  <li> Item 2 </li> 
</ul> 
```

Ordered List:
```HTML
<ol>
  <li> Item 1</li>
  <li> Item 2</li>
</ol>
```

Input Elements (Text Type):
``` HTML
<input type = "text"> 
```

Placeholder For Input:
```HTML
<input type = "text" placeholder = "This is placeholder text">
```

Submit Input Data:
```HTML
<form action = "/url-where-you-want-to-submit-form-data">
  <input>
</form>
```

Submit Button:
```HTML
<button type = "submit"> this button submits the form </button>
```

**Require Submission**:
```HTML
<input type = "text" required>
```

Radio Buttons:
```HTML
<label for="outdoor">
<input id="outdoor" type="radio" name="indoor-outdoor"> Outdoor
</label>
```

Checkboxes:
```HTML
<label for = "test"><input id="test" type="checkbox" name="test" > Test1 </label>
```

Pre-Checked Checkboxes:
```HTML
<input type = "radio" name = "test-name" checked>
```

**Note:** You can assign a value to an input by typing
```HTML
<input id = "x" value = "assigned value"> 
```

Tell Browser HTML Version:
```HTML
<!DOCTYPE html>

<html>

**CODE**

</html>
```
## Usual Page Layout:
```html
<!DOCTYPE html>
<html>
  <head>
    <meta />
  </head>
  <body>
    <div>
    </div>
  </body>
</html>
```
## Tags:

main - helps search engines find the main page of your site
