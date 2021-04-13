# **Chapter 4 : Links**

Links are the defining feature of the web because they allow you to move from one web page to another.

```
<a href="http://www.imdb.com">IMDB</a>
<!-- Used to Linke ti web pages outside the project -->
<a href="index.html">Home</a>
<!-- Used to Link to another page inside the project -->
```

* ### Email Links

Use `mailto` To create a link that starts up the user's email program and addresses an email to a specified email address, you use the `<a>`element. However, this time the value of the href attribute starts with mailto: and is followed by the email address you want the email to be sent to.

`<a href="mailto:jon@example.org">Email Jon</a>`

 * ### Opening Links in a new window

If you want a link to open in a new window, you can use the target attribute on the opening `<a>` tag. The value of this attribute should be \_blank.

Generally you should avoidopening links in a new window,but if you do, it is considered good practice to inform users
that the link will open a new window before they click on it.

`<a href="http://www.imdb.com" target="_blank"> Internet Movie Database</a>`

--------------------

# **Chapter 15  Layout**

**page 358 to 364**

CSS treats each HTML elemnt as if it is in its own box, This box will either be a **block-level** box or an **inline box**

* Block-level elemtns : `<h1-h6> <p> <ul> <li>`
* Inline-level elements : `<img> <b> <i>`

### Containing Elemtns

if one block-level eemtn sits inside another block-level elemnt then the outer box is known as the **containing** or **parent** element,It is common to group a number of elements together inside a `<div>`(or other block-level) element. For example, you might group together all of the elements that form the header of a site (such as the logo and the main navigation). The `<div>` element that contains this group of elements is then referred to as the containing element.

### ControLLing the position of eLements

CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.

* **Normal flow** : Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. Even if you specify the width of the boxes and there is space for two elements to sit side-by-side, they will not appear next to each other. This is the default behavior (unless you tell the browser to do something else).

* **Relative Positioning** : This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position they would be in in normal flow.

* **Absolute Positioning** : This positions the element
  in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position
  of any surrounding elements (as they simply ignore the space it would have taken up). Absolutely positioned elements move as users scroll up and down the page.

To indicate where a box should be positioned, you may also need to use box offset properties to tell the browser how far from the top or bottom and left or right it should be placed.

* Fixed Positioning : This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element. Elements with fixed positioning do not affect the position of surrounding elements and they do not move when the user scrolls up or down the page.

* Floating elements : Floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box. The floated element becomes a block-level element around which other content can flow.

-----------------------

# **Chapter 3 :Functions, Methods, and Objects**

### Functions

functions let you group a series of statments together to perform a specific task, If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements).

To create a function, you give it a name and then write the statments neede to achieve its task inside the curly braces.
This is known as a **_function declaration_**

```
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
name();
```

### variable scope

The location where you declare a varable will affect where it can be used within you code, if you declare it within a function, it can only be used within that function. This is known as the variable's scope.

In JavaScript there are two types of scope:

1. Local scope :

Variables declared within a JavaScript function, become **LOCAL** to the function.

Local variables have **Function scope:** They can only be accessed from within the function.

2. Global scope :

A variable declared outside a function, becomes **GLOBAL**.

A global variable has **global scope:** All scripts and functions on a web page can access it.


* JavaScript has function scope: Each function creates a new scope.

* Scope determines the accessibility (visibility) of these variables.

* Variables defined inside a function are not accessible (visible) from outside the function.

------------
# **The article : Pair Programming**

![pair](https://images.prismic.io/impactio-blog/06eab7d7-e9ef-4ae3-b93b-8bcc47372fb3_Pair++programming.png?auto=compress,format)

Pair Programming :technique in which two programmers work together at one workstation. One, the driver, writes code while the other, the observer or navigator, reviews each line of code as it is typed in. The two programmers switch roles frequently.

pair programming can effect in a good way :

* Greater efficiency

* Engaged collaboration

* Learning from fellow students

* Social skills

* Job interview readiness

* Work environment readiness

