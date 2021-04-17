# **Chapter 3 : Objects**

Objects group together a set of variables and function to create a model of a something you would recognize from the real world,

IN AN OBJECTS VARIABLES BECOMES KNOWN AS PROPERTIES properties tell us about the object,such as the name of a hotel or the number of rooms it has.

IN AN OBJECTS FUNCTIONS BECOMES KNOWN AS METHODS methods represent tasks that are associated with the object.

```js
var hotel = {
  name: "Quay",
  rooms: 40,
  booked: 25,
  gym: true,
  roomTypes: ["twin", "double", "suite"],
  checkAvailability: function () {
    return this.rooms - this.booked;
  }
};
// This is How to accessing an object, properities and methods.
var hotelName = hotel.name;
// This will gives us hotelName = Quay;
var roomesFree = hotel.checkAvalibilty();
// This will execute the function inside the object hotel.
// Another way to access an Object (JUST ITS PROPERTIES).
var hotelRooms = hotel["rooms"];
```

The code above, you can see name,rooms,booked,gtm, and roomTypes : all of these are called properties which have KEY and VALUE for each one. checkAvailability(); called a method.

You accessing an Object by using what we call a DOT NOTATION It is shown above in the comments.

# **Chapter 5: Document Object Model**

![Dom](https://simplesnippets.tech/wp-content/uploads/2018/10/what-is-document-object-model-in-JS-featured-image.jpg)

The Document object model (DOM) specifies how browsers shuould create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.

You can imagin that the HTML page is like a tree, each element has some branches under it all these branched has one parent in the top of it. which it is the `<html>` tag .

* types of Nodes:

1. document node
2. element node
3. attribute nodes
4. text nodes

### Working with the DOM tree ###

STEP 1: ACCESS THE ELEMENTS

* SELECT AN INDIVIDUAL ELEMENT NODE
* SELECT MULTIPLE ELEMENTS
* TRAVERSING BETWEEN ELEMENT NODES

STEP 2: WORK WITH THOSE ELEMENTS

* ACCESS/ UPDATE TEXT NODES
* WORK WITH HTML CONTENT
* ACCESS OR UPDATE ATTRIBUTE VALUES

<li> Access the elements : you can access any element in the DOM by using these selectors.</li>
  <ul>
 <li>getElementById(id name) : Used to select an element with a specific id.</li>

 <li>getElementsByClassName(class name) : Used to select all elements that have that class name as an attribute (Returns an array of elements), to select one of the items you can use the **item(index)** method or you can access it just like an array.</li>

 <li>parentNode: select the parent of the current element node.</li>

 <li>previousSibling/nextSibling: select the previous of next sibling of the DOM tree.</li>

 <li>firstChild/lastChild: select the first child of the last of the current element.</li>

 <li>querySelector(): Uses a CSS selector, and returns the first matching element.</li>

<li>getElementsByTagName(tag name) : select all elements that have this tag name.</li>

<li>querySelectorAll(): Uses a CSS selector to select all matching elements.</li>

----------------------------
<h2> Understanding The Problem Domain Is The Hardest Part Of Programming </h2>

There are many things is hard about programming

- Learning a new technology

- Naming things

- Testing your code

- Debugging

- Fixing bugs

- Making software maintainable

<h3> Why problem domains are hard.</h3>

The big issue is that many problem domains are like a puzzle with a blurry picture or no picture at all.you can’t really see what you are trying to build very clearly, The same thing happens when writing code. Writing code is a lot like putting together a jigsaw puzzle. We put together code with the purpose of building components that we have taken out of the “bigger picture” of the problem domain.

<h3> Programming is easy if you understand the problem domain.</h3>

understanding the problem is the most critical piece to the equation. It is very difficult to solve a problem before you know the question. It’s like buzzing in on Jeopardy before you hear the clue and shouting out random questions.

<h3> What can you do about it?</h3>

1. Make the problem domain easier
2. Get better at understanding the problem domain