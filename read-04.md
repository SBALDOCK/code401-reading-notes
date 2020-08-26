# Advanced Mongo/Mongoose

#### Why would a developer choose to make data models?
  * Data models accelerate development, reduce maintenance, increase application quality, and lower execution risks. It is basically the blueprint for a building, outlining all of the details that will result in the proper operation of the application. 
  * [hackolade.com](https://hackolade.com/benefits.html)

#### What purpose do CRUD operations serve?
  * CRUD, or create, read, update and delete represent the four ways to interact with database storage.

#### What kind of database is Postgres? What kind of database is MongoDB?
  * Postgres is a relational database system. Data is stored in tables and rows like an excel spreadsheet. Relationships are estabslished through Primary and Foreign keys.  MongoDB is a non-relational database system. Data is stores as a collection of JSON documents.
  * [medium.com](https://medium.com/@zhenwu93/relational-vs-non-relational-databases-8336870da8bc)

#### What is Mongoose and why do we need it?
  * Mongoose is an Object Data Modeling (ODM) library for MongoDB and Node.js. It essentially manages the relationship between data and translates betweeen objects in code and the representation of those objects in MongoDB.
  * [freecodecamp.org](https://www.freecodecamp.org/news/introduction-to-mongoose-for-mongodb-d2a7aa593c57/)

#### Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.
  * Three related pieces of data in an application are songs, albums and playlists within a music application. Each song belongs to an album, although albums are a separate thing not dependent on songs aside from their definition as a collection of related songs. Playlists are built by a user and may contain multiple songs from a single album, but more likely contain songs from a variety of album that the user prefers to listen to instead of or in addition to the album that a single song comes from. Playlists are not related to albums aside from the fact that playlists are built from songs that belong to albums. 


### Vocabulary

* **database** - A database acts as a storage container for various types of data that one wishes to maintain.
* **data model** - A data model is the blueprints of a database, helping conceptualize the strucutre and relationships between pieces of data. 
* **CRUD** - Create, Read, Update, Delete - The four necessary elements of Database management
* **schema** - Data that describes the content and strucutre of the database. 
* **sanitize** - Cleansing and scrubbing user input to prevent it from vulnerabilities 
* **Structured Query Language (SQL)** - A query language built to retrieve and store information in databases.
* **Non SQL (No SQL)** - Databases that are not organized like a SQL database in tabs and rows. It is a mechanism for storage and retrieval of non-relational databases.
* **MongoDB** - An object-oriented NoSQL database. Data objects are stored as separate documents inside a collection rather than in columns and rows as in relational databases. 
* **Mongoose** - Mongoose is a library that creates structure for MongoDB database usage.  
* **record** - A collection of fields about the same person, item or object in a database.
* **document** - A unique set of data stored in a NoSQL database
* **Object Relation Mapping (ORM)** - A technique for converting data between incompatible systems. This uses object-oriented programming languages. 

[home](README.md)