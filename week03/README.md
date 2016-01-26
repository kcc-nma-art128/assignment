# Week 3 - Box Model & Block Elements

## Company Name #1
This week we will begin Site #1 Company Name 1 by breaking down the common web page into specific sections commonly used for layout, introducing HTML5 tags, and more.

#### Assets:
- [Company Name 1 - Site Map & Wireframes](assets/CompanyName1-sitemap-wireframes.pdf)
- [Company Name 1 - Layout & Code Notes](assets/CompanyName1-notes.pdf)
- [Company Name 1 - Home Page Design](assets/CompanyName1-Design-home.jpg)
- [Company Name 1 - About Sub Page Design](assets/CompanyName1-Design-about.jpg)
- [Company Name 1 - Source Design File](assets/CompanyName1-Design.psd)


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


