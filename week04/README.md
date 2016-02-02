# Week 4 - Intro To CSS Positioning & IR
There are multiple ways to position HTML elements using CSS. This week we will go over some of the popular techniques and best practices, in addition to an intro to two effective image replacement techniques.

## Intro to CSS Positioning
### Floats
- Float usage test
- Clear property
- Grid Systems

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
