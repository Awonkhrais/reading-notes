![HTML](https://lh3.googleusercontent.com/proxy/7ypNazsZZGC3lzvqoJygEecwOYezc93XA3ecZR6XRHQsQsph_mRcupcPR0qM-bqPsg_6APkGPMIdl22O40ZwgjUYoZfe6_W1-D1N1eQjxDN7tUkqTzV6snJ4biV2wYNXyOma8zpqGlQsYR9G)

# **Introduction**

**How people access the web:**

* Browsers
* Web servers
* Devices
* Screen readers

Note: all websites use HTML and CSS to create a web page.

# **HTML Structure**

```
<html>
<body>
<h1>This is the Main Heading</h1>
<p>This text might be an introduction to the rest of
the page. And if the page is a long one it might
be split up into several sub-headings.<p>
<h2>This is a Sub-Heading</h2>
<p>Many long articles have sub-headings so to help
you follow the structure of what is being written.
There may even be sub-sub-headings (or lower-level
headings).</p>
<h2>Another Sub-Heading</h2>
<p>Here you can see another sub-heading.</p>
</body>
</html>
```

* HTML are text documents that uses (tags/elements) inside angled brackets.

* Tags are usually made up of two tags: an opening tag and a closing tag.

* These tags usually come in pairs but there are some tags that don't and are called "self-closing tags".

* Opening tags can carry attributes.

* Attributes require a name and a value.

* The attribute **name** should be written in lowercase.

* The attribute **value** should be placed in double quotes.

* Tags act like containers. They tell you something about the information that lies between their opening and closing tags.

![tags attributes](./1.png)

## Body, head & title

body

You met the body element in the first example we created. Everything inside this element is shown inside the main browser window.

Head

Before the body element you will often see a head element. This contains information about the page (rather than information that is shown within the main part of the browser window that is highlighted in blue on the opposite page). You will usually find a title element inside the head element.

Title

The contents of the title element are either shown in the top of the browser, above where you usually type in the URL of the page you want to visit, or on the tab for that page (if your browser uses tabs to allow you to view multiple pages at the same time).

# **Extra Markup**

* DOCTYPES tell browsers which version of HTML you are using.

```
<!DOCTYPE html>
```

* You can add comments to your code between the markers,will not be
visible in the user's browser.

```
<!-- comment goes here -->
```

* The id and class attributes allow you to identify particular elements.(You can add Id for one element only and it can not be repeated like , Class can be implemented to more than one element)

```
<p id="pullquote"></p>

<p class="important"></p>
```
* Block Elements some elements will always appear to start on a new line in the browser window. These are known as block level elements. Examples of block elements are `(<h1>, <p>, <ul>, and <li>).`

* Inline Elements some elements will always appear to continue on the same line as their neighbouring elements. These are known as inline elements. Examples of inline elements are `<<a>, <b>, <em>, and <img>).`

* Grouping Text & Elements In a Block `<div>` , allows you to group a set of elements together in one block-level box.

* Grouping Text & Elements Inline `<span>` , this element acts like an inline equivalent of the `<div>` element. It is used to either:

1. Contain a section of text where there is no other suitable element to differentiate it from its surrounding text.

2. Contain a number of inline elements The most common reason why people use elements is so that they can control the appearance of the content of these elements using CSS.

* Escape characters are used to include special characters in your pages such as <, >, and ©.

# **HTML5 Layout**

![Layout](./2.png)

# **Process & Design**



When you want build a successful site you should collect some information to make sure that your site is going to be useful and targeting the correct people that the going to use it.

So you should take these question in consider : 

1. Who Is The Site For ?
2. Why People Visit Your Website ?
3. What Your Visitors are Trying to Achieve ?
4. What Information Your Visitors Need ?
5. How Often People Will Visit Your Site ?

### **Site Maps**

The aim is to create a diagram of the pages that will be used to structure the site. This is known as a **site map** and it will show how those pages can be grouped.

![sitemaps](./3.png)

### **Wireframes**

A wireframe is a simple sketch of the key information that needs to go on each page of a site. It shows the hierarchy of the information and how much space it might require.

![wireframe](https://d33wubrfki0l68.cloudfront.net/dbb80f2f6a5dafa25f702ad00bc429057fb59cec/52716/en/blog/uploads/versions/samuel-student-wireframe---x----972-715x---.png)

---------------------------------------------------------

![JS](https://1.bp.blogspot.com/-AiCbf3wML0s/XpxtUniW6nI/AAAAAAAADEc/a-4WeuawfoYxR57VQ0LcZTuekGhAF2F4wCLcBGAsYHQ/w1200-h630-p-k-no-nu/javascript.jpg)

# **Javascript**

### How JavaScript makes webpage more interactive :

1. **Access content** you can use JavaScript to select any element,attribute,or text from an HTML page.
2. **Modify content** you can use JavaSpcript to add element,attribute,and text to the page or remove them.
3. **Program Rules** you can specify a set of steps for the browser to follow which allows it to access or change the content of a page.
4. **React to Event** you can specify that a script should run when a specific event has occurred.

## **The ABC of programming**

**A :** What is a script and how do I create one ?

* A script is a series of instructions that the computer can follow in order to achieve a goal.

* Each time the script runs, it might only use a subset of all the instructions.

* Computers approach tasks in a different way than humans, so your instructions must let the computer solve the task prggrammatically.

* To approach writing a script, break down your goal into a series of tasks and then work out each step needed to complete that task (a flowchart can help).

**B :** How do computers fit in with the world around them ?

![B](./4.png)

**C :** How do I write a script for a web page ?

* It is best to keep JavaScript code in its own JavaScript file.
JavaScript files are text files (like HTML pages and CSS style sheets), but they have the .js extension.

* The HTML ```<script>``` element is used in HTML pages to tell the browser to load the JavaScript file (rather like the link element can be used to load a CSS file).

* If you view the source code of the page in the browser, the JavaScript will not have changed the HTML, because the script works with the model of the web page that the browser has created.

