### Create a Media Query

Media queries are a way to adjust the presentation of text and elements depending on the size of the display ( this is more accurately called the viewport - the user's visible area of a web page) which changes depending on the device accessing the site. 

```HTML
<style>
@media (max-width | max-height : #px) { /* CSS Rules */}
</style>
```

`max` can be replaced with `min` 

### Make an Image Responsive
```CSS
<style> 
img{
	max-width: 100%; height: auto;
}
</style>
```
 
 This will make sure the image does not overextend the viewport
 
 ### Retina Image for Higher Resulution Displays
 ```CSS
<style>
img{
	width: 1/2px; height: 1/2px;
}
</style>
<img src = "image.jpg" alt = "Retina Image"> 
 ```
 Interpret the `1/2px` as half of pixels that the original image contains

### Make Text Responsive
The four different viewport units are:
-   `vw` (viewport width): `10vw` would be 10% of the viewport's width.
-   `vh` (viewport height): `3vh` would be 3% of the viewport's height.
-   `vmin` (viewport minimum): `70vmin` would be 70% of the viewport's smaller dimension (height or width).
-   `vmax` (viewport maximum): `100vmax` would be 100% of the viewport's bigger dimension (height or width).

Example:
```CSS
body { width : 30vw; }
```

### Flex 
Placing the CSS property `display: flex;` on an element allows you to use other flex properties to build a responsive page.

``` HTML
<style>

 body {

 font-family: Arial, sans-serif;

 }

 header {

 display: flex;

 }

 header .profile-thumbnail {

 width: 50px;

 height: 50px;

 border-radius: 4px;

 }

 header .profile-name {

 display: flex;

 margin-left: 10px;

 }

 header .follow-btn {

 display: flex;

 margin: 0 0 0 auto;

 }

 header .follow-btn button {

 border: 0;

 border-radius: 3px;

 padding: 5px;

 }

 header h3, header h4 {

 display: flex;

 margin: 0;

 }

 #inner p {

 margin-bottom: 10px;

 font-size: 20px;

 }

 #inner hr {

 margin: 20px 0;

 border-style: solid;

 opacity: 0.1;

 }

 footer {

 display: flex;

 }

 footer .stats {

 display: flex;

 font-size: 15px;

 }

 footer .stats strong {

 font-size: 18px;

 }

 footer .stats .likes {

 margin-left: 10px;

 }

 footer .cta {

 margin-left: auto;

 }

 footer .cta button {

 border: 0;

 background: transparent;

 }

</style>

<header>

 <img src="https://freecodecamp.s3.amazonaws.com/quincy-twitter-photo.jpg" alt="Quincy Larson's profile picture" class="profile-thumbnail">

 <div class="profile-name">

 <h3>Quincy Larson</h3>

 <h4>@ossia</h4>

 </div>

 <div class="follow-btn">

 <button>Follow</button>

 </div>

</header>

<div id="inner">

<p>I meet so many people who are in search of that one trick that will help them work smart. Even if you work smart, you still have to work hard.</p>

 <span class="date">1:32 PM - 12 Jan 2018</span>

 <hr>

</div>

<footer>

 <div class="stats">

 <div class="Retweets">

 <strong>107</strong> Retweets

 </div>

 <div class="likes">

 <strong>431</strong> Likes

 </div>

 </div>

 <div class="cta">

 <button class="share-btn">Share</button>

 <button class="retweet-btn">Retweet</button>

 <button class="like-btn">Like</button>

 </div>

</footer>
```

![[Pasted image 20211229174234.png]]

Flex helps align elements with one another 

#### Options for Flex:
```CSS
<style> 
#box{
	display: flex;
	flex-direction: row-reverse, column-reverse, column, row (deafult row)
}
</style>
```

There are several options for how to space the flex items along the line that is the main axis. One of the most commonly used is `justify-content: center;`, which aligns all the flex items to the center inside the flex container. Other options include:

-   `flex-start`: aligns items to the start of the flex container. For a row, this pushes the items to the left of the container. For a column, this pushes the items to the top of the container. This is the default alignment if no `justify-content` is specified.
-   `flex-end`: aligns items to the end of the flex container. For a row, this pushes the items to the right of the container. For a column, this pushes the items to the bottom of the container.
-   `space-between`: aligns items to the center of the main axis, with extra space placed between the items. The first and last items are pushed to the very edge of the flex container. For example, in a row the first item is against the left side of the container, the last item is against the right side of the container, then the remaining space is distributed evenly among the other items.
-   `space-around`: similar to `space-between` but the first and last items are not locked to the edges of the container, the space is distributed around all the items with a half space on either end of the flex container.
-   `space-evenly`: Distributes space evenly between the flex items with a full space at either end of the flex container

```CSS
<style>
jsutify-content: center;
</style>
```