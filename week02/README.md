# Week 2 - HTML & CSS

## CSS
CSS (Cascading Styles Sheets), is a way to style and present HTML. It is the recommended way to control the presentation layer in a web document. Whereas HTML is what forms the structure of a web page, CSS is what we use to style the HTML with colors, backgrounds, font sizes, layout, and more.

**CSS Syntax:**
```css
selector {
    property: value;
}
```

#### Methods of adding CSS
There are three ways to insert a style sheet:
- External style sheet (Linking to a separate CSS file)
- Internal style sheet (Embedding CSS into the HTML
)
- Inline style (Inline CSS to HTML tags)

**HTML for linking to an external CSS file:**
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title></title>
    <link href="css/style.css" rel="stylesheet" type="text/css">
  </head>
  <body>
  </body>
</html>
```


## IDs vs Classes
**ID**'s are unique
- Each element can have only one ID.
- Each page can have only one element with that ID.

**Classes** are reusable, NOT unique
- You can use the same class on multiple elements.
- You can use multiple classes on the same element.

#### Syntax
**HTML:**
```html
<!-- ID Attribute -->
<div id="content"></div>

<!-- Class Attribute -->
<div class="container"></div>
```

**CSS:**
```css
/* ID Selector */
#content {
  background-color: #ccc;
  padding: 20px;
}

/* Class Selector */
.container {
  max-width: 980px;
  margin: 0 auto;
}
```


#### When should you use an ID versus a Class?
**Rule of thumb:** use id's for behavior and classes for styling.

An element can have both an `id` and a `class`, so start with a `class`. If you need something to be unique for a specific behavior (like navigation), add a unique `id` for that page.


## CSS Specificity
It may not seem like something that important, and in most cases you won’t come across any conflicts at all, but the larger and more complex your CSS files become, or the more CSS files you start to juggle with, the greater likelihood there is of conflicts turning up.

One of the most difficult concepts to grasp in Cascading Stylesheets is CSS Specificity. It is where the browser decide which CSS property values are the most relevant to an element and therefore will be applied. Specificity is based on the matching rules which are composed of CSS selectors of different sorts. If two selectors apply to the same element, the one with higher specificity wins.

**Specificity Rules:**
- If you have written the same rule twice, the latest rule is the one that counts.
  + The last rule defined overrides any previous, conflicting rules.
- ID selectors have a higher specificity than attribute selectors.
- Embedded style sheet is closer to the element to be styled.
- A class selector beats any number of element selectors.

**Measure Specificity:**

| Selector | Specificity |
| -------- | ----------- |
| * { } | 0 |
| li { } | 1 (one element) |
| li:hover { } |	2 (one element, one pseudo-element) |
| ul li { } |	2 (two elements) |
| ul ol li.red { } |	13 (three elements, one class) |
| .sith	| 10 (one class selector) |
| li.red.level { } |	21 (one element, two classes) |
| #sith	| 100 (one id selector) |
| body #darkside .sith p { }	| 112 (HTML selector, id selector, class selector, HTML selector; 1+100+10+1) |
| style=”” |	1000 (one inline styling) |

[CSS Specificity Wars – Cheat Sheet](https://stuffandnonsense.co.uk/archives/images/specificitywars-05v2.jpg)


## Base HTML & CSS
What is the best way to start coding from scratch? What HTML/CSS code do front-end developers commonly repeat across multiple projects?

Start coding with a strong base (simple, semantic markup with initial base CSS styling for core elements such as the typography, headings, lists, links, and all media).

Base [HTML](base/index.html) & [CSS](base/css/style.css)


## Homework:
- Assignment 2 - Post "HTML page with linked CSS file" on your class web page.


### Reference
- [CSS Introduction](http://www.w3schools.com/css/css_intro.asp)
- [CSS Zen Garden](http://www.csszengarden.com/)
- [CSS Properties](http://www.w3schools.com/cssref/)
- [The Difference Between ID and Class](https://css-tricks.com/the-difference-between-id-and-class/)
- CSS Specificity
  + [CSS Specificity: Things You Should Know](https://www.smashingmagazine.com/2007/07/css-specificity-things-you-should-know/)
  + [HTML Dog Specificity](http://www.htmldog.com/guides/css/intermediate/specificity/)
  + [CSS Specificity Wars – Cheat Sheet](https://stuffandnonsense.co.uk/archives/images/specificitywars-05v2.jpg)
- CSS Reset
  + [CSS Tools: Reset CSS](http://meyerweb.com/eric/tools/css/reset/)
  + [normalize.css](https://github.com/necolas/normalize.css/)
