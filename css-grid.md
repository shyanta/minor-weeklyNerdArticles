# CSS-grid, why every browser should support it

## What is CSS-grid?
CSS-grid is a very new feature in CSS. With grid, you can setup a grid layout for your website, or components inside your website. You can divide your page in multiple columns or rows, like you used to do with tables. Only with grid, you’re more flexible with placing your content in it. You can place the child elements anywhere, they can even overlap each other.

## Why use CSS-grid?
With grid, you can bring the layout of your website to the next level. I can hear you say, “Why not just use flexbox”. Well, of course flexbox is a very nice feature, but preferred on component (or even smaller) level. Yes, you also can make rows and columns with flexbox, but you don’t really are the boss of where the components will take place. You can’t just place it in the middle of the right halve page. Maybe with a lot of detours, but with grid, you can do this with 2 or 3 simple rules of CSS.

Also, with grid you can set a fixed number of rows over your page, something flexbox can’t do. And, with grid, you can make one item start on the third row, and the next item on the first row.

With grid, you can create a playful layout, where we now often use a layout library, like Masonry. Masonry creates a layout where each, for example, image has a different height and width. (see the image below)
![Masonry](/images/masonry.jpg)
<sup>5: masonry.desandro.com</sup>
 
## A quick start: How does CSS-grid work?
To start up the CSS-grid. You `display: grid` the container of the items you want to place in grid layout. With the following lines, you can tell the container how many rows and columns you want.
```CSS
grid-template-columns: 20% 20% 20% 20% 20%;
grid-template-rows: 20% 20% 20% 20% 20%;
```

This makes a layout of five by five. You can place each child inside this container, over this grid of 5x5. Like this:

![Grid layout](/images/gridEmpty.jpg)

Also, you can template some areas, say your header has to take in 5 columns and 2 rows. You can set this to the area ‘header’.
```CSS
grid-template-areas:
    "header header header header header"
    "header header header header header"
    "main main main . sidebar"
    "main main main . sidebar"
    "footer footer footer footer footer";
```
So right now, you have a header that is 5x2. A main that is 3x2, a sidebar that is 1x2 and a footer that is 5x1. This looks like this:
![Grid layout](/images/gridFilled.jpg)

The placement of the children can be done with the following properties.
-   **grid-row-start**<br/>
    Tell the child on what row to start.<br/>
    `grid-row-start: 1;`
-   **grid-column-start**<br/>
    Tell the child on what column to start.<br/>
    `grid-column-start: 1;`
-   **grid-row-end**<br/>
    Tell the child on what row to end.<br/>
    `grid-row-end: 2;`
-   **grid-column-end**<br/>
    Tell the child on what column to end.<br/>
    `grid-column-end: 3;`
-   **grid-row**<br/>
    This is used to tell the child on what row to start and end.<br/>
    `grid-row: <start-line> / <end-line> | <start-line> / span <value>;`
-   **grid-column**<br/>
    This is used to tell the child on what column to start and end.<br/>
    `grid-column: <start-line> / <end-line> | <start-line> / span <value>;`
-   **grid-area**<br/>
    This is used to tell the child what template area to use. In this case this is placed in the sidebar<br/>
    `grid-area: sidebar;`

The placement of the container can be done with the following properties.
-	**grid-auto-columns & grid-auto-rows**<br/>
    This fills the unknown spaces in the grid layout<br/>
    `grid-auto-columns: 60px;`
-	**grid-auto-flow**<br/>
    This tells how to autoplace the items. When set to row, they are initially placed next to each other in a row. And with column, they are placed in a column.<br/>
    `grid-auto-flow: row | column | row dense | column dense`
-   **grid-row-gap & grid-column-gap & grid-gap**<br/>
    With these properties you can tell the container how big the gaps between the columns and rows are supposed to be. You can set this to zero if you want everything to be near each other. And you can set it higher if you want some white space in-between them.<br/>
    `grid-gap: <grid-row-gap> <grid-column-gap>;`

## So, why should this be supported everywhere?
As you can see, grid is just ** awesome. You can do some much with it. It works very nice; your site has a clean and fixed look. The appearance is just amazing.
However, only the newest browsers support it. For now, it’s supported for 65% and with prefixes for 70%. This is a lot, but you should remember that a lot of people still use Internet Explorer. And sadly, the support on IE or Firefox is very bad. You can make your site with grid, but you have to write a completely different piece of code, to make it look just as nice on the other browsers. Because this will take a lot of time, a lot of people don’t think it’s worthy to even try grid. Which is very sad, because it’s such a nice new feature of CSS. I think, if other browsers will support grid better, more people will use it on their website. And that is such a big improvement.<sup>4: caniuse.com</sup>

So, let’s take a vote for it, start a petition or something. We’ve got to fight for grid. Because it’s just so god damn awesome.

## Sources
1.	https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout
2.	https://www.w3.org/TR/css-grid-1/
3.	https://css-tricks.com/snippets/css/complete-guide-grid/
4.	http://caniuse.com/#search=display%3A%20grid
5.	https://masonry.desandro.com/index.html
