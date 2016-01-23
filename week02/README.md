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


#### When should you use an ID versus a Class?
**Rule of thumb:** use id's for behavior and classes for styling.

An element can have both an `id` and a `class`, so start with a `class`. If you need something to be unique for a specific behavior (like navigation), add a unique `id` for that page.


## CSS Specificity
- What is specificity?
- Why does it matters?


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
