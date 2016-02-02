# Week 3 - Box Model & Block Elements

## Company Name #1
This week we will begin Site #1 Company Name 1 by breaking down the common web page into specific sections commonly used for layout, introducing HTML5 tags, and more.

What we will be building: [Company Name 1 - Step #1: Basic setup](http://emmanuelpilande.com/art128/companyname1-step1/)

#### Assets:
- [Company Name 1 - Site Map & Wireframes](assets/CompanyName1-sitemap-wireframes.pdf)
- [Company Name 1 - Layout & Code Notes](assets/CompanyName1-notes.pdf)
- [Company Name 1 - Home Page Design](assets/CompanyName1-Design-home.jpg)
- [Company Name 1 - About Sub Page Design](assets/CompanyName1-Design-about.jpg)
- [Company Name 1 - Source Design File](assets/CompanyName1_Design.psd)


#### Set up HTML

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title></title>

    <!-- VIEWPORT FOR MOBILE -->
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <!-- MAIN CSS -->
    <link rel="stylesheet" href="css/style.css">
  </head>
  <body>
    <div class="container">
      <h1></h1>
      <h2></h2>
      <h3></h3>
      <h4></h4>
      <h5></h5>
      <h6></h6>
      <p></p>
      <ul>
        <li></li>
      </ul>
      <ol>
        <li></li>
      </ol>
      <a href="#"></a>
    </div>
  </body>
</html>
```

##### HTML5 Shiv
Google Shim (aka Shiv) - HTML5 backward compatibility support:

```html
<!--[if lt IE 9]>
    <script src="http://html5shim.googlecode.com/svn/trunk/html5.js"></script>
<![endif]-->
```


#### Set up CSS
**Base CSS for starting a site:**

```css
/* CSS TABLE OF CONTENTS
=====================================
	#BASE CSS
	#SITE-SPECIFIC CSS
===================================== */

/* BASE (Initital Setup)
=====================================
	#RESET
	#HTML5
	#BASE TYPOGRAPHY
		#BODY
		#HEADINGS
		#PARAGRAPHS
		#LINKS
		#LISTS
	#IMAGES
	#CLEARFIX
===================================== */

/* SITE SPECIFIC (Custom CSS for The Client Site)
=====================================
	#SITE-SPECIFIC GENERAL STYLING
	#SITE-SPECIFIC TYPOGRAPHY
	#LAYOUT/GRID
	#SECTIONS
	#MEDIA QUERIES
	#@FONT-FACE
===================================== */
```

**Media Queries:**

```css
/* MEDIA QUERIES
===================================== */
/* Tablet */
@media only screen and (min-width: 48em) and (max-width: 62em) {

}

/* MOBILE */
@media only screen and (max-width: 47.9999em) {

}
```


## Div's
`<div>` is short for "division", allows you to divide your page. It is used to group elements for styling purposes giving you more control over the structure, space, width, layout, etc.

- Div usage tests
  + Normal Flow
  + Multiple Classes
  + CSS positioning
  + Grouping & nesting


## Box Model
All HTML elements can be considered as boxes. In CSS, the term "box model" is used when talking about design and layout. The CSS box model is essentially a box that wraps around every HTML element. It consists of: content, padding, borders, & margin.

**Every element on a page is a rectangular box.**

![Box Model](https://i.imgur.com/aetBH1x.png)

- 4 shells
  + Content - The content of the element
  + Padding - Space inside the element & around the content
  + Border - Between padding & margin
  + Margin - Space outside the element

What is the total width of the element below:
```css
div {
  width: 400px;
  height: 100px;
  margin: 0 20px;
  padding: 20px;
  border: 4px solid #333;
}
```

## Display Block vs Inline
- block — Form boxes according to the css box-model. They have width, height, padding, border, and margin and they stack vertically on top of each other.
- inline — don’t form boxes. They sit horizontally next to each other.
- inline-block — Behaves like block elements on the inside where they form boxes. On the outside they act like inline elements sitting horizontally next to each other instead of stacking on top of each other.



## Responsive Images
Allow images to scale up & down, but never scale larger than it's original size. This will make the image responsive & fit the parent div/container.
```css
img {
  max-width: 100%;
  height: auto;
}
```


## Homework:
- Starting with a solid base HTML and CSS setup, begin coding Company Name Site #1 by dividing the page into major sections using semantic HTML5 tags to designate different sections of the site. Then add a small amount of content and use CSS to control the presentation of all sections and content, such as background color, margin, and padding. Work from the "outside in" and "top down."


### Reference
- [HTML5 Elements](http://www.w3schools.com/html/html5_new_elements.asp)
- [HTML5 Shiv](https://github.com/aFarkas/html5shiv)
  + [w3schools - HTML5 browsers](http://www.w3schools.com/html/html5_browsers.asp)
- [Why Ems](https://css-tricks.com/why-ems/)
- [Box Model](https://css-tricks.com/the-css-box-model/)
- [Explain div tag to non-programmer](http://stackoverflow.com/a/14027798/3567750)
