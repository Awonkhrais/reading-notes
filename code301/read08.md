# Readings: APIs


REST or *Representational State Transfer* is a architectural "style for distributed systems based on hypermedia" propsed by Roy Fielding. 

### REST APIs are designed around a ____. 

REST APIs are designed around a resource. "REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client." 

### What is an identifer of a resource? Give an example. 

A resource identifier is a URI. Some examples of these identifiers can be seen like this: 

```https://adventure-works.com/orders/1 // HTTP example ```
            

### What are the most common HTTP verbs? 

Some common HTTP verbs are: GET, POST, PUT, PATCH, and DELETE. 

### What should the URIs be based on? 

The naming convention for the URIs should be based on the collection of data that you are referencing. 

### Give an example of a good URI. 

An example of a good URI can be for the collection of sales data within an internal organizational web-page. For instance for sales a URI can look like this:

```http://example-organization.com/sales ```

### What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing? 

To have a 'chatty' API can simply mean that there is too much going on and therefore will result in more latency when retrieving data. This can generally be solved by condensing large amounts of data broken into smaller bits into a larger bits. 

### What status code does a successful GET request return? 

A succesful GET code is status code 200 or 'ok' 

### What status code does an unsuccessful GET request return? 

An unsuccessful GET code is status code 404 or 'not found' 

### What status code does a successful POST request return? 

A successful POST request is status code 201 or 'created' 

### What status code does a successful DELETE request return? 

A successful DELETE request is status code 204 or successfully handled


### How would you match your name using RegEx?

I would first need to know what characters I have, and the format. So I have only letter so I would need the lower case and the upper case letters in string. 

