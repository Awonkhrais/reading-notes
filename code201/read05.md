# **Chapter 5 :  Images** 

Images should be :

* Be relevant
* Convey information
* Convey the right mood
* Be instantly recognisable
* Fit the color palette

```
<img
  src="https://aws-tiqets-cdn.imgix.net/images/content/b344ad3ceb934267846a0233d35bc97a.jpg?auto=format&fit=crop&ixlib=python-3.2.1&q=25&s=5c0f733ddca9f01b2760b24f2208bc83&w=375&h=250&dpr=2.625"
  alt="Real madrid stadium"
  title="this stadium called santiago bernabeu"
/>
```
![stadium](https://aws-tiqets-cdn.imgix.net/images/content/b344ad3ceb934267846a0233d35bc97a.jpg?auto=format&fit=crop&ixlib=python-3.2.1&q=25&s=5c0f733ddca9f01b2760b24f2208bc83&w=375&h=250&dpr=2.625)

`src`: This tells the browser where
it can find the image file. This will usually be a relative URL pointing to an image on your own site.

`alt`:This provides a text description of the image which describes the image if you cannot see it.

`title` : You can also use the title attribute with the `<img>`element to provide additional information about the image.

`align` : you can choose between left,right,middle,bottom,and top.

### **HTML5 Figure and Figure caption.**

`<figure>`:Images often come with captions. HTML5 has introduced a new `<figure>` element to contain images and their caption so that the two are associated. you can have more than one image in the `<figure>` tag, you can say it is like the container.

`<figcaption>` : The `<figcaption>` element has been added to HTML5 in order to allow web page authors to add a caption to an image.

Example:

```html
<figure>
  <img
    src="img/otters.jpg"
    alt="Photograph of   two sea otters floating in water"
  />
  <br />
  <figcaption>
    Sea otters hold hands when they sleep so they don't drift away from each
    other.
  </figcaption>
</figure>
```

<figure>
  <img
    src="https://rmadrid37.files.wordpress.com/2015/05/dem-fans.jpg"
    alt="Photograph of real madrid stadium"
  />
  <br />
  <figcaption>
    real madrid fan at stadium in champions legaue match.
  </figcaption>
</figure>


--------------------------

# **Chapter 11: Color**

Color can really bring your pages to life. The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:

* RGB values : These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90)
* hex codes : These are six-digit codes that represent the amount of red, green and blue in a color, preceded by # sign. For example: #ee3e80
* color names : you can type the color you want.
* HSL : (hue, saturation, lightness) 

# **Chapter 12 : Text**

There is 3 main types of default fonts in general.

- Serif : <p style="font-family: serif; ">Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs</p>.

- Sans-serif : <p style ="font-family: sans-serif;">Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.</p>

- Monospace : <p p style ="font-family: monospace;">Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts have different widths.)</p>

These fonts and many others are installed in your computer by default, but what if i want to use a font that is not intalled?

```css
@font-face {
  font-family: "ChunkFiveRegular";
  src: url("fonts/chunkfive.eot");
}
h1,
h2 {
  font-family: ChunkFiveRegular, Georgia, serif;
}
```

as shown above you can use something called `@font-face` this makes you define a new font family with its url and source, then you can use it freely in any selector you want.

Some important properties for text :

`font-weight : bold/normal` : it makes your text <span style="font-weight : bold">bold</span> ir normal.

`font-style : normal/italic/oblique` : it makes your text appear normal, <span style="font-style : italic">italic</span>, and <span style="font-style : obliqu">obliqu</span>

`text-transform : uppercase/lowercase/capitalize` it makes you text , <span style = "text-transform : uppercase" > uppercase</span> , <span style = "text-transform : lowercase" > LOWERCASE</span> , <span style = "text-transform : capitalize" > capitalize</span>.

`text-decoration : none/underline/overline/line-through/blink` it makes you text , <span style = "text-decoration: none" > none</span> , <span style = "text-decoration : underline" > underline</span> , <span style = "text-decoration : overline" > overline</span>,
<span style = "text-decoration: line-through" > line through</span> , <span style = "text-decoration : blink" > blink</span>

`line-height` : take a unit like 5px of 1.5 just like WORD , it gives a space between each line.

`letter-spacing/word-spacing` : <span style = "letter-spacing: 5px" > letter spacing</span>

<span style = "word-spacing: 5px" > This Text has normal space</span>

`text-align: left/right/justify/center` :

<p style = "text-align: left" > This Text has left align</p>  
<p style = "text-align: right" > This Text has right align</p>  
<p style = "text-align: center" > This Text has center align</p>  
<p style = "text-align: justify" > This Text has justify align</p>

`text-shadow` :

<p style = "background-color: #cccccc;
color: #ffffff;
text-shadow: 2px 2px 7px #111111;" > This Text has shadow </p>

| Selector  | meaning | example |
| :-------: | :----------------------------------- |--------------------------------|
| existence |                             [ ] Matches a specific attribute                              | p[class] select all p with class attribute                                               |
| equality  |                  [=] Matches a specific attribute with a specific value                   | p[class="dog"] select all p with attribut class has a value of dog                       |
|   Space   | [~=] Matches a specific attribute whose value appears in a space- separated list of words | p[class~="dog"] select all p with attribute class and has a seperated value contains dog |  |
|  prefix   |        [^=] Matches a specific attribute whose value begins with a specific string        | p[attr^"d"] select all p with an attribute begins with d letter                          |
| Substring |        [*=] Matches a specific attribute whose value contains a specific substring        | p[attr*"do"] select any p with and attribute has a value contains the letter do          |
|  Suffix   |         [$=] Matches a specific attribute whose valu ends with a specific string          | p[attr$"g"] targer any p with an attribute has a vale ends with the letter g             |