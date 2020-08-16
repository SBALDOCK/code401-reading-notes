## Express

### Express Routing
* This is an event driven system
* Same routing patter as vanilla JS and JQuery
* When a get event happens on "/thing", run this function...
* The **request** object will accept Parameters and Query Strings
* The **response** object is responsible for sending data back to browser
* Responses include headers, cookies, and status codes

### Express Middleware
* Middleware is a series of functions that the request moves through
* Each receives **request, response and next** as parameters
* Two types - Application and Route
* **Application**
  * Error handling
  * Bringing in other routes
  * Applies Defaults
  * JSON, Body and Form parsing
  * Runs on every request
* **Route**
  * Specifically for a route
  * Are you logged in?
  * What is your IP?
  * Have we seen you here before?

### Modularization & Separation of Concerns
* Modularize code into logical chunks
* Each thing should do the thing it is best at

### CRUD Operations with REST and Express
* CREATE - app.post('/resource')
* READ - app.get('/resource')
* UPDATE - app.put('/resource/:id')
* DELETE - app.get('/resource/:id')

### Server Testing
* Avoid starting actual server for testing
* Export server as a module in a library
* Use **supertest** to run tests
  * Hits routes as though server is running without starting it
  * One less thing to go wrong (eliminate variables)
* Wrap **superagent** in a module that persons this
  * 100% fake every call to the API
  * Only tests the interface to the API, not actual data

### Test Pyramid
* Server Testing
  * Units - Server Internal Functions
    * Mock integrations
  * Integration - How it connects to other services
    * Hard dependencies
  * Acceptance
    * Server might be a dependency of another test

### What is Middleware?
  * Functions invoked by the Express.js routing layer before final request handler is made
  * On a route, do something first, then pass it along to the next function
  * Request and Response used each time to pass to the next whatever it is being handled
  * Deal with CORS or CSRF issues first, check to see if user is authorized, and then send them where they want to go
  * **App.use** runs middleware on all requests
  * Can declare middleware functions wherever in file due to hoisting

