# Chapter 16: Images

![img](https://lh3.googleusercontent.com/proxy/_pmbGrGV3T8UC9YChWEtEoBQM3YXhugrAEH_aa9VopWHDdnER153gz1MVLERQreQ8WYHaolFetMA8-sI5e3cxHn36hRSOsGVbM-DEF1oG3BE9wMFO7g)

CSS Setting height and width for images the height and width properties are used to set the height and width of an element.

The `height` and `width` properties do not include padding, borders, or margins. It sets the height/width of the area inside the padding, border, and margin of the element.


### Aligne Images Using CSS.

```css
img.align-left {
  float: left;
  margin-right: 10px;
}
img.align-right {
  float: right;
  margin-left: 10px;
}
img.medium {
  width: 250px;
  height: 250px;
}
```

### Center Images using CSS

```css
img.align-center {
  display: block;
  margin: 0px auto;
}
img.medium {
  width: 250px;
  height: 250px;
}
```

### Background Images.

The background-image property allows you to place an image behind any HTML element. This could be the entire page or just part of the page. By default, a background image will repeat to fill the entire box.

```css
body {
  background-image: url("image-Path");
}
```

**background-repeat** : The background-repeat property can have four values:

  - repeate : The background image is repeated both horizontally and vertically (the default way it is shown if the background-repeat property isn't used).

  - repeat-x : The image is repeated horizontally only

  - repeat-y : The image is repeated vertically only.

  - no-repeat : The image is only shown once.

**background-attachment** : specifies whether a background image should stay in one position or move as the user scrolls up and down the page. It can have one of two values:

  - fixed : The background image stays in the same position on the page.

  - scroll : The background image moves up and down as the user scrolls up and down the page.


  # Chapter 19: Practical Information

  ![seo](https://blog.mailrelay.com/wp-content/uploads/2016/12/campana-seo.png)

  **Search Engine Optimization (SEO)**

Search engine optimization (or SEO) is the practice of trying to help your site appear nearer the top of search engine results
when people look for the topics that your website covers.

**(the words people might search on to find your site) can appear in order to improve its findability:**
1. Page title
2. URL / Web Address
3. Headings
4. Text
5. Link text
6. image ALT text 
7. Page descriptions


----------------------

# Video and Audio APIs.

HTML5 comes with elements for embedding rich media in documents `<video>` and `<audio>`

<video controls>
  <source src="img/rabbit320.mp4" type="video/mp4">
  <p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
</video>

```js
<video controls>
  <source src="img/rabbit320.mp4" type="video/mp4">
  <p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
</video>
```

You can review what all the HTML features do in the article linked above; for our purposes here, the most interesting attribute is `controls`, which enables the default set of playback controls. If you don't specify this, you get no playback controls.