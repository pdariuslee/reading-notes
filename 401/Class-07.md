# Readings: Express

## [HTTP Basics](https://code.tutsplus.com/tutorials/http-the-protocol-every-web-developer-must-know-part-1--net-31177)

### By Pavan Podila

---

Q: What’s the difference between PUT and PATCH?

A: PUT is a method of modifying resource where the client sends data that updates the entire resource. While PATCH applies a partial update to the resource (This means that you are only required to send the data that you want to update, and it won’t affect or change anything else.).

Q: Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

A: Swagger, Postman & Nock

Q: Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

A: Swagger - Under responses, each response definition starts with a status code, such as 200 or 404. An operation typically returns one successful status code and one or more error statuses. To define a range of response codes, you may use the following range definitions: 1XX, 2XX, 3XX, 4XX, and 5XX. If a response range is defined using an explicit code, the explicit code definition takes precedence over the range definition for that code. Each response status requires a description. For example, you can describe the conditions for error responses.

APIDoc.js - 

Q: Compare and contrast SOAP and ReST

A: SOAP

- SOAP provides the following advantages when compared to REST:

- Language, platform, and transport independent (REST requires use of HTTP)     

- Works well in distributed enterprise environments (REST assumes direct point-to-point communication)

- Standardized

- Provides significant pre-build extensibility in the form of the WS* standards

- Built-in error handling

- Automation when used with certain language products

(https://www.soapui.org/learn/api/soap-vs-rest-api/)

REST is easier to use for the most part and is more flexible. It has the following advantages when compared to SOAP:

- Uses easy to understand standards like swagger and OpenAPI 

- Specification 3.0

- Smaller learning curve

- Efficient (SOAP uses XML for all messages, REST mostly uses smaller message formats like JSON)

- Fast (no extensive processing required)

- Closer to other Web technologies in design philosophy


--- 

Term

SOAP - SOAP ( Simple Object Access Protocol) is a message protocol that allows distributed elements of an application to communicate. SOAP can be carried over a variety of lower-level protocols, including the web-related Hypertext Transfer Protocol (HTTP).  SOAP defines a header structure that identifies the actions that various SOAP nodes are expected to take on the message, in addition to a payload structure for carrying information. The concept of routing a message through a string of nodes that perform different functions is how SOAP supports things like addressing, security and format-independence. Essentially, the headers identify roles, which in turn provide the SOA features which SOAP then routes to. Stringing messages through a sequence of steps is uncommon in today’s microservice-centric development environments.

(https://searchapparchitecture.techtarget.com/definition/SOAP-Simple-Object-Access-Protocol)

ReST Verbs - specify an action to be performed on a specific resource or a collection of resources. When a request is made by the client, it should send this information in the HTTP request:

REST verb

Header information

Body (optional)

As we mentioned previously, REST uses the URI to decode its resource to be handled. There are quite a few REST verbs available, but six of them are used frequently. They are as follows:

GET

POST

PUT

PATCH

DELETE

OPTIONS

(https://hub.packtpub.com/what-are-rest-verbs-and-status-codes-tutorial/)


CRUD Verbs - The primary or most-commonly-used HTTP verbs (or methods, as they are properly called) are POST, GET, PUT, PATCH, and DELETE. These correspond to create, read, update, and delete (or CRUD) operations, respectively. 

(https://www.restapitutorial.com/lessons/httpmethods.html#:~:text=The%20primary%20or%20most%2Dcommonly,but%20are%20utilized%20less%20frequently.)

Swagger - allows you to describe the structure of your APIs so that machines can read them. The ability of APIs to describe their own structure is the root of all awesomeness in Swagger. Why is it so great? Well, by reading your API’s structure, we can automatically build beautiful and interactive API documentation.

(https://swagger.io/docs/specification/2-0/what-is-swagger/)


[Back to Home](https://pdariuslee.github.io/reading-notes/)