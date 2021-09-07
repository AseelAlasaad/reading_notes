# Read08

**What does REST stand for?**

**REST stands for representational state transfer**

Roy Fielding proposed Representational State Transfer (REST) as an architectural approach to designing web services. REST is an architectural style for building distributed systems based on hypermedia. REST is independent of any underlying protocol and is not necessarily tied to HTTP. However, most common REST API implementations use HTTP as the application protocol, and this guide focuses on designing REST APIs for HTTP.

**What is an identifer of a resource? Give an example**

 For example, in an e-commerce system, the primary entities might be customers and orders. Creating an order can be achieved by sending an HTTP POST request that contains the order information. The HTTP response indicates whether the order was placed successfully or not. When possible, resource URIs should be based on nouns (the resource) 

 **What are the most common HTTP verbs?**

The most common types of request methods are GET and POST but there are many others, including HEAD, PUT, DELETE, CONNECT, and OPTIONS.


**What should the URIs be based on?**

URIs should be short in length.

**What status code does a successful GET request return?**

A successful GET method typically returns HTTP status code 200 (OK). 

**What status code does an unsuccessful GET request return?**

If the resource cannot be found, the method should return 404 (Not Found).

**What status code does a successful POST request return?**

If a POST method creates a new resource, it returns HTTP status code 201 (Created). The URI of the new resource is included in the Location header of the response. The response body contains a representation of the resource.


**What status code does a successful DELETE request return?**

If the delete operation is successful, the web server should respond with HTTP status code 204 (No Content),


