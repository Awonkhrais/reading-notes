# **Chapter3 : List**

* We have 3 tybes of lists in HTML :

1. Ordered lists : An ordered list starts with the `<ol>` tag. Each list item starts with the `<li>` tag.The list items will be marked with numbers by default.

2. Unordered lists : An unordered list starts with the `<ul>` tag. Each list item starts with the `<li>` tag.The list items will be marked with bullets (small black circles) by default.

3. Definition lists (Description Lists):A description list is a list of terms, with a description of each term.The `<dl>` tag defines the description list, the `<dt>` tag defines the term (name), and the `<dd>` tag describes each term.

```
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
```
|  Tag  | Description |
|-------|-------------|
|`<ul>` |Defines an unordered list
|`<ol>` |Defines an ordered list
|`<li>` |Defines a list item
|`<dl>` |Defines a description list
|`<dt>` |Defines a term in a description list
|`<dd>` |Describes the term in a description list


**Note:** we can use something called **nested list** >> You can put a second list inside an `<li>` element to create a sublist or nested list.

```
<ul>
  <li>Coffee</li>
  <li>Tea
    <ul>
      <li>Black tea</li>
      <li>Green tea</li>
    </ul>
  </li>
  <li>Milk</li>
</ul>
```
------------------------------------------------------------
# **Chapter 13 : Boxes**

In web development, the CSS box model refers to how HTML elements are modeled in browser engines and how dimension of those HTML elements are derived from CSS properties. It is a fundamental concept for the composition of HTML webpages.

![boxes](https://codinglead.github.io/images/box-model.png)

* By default a box is sized just big enough to hold its contents, To set your own dimensions for a box you can use the `height and width` properties.

**OverFlowing Content**

`overflow`

The overflow property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values:

`hidden` : This property simply hides any extra content that dos not fit in the box.

`scroll` : This property adds a scrollbar to the box so that users can scroll to see the missing content.

![overflow](https://codebridgeplus.com/wp-content/uploads/Csslist2_overflow.png)


## Border, margin & Padding.

Every box has three available properties that can be adjusted to control its appearance: The padding and margin properties are very helpful in adding space between various items on the page.

- Border : Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another.

- Margin : Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.

- Padding : Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents.

![margin&padding](./7.png)

We can adjust on the border these :

 1. border-width.
 2. border-style.
 3. border-color.
 4. border-shorthand :The border property allows you to specify the width, style and color of a border in one property
(and the values should be coded in that specific order).

```
p {
width: 250px;
border: 3px dotted #0088dd;}
```

## Change Inline/Block

`display`

* inline : This causes a block-level element to act like an inline element.

* block : This causes an inline element to act like a block-level element.

* inline-block : This causes a block-level element to flow like an inline element, while retaining other features of a block-level element.

* none : This hides an element from the page. In this case, the element acts as though it is not on the page at all (although a user could still see the content of the box if they used the view source option in their browser).

## Hiding Boxes

`visiblity`

* hidden : This hides the element,If the visibility of an element is set to hidden, a blank space will appear in its place.
* visible : This shows the element.

`border-radius` : CSS3 introduces the ability to create rounded corners on any box, using a property called border-radius. The value indicates the size of the radius in pixels.

`border-radius` : To create more complex shapes, you can specify different distances for the horizontal and the vertical parts of the rounded corners.

------------------------------------------------

# **Chapter 2: Basic JavaScript Instructions**

### **Arrays :** An array is a special type of variable. It doesn't just store one value; it stores a list of values.

* You should consider using an array whenever you are working
with a list or a set of values that are related to each other.

* Arrays are especially helpful when you do not know how
many items a list will contain because, when you create the
array, you do not need to specify how many values it will hold.

------------------------------------------

# **Chapter 4: Decisions and Loops**

## switch statment
A switch statement starts with avariable called the switch value.Each case indicates a possible value for this variable and the code that should run if the variable matches that value.

syntax:

```
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
```

Example:

```
var msg;
var level = 2;
switch (level) {
  case 1:
    msg = "Good Luck on the first test";
    break;
  case 2:
    msg = "Second of three - Keep going!";
    break;
  case 3;
    msg = "Final round, almost there!";
    break;
  default:
    msg = "Good Luck!";
    break;
}
```

* The switch expression is evaluated once. The value of the expression is compared with the values of each case. If there is a match, the associated block of code is executed. If there is no match, the default code block is executed. The break Keyword : When JavaScript reaches a break keyword, it breaks out of the switch block. This will stop the execution of inside the block. It is not necessary to break the last case in a switch block. The block breaks (ends) there anyway.

* The default Keyword : The default keyword specifies the code to run if there is no case match.

