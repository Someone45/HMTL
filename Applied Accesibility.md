### Text Alternative for Visually Impaired Accessibility
Individuals with visual impairments use screen readers that access the  `alt` attribute of an image to provide the user with information. Always include `alt` text made up of a brief description of the image - this is mandarory for HTML 5.

#### If the image does not need a description or is decorative
```HTML
<img src = "x.jpeg" alt="">
```

## Syntax
The `section` element is also new with HTML5, and has a slightly different semantic meaning than `article`. An `article` is for standalone content, and a `section` is for grouping thematically related content. They can be used within each other, as needed. For example, if a book is the `article`, then each chapter is a `section`. When there's no relationship between groups of content, then use a `div`.

`header` shares the embedded landmark feature you saw with `main`, allowing assistive technologies to quickly navigate to that content. It's used to wrap introductory information or navigation links for its parent tag and works well around content that's repeated at the top on multiple pages.

The `nav` element is another HTML5 item with the embedded landmark feature for easy screen reader navigation. This tag is meant to wrap around the main navigation links in your page.

HTML5 introduced the `figure` element and the related `figcaption`. Used together, these items wrap a visual representation (like an image, diagram, or chart) along with its caption. Wrapping these elements together gives a two-fold accessibility boost by semantically grouping related content and providing a text alternative explaining the `figure`. Example:

```html
<figure>
  <img src="roundhouseDestruction.jpeg" alt="Photo of Camper Cat executing a roundhouse kick">
  <br>
  <figcaption>
    Master Camper Cat demonstrates proper form of a roundhouse kick.
  </figcaption>
</figure>
```

The `label` tag wraps the text for a specific form control item, usually the name or label for a choice. This ties meaning to the item and makes the form more readable. The `for` attribute on a `label` tag explicitly associates that `label` with the form control and is used by screen readers. Example:

```html
<form>
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
</form>
```

### Audio Content
```HTML
<audio id=" " controls>
	<source src = "x.mp3" type = "audio/mpeg">
</audio>
```

### Date Input
```html
 <form>

 <p>Tell us the best date for the competition</p>

 <label for="pickdate">Preferred Date:</label>

 <input type = "date" id = "pickdate" name = "date">

 <input type="submit" name="submit" value="Submit">

 </form>
```
![[Pasted image 20211229154213.png]]

### Standardize Time
```html
<p> Text <time datetime="2013-02-13">last Wednesday</time>, Text.</p>
```

### Make Elements Visible Only To Screen Readers
```css
<style>
.sr-only {
  position: absolute;
  left: -10000px;
  width: 1px;
  height: 1px;
  top: auto;
  overflow: hidden;
}
</style>
```
-   `display: none;` or `visibility: hidden;` hides content for everyone, including screen reader users
-   Zero values for pixel sizes, such as `width: 0px; height: 0px;` removes that element from the flow of your document, meaning screen readers will ignore it

### Keyboard Shortcuts / Acess Keys
HTML offers the `accesskey` attribute to specify a shortcut key to activate or bring focus to an element. Adding an `accesskey` attribute can make navigation more efficient for keyboard-only users.

```html
<button accesskey="b">Important Button</button>
```

`acesskey = " "` is the one thing that matters to create the access key

### Use tabindex to Add Keyboard Focus to an Element
The HTML `tabindex` attribute has three distinct functions relating to an element's keyboard focus. When it's on a tag, it indicates that the element can be focused on. The value (an integer that's positive, negative, or zero) determines the behavior.

```html
<div tabindex="0">I need keyboard focus!</div>
```

A negative `tabindex` value (typically -1) indicates that an element is focusable, but is not reachable by the keyboard. This method is generally used to bring focus to content programmatically (like when a `div` used for a pop-up window is activated)

This essentially brings order to every element that tab will access going from 0 to inf.