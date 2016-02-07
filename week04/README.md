# Week 4 - Intro To CSS Positioning & IR
There are multiple ways to position HTML elements using CSS. This week we will go over some of the popular techniques and best practices, in addition to an intro to two effective image replacement techniques.

[Company Name 1 - Step #2: Image Techniques](http://emmanuelpilande.com/art128/companyname1-step2/)

## Intro to CSS Positioning
### Floats
- Float usage test
  + [All About Floats](https://css-tricks.com/all-about-floats/)
  + The float property specifies whether or not a box (an element) should float

     ```
     float: none|left|right|initial|inherit;
     ```

- Clear property
  + [What does clear both do](http://stackoverflow.com/questions/12871710/what-does-the-css-rule-clear-both-do)
  + The clear property specifies on which sides of an element floating elements are not allowed to float.

     ```
     clear: none|left|right|both|initial|inherit;
     ```

- Grid Systems
  + [Understanding Grid Systems](http://www.sitepoint.com/understanding-css-grid-systems/)
  + [Skeleton](http://getskeleton.com/)
  + [Bootstrap](http://getbootstrap.com/css/)
  + [Foundation](http://foundation.zurb.com/)

##### Containing Floats
```css
.row:before,
.row:after {
  content: "";
  display: table;
}
.row:after {
  clear: both;
}
.row {
  clear: both;
  *zoom: 1;
}
```

### Positioning
- Static
- Relative
- Absolute
- Fixed


## Inserting Images (2 techniques):
**HTML IMG Tag:**

```html
<img src="images/myimage.jpg" alt="My Image">
```

**CSS Background Image:**

```css
background-image:url('images/myimage.jpg');
```

## Image Replacement techniques (2 techniques):
[Image Replacement techniques](https://css-tricks.com/the-image-replacement-museum/)

**Rundle "Phark" Technique (for non-links):**

```css
.phark {
  width: 300px;
  height: 75px;
  background: url('myimage.png');
  text-indent: -9999px;
}
```

**Leahy/Langridge Technique (for links)**:

```css
.leahy {
  width: 300px;
  height: 0;
  padding: 75px 0 0 0;
  background: url('myimage.png');
  overflow: hidden;
}
```


## Homework:
- Continue to Step 2 of coding Company Name 1. Be sure to work in a new (separate) folder, such as "companyname1_step2."


### Reference
- [CSS Layout - float and clear](http://www.w3schools.com/css/css_float.asp)
- [All About Floats](https://css-tricks.com/all-about-floats/)
- [CSS Layout - The position Property](http://www.w3schools.com/css/css_positioning.asp)
- [Image Replacement techniques](https://css-tricks.com/the-image-replacement-museum/)
