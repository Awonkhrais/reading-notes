# **HTML Text**

![text](https://cdn.educba.com/academy/wp-content/uploads/2019/12/HTML-Text-Formatting-Tags.jpg)

When creating a web page, you add tags (known as markup) to the content of the page. These tags provide exxtra meaning and allow browsers to show users the appropriate structure for the page.

* Structural markup : the elemnts that you can user to describe both headings and paragraphes.

* Semantic markup : which provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it), the meaning of acronyms, and so on

|      Tags      |      Name       |                                                 Usage                                             |
| :------------: | :-------------: | :-----------------------------------------------------------------------------------------------: |
| `<h1> to <h6>` |    Headings     |                 HTML headings are titles or subtitles that you want to display on a webpage.      |
|     `<p>`      |   Paragraphs    | A paragraph always starts on a new line, and browsers automatically add some white space (a margin) before and after a paragraph.
|     `<b>`      |      bold       |                       By enclosing words in the tags `<b>` and `</b>` we can make characters appear bold.                        |
|     `<i>`      |     italic      |                        By enclosing words in the tags `<i>` and `</i>` we can make characters appear italic.                       |
|    `<sup>`     |   superscript   |                   Superscript text appears half a character above the normal line                              |
|    `<sub>`     |    subscript    |                            Subscript text appears half a character below the normal line                            |
|    `<br/>`     |      breaks      |                        inserts a single line break.                                              |
|    `<hr/>`     | horizontal rule |                                          To create a break between themes                                            |
|   `<strong>`   |     strong      |                      defines text with strong importance. The content inside is typically displayed in bold. `<strong>`important`</strong>`                      |
|     `<em>`     |    emphasis     |                   defines emphasized text. The content inside is typically displayed in italic.                   |
| `<blockquote>` |   block qoute   |                      is used for longer quotes that take up an entire paragraph                       |
|     `<q>`      |     quotes      |                        is used for shorter quotes that sit within a paragraph                         |
|    `<abbr>`    |  abbreviation   |                A title attribute on the opening tag is used to specify the full term.                 |
|    `<cite>`    |    citation     |            When you are referencing a piece of work such as a book, film or research paper            |
|    `<dfn>`     |    defining     |                            The first time you explain some new terminology                            |
|  `<address>`   |     address     |                        to contain contact details for the author of the page.                         |
|    `<ins>`     |    inserted     |                        to show content that has been inserted into a document                         |
|    `<del>`     |     delete      |                         can show text that has been deleted from a document.                          |
|     `<s>`      |                 | element indicates something that is no longer accurate or relevant (but that should not be deleted).  |

----------------------------------------------------

# **Introduction CSS**

![css](https://www.freetutorialsplus.com/css-tutorial/images/css-illustration.png)


CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a **selector** and a **declaration**.

```css
p {
  font-family: Arial;
  color: red;
}
```

* p is the selector
* font-family : called the property.
* Arial : called the value.

## You can link HTML to CSS using in two different ways:

**External CSS**

```
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

**Internal CSS**

```
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

## CSS Selctors :
![cssselcrtors](./5.png)

---------------------------------------------------
# **Basic JavaScript Instructions**

A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon.

A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.

## Rules for Naming Variables:

1. the name must begin with a letter, dollar sign (\$) or an underscore(\_), **Not with a number**
2. The name can contain numbers, dollar sign, or an underscore, **But it must not include a dash (-) or a period (.)**
3. You can't use a [reserved](https://www.w3schools.com/js/js_reserved.asp) or keywords in javascript.
4. All vairables are case sensitive.
5. Use a name that describe the kind on information you want to store.
6. use **camelCase** if the vairable is more than one word.

## Arrays
An array is a special type of variable. It doesn’t just store one calue, it stores a list of values.

```js
var colors;
colors = ["red", "black", "blue"];
colors[0]; // this wll gives you the first value of this array 'red'
colors[1] = "yellow"; // this will change the second value form black to yellow
```
**Note:** Values in an array are accessed as if they are in a numberd list, it is important to know that the numering of this list starts from **zero** Not one.

## Operators
![operators](./6.png)

---------------------------------------------

# **Decisions and Loops**

To make decisions we should use conditional statements that included in the JavaScript code assist with decision making, based on certain conditions. The condition specified in the conditional statement can either be true or false. The conditional statements execute the associated piece of code only if the condition is true.

In JavaScript we have the following conditional statements:

* Use if to specify a block of code to be executed, if a specified condition is true.
* Use else to specify a block of code to be executed, if the same condition is false.
* Use else if to specify a new condition to test, if the first condition is false.
* Use switch to specify many alternative blocks of code to be executed.

## Comparison Operators

| Symbol |         Name          |                                   Job                                   |
| :----: | :-------------------: | :---------------------------------------------------------------------: |
|   ==   |      Is Equal To      |             compares two values to see if they are the same             |
|   !=   |    Is Not Equal To    |           compares two values to see if they are not the same           |
|  ===   |    Strict Equal To    |   compares two values and cheack there data type if they are the same   |
|  !==   |  Strict Not Equal To  | compares two values and cheack there data type if they are not the same |
|   >    |      Grater than      |      checks if the number on the left is greater than on the right      |
|   <    |       Less than       |       checks if the number on the left is less than on the right        |
|   >=   | greater than or equal | checks if the number on the left is greater than or equal on the right  |
|   <=   |  less than or equal   |   checks if the number on the left is less than or equal on the right   |

## Logical Operators

![logical](https://i.ytimg.com/vi/JVL6xEzOCrE/maxresdefault.jpg)