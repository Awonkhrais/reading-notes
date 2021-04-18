# **Domain Modeling**

Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

Here's some tips to follow when building your own domain models.

1.  When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.

2.  Model its attributes with a constructor function that defines and initializes properties.

3.  Model its behaviors with small methods that focus on doing one job well.

4.  Create instances using the new keyword followed by a call to a constructor function.

5.  Store the newly created object in a variable so you can access its properties and methods from outside.

6.  Use the this variable within methods so you can access the object's properties and methods from inside.

----------------------------------------------

# **Chapter 6: HTML Tables**

The `<table>` tag defines an HTML table.

Each table row is defined with a `<tr>` tag. Each table header is defined with a `<th>` tag. Each table data/cell is defined with a `<td>` tag.

By default, the text in `<th>` elements are bold and centered.

By default, the text in `<td>` elements are regular and left-aligned.


```html
<html>
  <head>
    <title>Tables</title>
  </head>
  <body>
    <table>
      <thead>
        <tr>
          <th></th>
          <th scope="col">Home starter hosting</th>
          <th scope="col">Premium business hosting</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th scope="row">Disk space</th>
          <td>250mb</td>
          <td>1gb</td>
        </tr>
        <tr>
          <th scope="row">Bandwidth</th>
          <td>5gb per month</td>
          <td>50gb per month</td>
        </tr>
        <!-- more rows like the two above here -->
      </tbody>
      <tfoot>
        <tr>
          <td></td>
          <td colspan="2">Sign up now and save 10%!</td>
        </tr>
      </tfoot>
    </table>
  </body>
</html>
```
<html>
 <head>
 <title>Tables</title>
 </head>
 <body>
 <table>
 <thead>
 <tr>
 <th></th>
 <th scope="col">Home starter hosting</th>
 <th scope="col">Premium business hosting</th>
   </tr>
 </thead>
 <tbody>
 <tr>
 <th scope="row">Disk space</th>
 <td>250mb</td>
 <td>1gb</td>
 </tr>
 <tr>
 <th scope="row">Bandwidth</th>
 <td>5gb per month</td>
 <td>50gb per month</td>
 </tr>
<!-- more rows like the two above here -->
 </tbody>
 <tfoot>
 <tr>
 <td></td>
 <td colspan="2">Sign up now and save 10%!</td>
 </tr>
 </tfoot>
 </table>
 </body>
</html>


`<table>` : a table tag which contain all the table tags.

`<thead>` : tells the browser that inside this tage is the table head.

`<tbody>` : tells the browser that inside this tage is the table body.

`<tr>` : table row.

`<th>` : table head data.

`<td>` : table data.

`<tfoot>` : The footer belongs inside the `<tfoot>` element.

--------------

# **Chapter 3: JS : Functions, Methods, and Objects**

## Constructor Object 

```js
let hotel = new Object();
(hotel.name = "Quay"),
  (hotel.rooms = 40),
  (hotel.booked = 25),
  (hotel.checkAvailability = function () {
    return this.rooms - this.booked;
  });


// To update the value of properties, use dot notation or square brackets.
hotel.name = "Park";
hotel["name"] = "Park";
// delete a propertiy.
delete hotel.name;
```
![object write way](./8.png)
![object write way](./9.png)

The this keyword in used insted of the object name to indicate that the property or method belongs to the object that this function created.

When do we use individual Object Or multiple Objects.

1. Indivudal Objects

   - when you are storing/ transmitting data between application.

   - for global or configuration objects that set up information for the page.

2. Multible Objects.

   - You have lots of objects used with similar functionality whithin a page.
   - A complex object might not be used in code.

   ## Arrays Are Objects.

Arrays are actually a special type of objects, They hold a related set key/value pairs, but the key for each value is its **index** number.

You can combine arrays and object inside each other.

```javascript
object1 = {
  room1: [420, 40, 10],
  room2: [460, 20, 20],
  room3: [230, 0, 0],
  room4: [620, 150, 60],
};

object1.room1[0];
//  this gives 420
```