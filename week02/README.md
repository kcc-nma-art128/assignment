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
