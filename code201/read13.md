# The Past, Present & Future of Local Storage for Web Applications.


The need of localStorage were essential to have these benefits:

- A lot of storage space.
- On the client side.
- Persists beyond a page refresh
- Isn't transmitted to the server

It was nessary to over come the usadge of Cookies, of course they could be used for persistent local storage of small amount of data, but they have some dealbreaking downsides:

- They are included with every HTTP request, therby slowing down the web application, therby sending data unencrypted over the internet.

- They are limited to 4 KB of data, enough to slow down your application, but not enought to be terribly useful.

![storge](https://i.morioh.com/2020/04/04/3bdf918d08a3.jpg)


# INTRODUCING HTML5 STORAGE

## what is HTML5 Storage?

it’s a way for web pages to store named key/value pairs locally, within the client web browser.Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.the latest version of pretty much every browser supports HTML5 Storage… even Internet Explorer!


## USING HTML5 STORAGE

- HTML5 Storage is based on named key/value pairs.

- The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. 

### setItem() & getItem() & removeItem():
- Calling setItem() with a named key that already exists will silently overwrite the previous value. 

- Calling getItem() with a non-existent key will return null rather than throw an exception.

- Calling removeItem() deletes the value,  with a non-existent key will do nothing.