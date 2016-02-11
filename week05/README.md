# Week 5 - Unordered Lists For Navigation
Unordered lists are a semantic way of marking up navigational links for web sites. This week we will learn how to stylize unordered lists using CSS to look like common navigational elements such as top and footer navs.

[Company Name 1 - Step #3: Navigation w/ Lists](http://emmanuelpilande.com/art128/companyname1-step3/)

## Web Fonts with @font-face
`@font-face` allows custom fonts to be loaded on a webpage if the user hasn't got that font installed. This enables web designers to use hundreds and thousands of different fonts and are not restricted to be "web-safe" fonts that the user has pre-installed on their computer.

**Hosted Font Services:**
- [font-face](http://www.font-face.com/)
- [Font Squirrel](http://www.fontsquirrel.com/)
- [Adobe Typekit](https://typekit.com/)
- [Google Fonts](https://www.google.com/fonts)

```css
@font-face {
  font-family: 'FontName';
  src: url('fontname.eot'); /* IE9 Compat Modes */
  src: url('fontname.eot?#iefix') format('embedded-opentype'), /* IE6-IE8 */
       url('fontname.woff2') format('woff2'), /* Super Modern Browsers */
       url('fontname.woff') format('woff'), /* Pretty Modern Browsers */
       url('fontname.ttf')  format('truetype'), /* Safari, Android, iOS */
       url('fontname.svg#svgFontName') format('svg'); /* Legacy iOS */
}
```

```css
body {
  font-family: 'FontName', Fallback, sans-serif;
}
```


## How to stylize lists for navigation
Company Name 1 three different navigation systems:
- Header utility navigation.
- Horizontal top navigation.
- Footer navigation.

**Using lists for navigation:**
- Use unordered lists.
- Control the list-style type (set to "none" to remove the default bullet points).
- Control the position of the list items via floats or displaying them "inline" or "inline-block".
- Control the visual formatting using margin, padding, and borders.
- Use a:hover for rollovers.
- For further control:
  + Use classes or css selectors, such as “:first-child” or “:last-child” to target specific list items

#### Two ways to create a horizontal navigation bar.

**Floating:**
```css
ul {
  margin: 0;
  padding: 0;
  list-style: none;
  background-color: #333;
  overflow: hidden;
}

li {
  float: left;
}

li a {
  display: block;
  padding: 10px 12px;
  text-align: center;
  color: white;
}
```

**Inline:**
```css
ul {
  margin: 0;
  padding: 0;
  list-style: none;
  background-color: #333;
}

li {
  display: inline-block;
}

li a {
  display: block;
  padding: 10px 12px;
  text-align: center;
  color: white;
}
```


## Homework:
- Continue to Step 3 of coding Company Name 1. Be sure to work in a new (separate) folder, such as "companyname1-step3."


### Reference
- [Can I Use](http://caniuse.com/)
- [CSS Font Stack](http://www.cssfontstack.com/)
- [CSS3 @font-face Rule](http://www.w3schools.com/cssref/css3_pr_font-face_rule.asp)
- [Using @font-face](https://css-tricks.com/snippets/css/using-font-face/)
- [Comprehensive Guide: When to Use Em vs. Rem](http://webdesign.tutsplus.com/tutorials/comprehensive-guide-when-to-use-em-vs-rem--cms-23984)
- [Chunk Five](http://www.fontsquirrel.com/fonts/ChunkFive)
