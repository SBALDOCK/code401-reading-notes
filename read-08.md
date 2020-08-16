## Express Routing & Connected API

Routes can be managed in separate modules from the main server, allowing us to extract that logic and wiring to be more topical.

How does this change the server’s role?

* index.js - Entry Point
* server.js - Hub, Exported Server
* models/categories.js, etc - Data Models
* routes/categories.js, etc - Routers and Handlers

* Incorporating separate modules from the main server better organizes code. Each module has its own file just for that use. Testing is also simplified. 

### Using Express Routing

* Routing is how application endpoints respond to client requests
* Routing methods specify a callback function (handler function)
* Application "listens" for requests that match the specified routes and methods. When it detects a match, it calls the specified callback function
* If routing method has more than one callback functions, must use "next" as an argument in the callback and call "next()" iin body of function
* App.all() works for **all** HTTP request methods
* $ must be escaped within ([]) in a path string
* Route paths can be strings or use **Regex** expressions
* **Express Routers** are mini express applications without all the bells and whistles of an express application - Only the routing elements
* Order is important - Middleware must be placed prior to route requests
* Use **.param()** to run for a certain parameter
  Example - router.param('name', function(req, res, next, name) {
  })
