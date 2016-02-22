# Week 6 - Layout with Columns & Image Sprites
This week we'll go over multiple column layouts that can be implemented via CSS using floats. We will also cover CSS rollovers/hover state with image sprites.

[Company Name 1 - Step #4: Columns](http://emmanuelpilande.com/art128/companyname1-step3/)

## Columns
A three column layout would look something like the following:

**html**
```html
<div class="row">
  <div class="column">
     First column
  </div>
  <div class="column">
     Second column
  </div>
  <div class="column">
     Thrid column
  </div>
</div>
```

**css**
```css
.column {
  width: 30%;      /* set column width */
  float: left;     /* float left or right */
  margin: 0 1.5%;  /* set left & right gutter */
}
```

The row class has a clearfix which will clear the floats & bring back it's children elements to normal flow.
Each column is floated left, making them line up horizontally.
They also have a width of 30% & margin left & right of 1.5%.
One column has a total width of 33%.

There are 3 columns, `33% * 3 = 99%` which will fill up the whole row.


## CSS Grid Systems
A grid system is a structure that allows for content to be stacked both vertically and horizontally in a consistent and easily manageable fashion. Additionally, grid system code is project-agnostic giving it a high degree of portability so that it may be adopted on new projects.

- [960 Grid](http://960.gs/)
- [1140 Grid](http://andytaylor.me/2013/04/09/1140px-css-grid-retired/)
- [Responsive Grid System](http://www.responsivegridsystem.com/)
- [Skeleton](http://getskeleton.com/)
- [Pure](http://purecss.io/grids/)
- [Bootstrap](http://getbootstrap.com/css/#grid)
- [Foundation](http://foundation.zurb.com/grid.html)


## Image Sprites
An image sprite is a collection of images put into a single image. A web page with many images can take a long time to load and generates multiple server requests. Using image sprites will reduce the number of server requests, save bandwidth, & help with performance.

## Homework:
- Continue to Step 4 of coding Company Name 1. Be sure to work in a new (separate) folder, such as "companyname1-step4."


### Reference
- [Understanding CSS Grid Systems from the Ground Up](http://www.sitepoint.com/understanding-css-grid-systems/)
- [Don’t Overthink It Grids](https://css-tricks.com/dont-overthink-it-grids/)
- [Responsive Web Design - Grid-View](http://www.w3schools.com/css/css_rwd_grid.asp)
- [CSS Image Sprites](http://www.w3schools.com/css/css_image_sprites.asp)
- [CSS Sprites: What They Are, Why They’re Cool, and How To Use Them](https://css-tricks.com/css-sprites/)
