# **Chapter 15 HTML Layout**
We talked about this chapter in [class04](https://awonkhrais.github.io/reading-notes/code201/read04.html) , so here I will add additional information.

![pisition](https://hackernoon.com/drafts/t2w3yae.png)

1. Noraml Flow : `position : static;` In normal flow, each block-level element sits on top of the next one. Since this is the default way in which browsers treat HTML elements, you do not need a CSS property to indicate that elements should appear in normal flow

2. Relative positions : `position : relativ;` Relative positioning moves an element in relation to where it would have been in normal flow. by using the offset properties (top or bottom and left or right).

3. Absolute positionsing : `position:absolute;` When the position property is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements on the page

4. Fixed positiosing : `position:fixed;` Fixed positioning is a type of absolute positioning that requires the position property to have a value of fixed.

5. OverLaping Elements: `z-index;` When you use relative, fixed, or absolute positioning, boxes can overlap. If boxes do overlap, the elements that appear later in the HTML code sit on top of those that are earlier in the page, you can use z-index to control which element sits on top. from (0-10)

6. Floating Elements : `float` The float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible.
--------------------------
## Screen Sizes - Screen resolution - Page sizes

Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens, same to resolution and page sizes, designers often try to create pages of around **960-1000** pixels wide.

To overcome these defferences, there is alot of layouts theat designers use, each one has its own advantages and disadvantages.

1. Fixed width layout.

Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels, for examples :  
 `widht : 970px`



2. Liquid layout.

Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages, for example `width:80%`

------
## CSS Frameworks.

CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch.

--------------------
### Multiple Style Sheets.
 `@import`

 The `@import` rule allows you to import a style sheet into another style sheet.

The `@import` rule must be at the top of the document (but after any @charset declaration).

The `@import` rule also supports media queries, so you can allow the import to be media-dependent.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Multiple Style Sheets - Import</title>
    <link rel="stylesheet" type="text/css" href="css/styles.css" />
  </head>
  <body>
    <!-- HTML page content here -->
  </body>
</html>
```

```css
@import url("tables.css");
@import url("typography.css");
body {
  color: #666666;
  background-color: #f8f8f8;
  text-align: center;
}
#page {
  width: 600px;
  text-align: left;
  margin-left: auto;
  margin-right: auto;
  border: 1px solid #d6d6d6;
  padding: 20px;
}
h3 {
  color: #547ca0;
}
```
note :If a styesheet uses the `@Import` rule, It should appear before the other rules.

### Multiple Style Sheets.
 `<link>`

 ```html
<!DOCTYPE html>
<html>
  <head>
    <title>Multiple Style Sheets - Link</title>
    <link rel="stylesheet" type="text/css" href="css/site.css" />
    <link rel="stylesheet" type="text/css" href="css/tables.css" />
    <link rel="stylesheet" type="text/css" href="css/typography.css" />
  </head>
  <body>
    <!-- HTML page content here -->
  </body>
</html>
```

