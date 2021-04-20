# **Chapter 7: HTML Forms**

The best known form on the web is probably the search box that sits right in the middle of Google’s homepage.

In addition to enabling users to search, forms also allow users to perform other functions online. You will see forms when registering as a member of a website, when shopping online, and when signing up for newsletters or mailing lists.


1.  Adding Text

    - Text input 

    - password input 

2.  Submitin forms

    - Submit button 

    - Uploding files 

3. Making Choices

    - Radio choices

    - Checkboxes 

    - Drop down boxes

    ![form](https://www.programming9.com/images/HTML-Images/form.JPG)
------------------------
# **Chapter 14 :Lists, Tables & Forms**

There are several CSS properties that were created to work with specific types ofHTML elements.

### Lists



1. `list-syle-type` : this property aloows you to control the shape or style of a bullet point.

- Unordered List (ul) :
  

- ordered List (ol) :

  - decimal (1 2 3 4 5)

  - decimal-leading-zero (01 02 03)

  - lower-alpha (a b c)

  - Upper-alpha (A B C)

  - Lower-romain (i. ii. iii.)

  - Upper-romain (I. II. III.)

2. `list-style-image` : You can specify an image to act as a bullet point using the list-style-image property.

```css
ul {
  list-style-image: url("images/star.png");
}
li {
  margin: 10px 0px 0px 0px;
}
```

3. `list-style-position` : Lists are indented into the page by default and the list-style-position property indicates whether the marker should appear on the inside or the outside of the box containing the main points.


## Forms

### Aligning from controls.

Labels for form elements are often different lengths, which means that the form controls will not appear in a straight line. This is demonstrated in the example on the right (without CSS applied to the form controls).


---
# **Chapter 6: JS Events**

![events](https://res.cloudinary.com/practicaldev/image/fetch/s--J43C-IwA--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dev-to-uploads.s3.amazonaws.com/i/1zm80qaekzgu8p54w98g.jpg)

DIFFERENT EVENT TYPES 
Here is a selection of the events that occur in the browser while you are browsing the web. Any of these events can be used to trigger a function in your JavaScript code. 
UIEVENTS Occur when a user interacts with the browser's user interface (UI) rather than the web page 

* Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked). 
* Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon. 
* When an event occurs on an element, it can trigger a JavaScript function.
* When this function then changes the web page in some way, it feels interactive because it has responded to the user. 
* You can use event delegation to monitor for events that happen on all of the children of an element. 
* The most commonly used events are W3C DOM events, although there are others in the HTMLS specification as well as browser-specific events.