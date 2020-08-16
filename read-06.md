# HTTP and REST

### HTTP

* HTTP - Hyper Text Transfer Protocol
* Stateless request-response layer protocol
* Foundation of the WWW
* Clients - Hosts that make requests in client-server model
* Server - Host designed to provide a service
* HTTP requests are formmated in text and transferred using TCP
* **TCP** - Transmission Control Protocol
* **Requests**
  * First line contains Method, URL, and HTTP Version
  * Example - POST / api/note HTTP/1.1
  * Following lines are request headers
    * Header is a key/value pair separated using a colon
* **Response**
  * Also formatted in text and transferred using TCP
  * First line contains HTTP version, Status Code, and Status Message
    * Example - HTTP/1.1 200 OK

### REST

* REST - REpresentational State Transfer
* Architecture style for designing networked applications
* Relies on a stateless, client-server protocol, almost always HTTP
* Treats server objects as resources that can be created or destroyed
* Can be used by virtually any programming language
* GET : READ
* POST : CREATE
* PUT : UPDATE
* PATCH : UPDATE
* DESTROY : DELETE
* Generally speaking, RESTful endpoints deliver data in JSON format
* **Swagger** - Swagger Docs present developers a way to see how to use APIs AND use it - live requests from within it
* 

### What is a REST API?

* API - Application Program Interface
  * APIs are everywhere
  * Contract provided by one piece of software to another
  * Structured request and response
  * A messenger between running software
* Some APIs require authentication to use their service
  * OAUTH - Access token
*

### HTTP Methods

* GET: Retrieve data from a specified resource
  * Most common type of request
* POST: Submit data to be processed to a specified resource
  * Example - Filling out a web form
* PUT: Update a specified resource
  * Usually send a request to an endpoint with an ID for the resource
* DELETE: Delete a specified resource
  * Need to send an ID to let server know what to delete
* HEAD: Rarely used
  * Same as get but does not return a body
* OPTIONS: Rarely used
  * Returns supported HTTP methods
* PATCH: Rarely used
  * Update partial resources

### Vocab

* URL - Uniform Resource Locator
  * Consist of protocol, host, port, resource path, and query
  * Example -  HTTP      www.  1234  path/to/resource   a=b&x=y
* URI - Uniform Resource Identifier
* Postman - Google chrome extension for submitting API requests




