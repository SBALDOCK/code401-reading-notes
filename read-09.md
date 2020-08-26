## API Server

### Express: Router Parameters
* Parameters in routes can be read
  * `app.get('/place/:city', (req, res) => {`
    `//req.params.city is now a readable value`
    `})`
* Middleware can run on any route
  * `app.get('/places/:city', getZip, (req, res) => {`
    `//req.params.city is read from the param`
    `//req.body.zip was grafted onto the request object`
    `by middleware})`
* Run middleware on every request
  * `app.use(getZip)`
* With Express, run middleware only when certain parameters are present and expected
  * `router.param('city', function (req, res, next, id) {`
    `console.log('Only runs on routes that have a city param')`
    `next()`
    `})`

### Sub Documents in Mongoose
* Mongoose provides structure to Mongo documents by providing rules and validation around data models
* With **sub-documents**, Mongoose uses a **schema** to describe a deeper part of the data model
  * Example - An online store has products, and also customers who have purchases products. With a **schema**, one can connect the store's products with the items ordered in a separate array
* Sub-documents are not "populated" unless done so manually
* 

### Middleware
* Also called pre and post **hooks**
* Functions that are passed control during execution of asynchronous functions
* Specified on the schema level
* Useful for writing plugins
* **Pre** middleware functions are executed one after another when each middleware calls the `next()` function
* **Post** middleware functions are executed after all pre middleware are run
* 

### Types of Middleware
* Document Middleware
  * **this** refers to the document
* Model Middleware
  * **this** refers to the model
* Aggregate Middlware
  * Executes whe `exec()` is called on an aggregate object
  * **this** refers to the aggregation object
* Query Middleware
  * **this** refers to the query

### Vocab
* ORM - Object-Relational Mapping - Converting data between incompatible systems


[home](README.md)