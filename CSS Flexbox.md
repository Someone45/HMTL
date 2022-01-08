## Align Elements 
The different values available for `align-items` include:
-   `flex-start`: aligns items to the start of the flex container. For rows, this aligns items to the top of the container. For columns, this aligns items to the left of the container.
-   `flex-end`: aligns items to the end of the flex container. For rows, this aligns items to the bottom of the container. For columns, this aligns items to the right of the container.
-   `center`: align items to the center. For rows, this vertically aligns items (equal space above and below the items). For columns, this horizontally aligns them (equal space to the left and right of the items).
-   `stretch`: stretch the items to fill the flex container. For example, rows items are stretched to fill the flex container top-to-bottom. This is the default value if no `align-items` value is specified.
-   `baseline`: align items to their baselines. Baseline is a text concept, think of it as the line that the letters sit on.

```CSS
<style> 
p{
align-items: center;
}
</style>
```

**This can also be used to align flex compontents**


## Flex-Wrap
However, using the `flex-wrap` property tells CSS to wrap items. This means extra items move into a new row or column. The break point of where the wrapping happens depends on the size of the items and the size of the container.

CSS also has options for the direction of the wrap:

-   `nowrap`: this is the default setting, and does not wrap items.
-   `wrap`: wraps items onto multiple lines from top-to-bottom if they are in rows and left-to-right if they are in columns.
-   `wrap-reverse`: wraps items onto multiple lines from bottom-to-top if they are in rows and right-to-left if they are in columns.

```CSS
<style>

 #box-container {

 background: gray;

 display: flex;

 height: 100%;

 flex-wrap: wrap;
}

</style>
```

## Flex-Shrink
```CSS
<style>
#item{
flex-shrink: #;
}
</style>
```
Controls the size of items as the container shrinks

## Flex-Grow
```CSS
<style>
#item{
flex-grow: #;
}
</style>
```

Opposite of `flex-shrink`, controls the size of the items as the container expands

## Flex for Initial Size of an Item
```CSS
<style>
#item{
flex-basis: 10px;
}

</style>
```

## Shortcut Flex Property
 The default property settings are `flex: 0 1 auto;`
 
 `flex: flex-grow flex-shrink flex-basis;`
 
 You can use this to assign values without having to insert a lot 
 
 ## Rearrange Items
 ```CSS
 <style> 
#box1{
order: #;
}
</style>
 ```
 
 The `order` property is used to tell CSS the order of how flex items appear in the flex container. By default, items will appear in the same order they come in the source HTML. The property takes numbers as values, and negative numbers can be used.
 
 ## align-self Property
 This is useful since other common adjustment techniques using the CSS properties `float`, `clear`, and `vertical-align` do not work on flex items.
 
 `align-self` accepts the same values as `align-items` and will override any value set by the `align-items` property.
 
 ```CSS
<style>
#box1{
align-self: center;
}
</style>
 ```
 
**Center can be replaced with any other setting**

