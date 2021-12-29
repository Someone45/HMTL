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

