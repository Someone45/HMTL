## CSS Grid
Turn any HTML element into a grid container by setting its `display` property to `grid`. This gives you the ability to use all the other properties associated with CSS Grid.

**Note:** In CSS Grid, the parent element is referred to as the container and its children are called items.

```CSS
<style>
.container{
	display: "grid";
}
</style>

<div class = "container">
	<div class = "d1">1</div> 
</div>
```

## Define Grid Element
`grid-template-columns` - Adds columns to the grid 

```CSS
.container{
	display: grid;
	grid-template-columns: 50px 50px;
}
```
^ This will output two columns that are each 50px wide

`grid-template-rows` - Adds rows to the grid

The format is identical to that of `grid-template-columns`

You can use absolute and relative units like `px` and `em` in CSS Grid to define the size of rows and columns. You can use these as well:

`fr`: sets the column or row to a fraction of the available space,

`auto`: sets the column or row to the width or height of its content automatically,

`%`: adjusts the column or row to the percent width of its container.

Here's the code that generates the output in the preview:

```css
grid-template-columns: auto 50px 10% 2fr 1fr;
```

This snippet creates five columns. The first column is as wide as its content, the second column is 50px, the third column is 10% of its container, and for the last two columns; the remaining space is divided into three sections, two are allocated for the fourth column, and one for the fifth.

## Column Gap
To add a gap between the columns, use the `grid-column-gap` property like this:

```css
grid-column-gap: 10px;
```
or
```css
grid-row-gap: 10px;
```
This creates 10px of empty space between all of our columns/rows.

```CSS
grid-gap: rowspx columnpx; 
```

## grid-column to Control Spacing
To control the number of columns an item will consume, you can use the `grid-column` property in conjunction with the line numbers you want the item to start and stop at.

Here's an example:

```css
grid-column: 1 / 3;
```

This will make the item start at the first vertical line of the grid on the left and span to the 3rd line of the grid, consuming two columns.

same applies with `grid-row: 1/3;`
![[Pasted image 20220107230317.png]]

## Align an Item Horizontally using justify-self
In CSS Grid, the content of each item is located in a box which is referred to as a cell. You can align the content's position within its cell horizontally using the `justify-self` property on a grid item. By default, this property has a value of `stretch`, which will make the content fill the whole width of the cell. This CSS Grid property accepts other values as well:

`start`: aligns the content at the left of the cell,

`center`: aligns the content in the center of the cell,

`end`: aligns the content at the right of the cell.

`justify-self: center;`

**`justify-self` is used for horizontral aligning while `align-self` is used for vertical alignment.** 

To do multiple items you use `justify-items` and `align-items`