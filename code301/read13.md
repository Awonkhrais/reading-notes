# Status Codes Based On REST Methods


### In your own words, describe what each group of status code represents:
100’s = *Informational status codes* 

200’s = *Success status codes request accepted*

300’s = *Redirection Status codes resource not available at location* 

400’s = *Client error codes* 

500’s = *Server error codes* 

### What is a status code 202?

A status code 200 rerpesents the asynchronous processing of the request. 

### What is a status code 308?

A status code 308 will redirect the client to another URL, and also not to use the current any longer. 

### What code would you use if an update didn’t return data to a client?

Status code 204 occurs when the data cant be returned to the client. 

### What code would you use if a resource used to exist but no longer does?

I think we could use code 308, to redirect the client. 

### What is the ‘Forbidden’ status code?

The forbidden status code will basically says there was no need for authorization, but we are going to block your access anyway. 

## Why do we need to pull our MongoDB database string out of our server and put it into our .env?

not only should we use the .env to hold our string for security, but we will also change the URL once we deploy. 

## What is middleware?
Middleware is software that basically the connection between the application, the user, and the data. 

## What does app.use(express.json()) do?

This line will allow to recieve json data as a body, instead of something like a  POST element or a GET. 

## What does the /:id mean in a route?

the :id is a parameter that can be accessed with the request method. This can looked at like the id attributes in HTML.

## What is the difference beween PUT and PATCH?

PUT will update all the information all at once, while PATCH updated data selectively(passed). 

## How do you make a defalut value in a schema?
Within schema you can create a default value by defining default 

          default: 
          
          
## What does a 500 error status code mean?

Status code 500 is an internal server error. 

## What is the difference between a status 200 and a status 201?

Status code 200 is good and 'ok'. Status code 201 will go to the backend side and signal creation for the resource and return with the header resources. 