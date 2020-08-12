# Node Ecosystem, TDD, CI/CD

### Reading, Research, and Discussion

* Why would you want to run JavaScript outside of a browser
  * Anytime JavaScript is used on the backend to interact with a Database, APIs, etc. using a server, one utilizes JavaScript outside of a browser. 

* What is the difference between a module and a package?
  * A module is a single file or block of code while a package is a collection of modules in directories that give a package hierarchy 
    [article](https://stackoverflow.com/questions/7948494/whats-the-difference-between-a-python-module-and-a-python-package#:~:text=A%20module%20is%20a%20single,e.g.&text=A%20package%20is%20a%20collection,that%20give%20a%20package%20hierarchy.&text=Any%20Python%20file%20is%20a,file's%20base%20name%20without%20the%20.)

* What does the Node Package Manager do?
  * NPM makes it easy for developers to share and resuse code to solve problems. Other developers can reuse the code in their own applications. It is easy to download updates to the code when they are made. The bits of resuable code are called packages. The biggest benefit is to utilize small solutions from outside your organization, written by specialists or those who have focuses specifically on solving that one little problem. Users can use the npm client to publish code and have it added to the NPM registry. 
    * [video](https://docs.npmjs.com/about-npm/index.html)

* Provide code snippets showing 3 different ways to export a function from a node module 
  * [resource](https://www.sitepoint.com/understanding-module-exports-exports-node-js/)

1. Require export
  * `const fs = require('fs');
     const folderPath = '/home/jim/Desktop/';

     fs.readdir(folderPath, (err, files) => {
       files.forEach(file => {
         console.log(file);
       });
    });`

2. Create and export
  * `const getName = () => {
      return 'Jim';
    };

    exports.getName = getName;`

3. Export a default value
  * `class User {
      constructor(name, age, email) {
        this.name = name;
        this.age = age;
        this.email = email;
      }

      getUserStats() {
        return `
          Name: ${this.name}
          Age: ${this.age}
          Email: ${this.email}
        `;
      }
    }

    module.exports = User;`

### Vocabulary Terms

* **ecosystem** - A collection of projects that are developed and evolve in the same programming environment. Typically, the projects share a common technological platform or language. 

* **Node.js** - An open-source, cross-platform, JavaScript framwork that executes JavaScript code outside of a web browser. Node.js provides unifying web-development around a single programming language rather than different languages for server and client scripts. 

* **V8 Engine** - Google's open source JavaScript and WebAssembly engine, utilizing C++. It takes JavaScript and executes it while browsing with Chrome. It acts indepedently from the brower in which it is hosted, which enabled the rise of Node.js. 

* **module** - A program that can be imported for use when needed. Each module servers a unique and separate operation and can be reused throughout a Node.js application. 

* **package** - A package is a collection of modules, or a directory with one or more files in it. 

* **node package manager(npm)** - NPM is a website, registry, and a client. This system allows programmers to publish and share code solutions that solve specific problems. Other programmers can easily install and use these solutions for their own code rather than having to try and solve the issue themselves. 

* **server** - A computer that provides services and data to a client, which is how the client-server model is built. A client interacts with a server by requesting some information, data, or resources. The server provides the answer (response) to that request.   

* **environment** - A setup for programming, including necessary software, working internet connection, browser, text editor, etc. 

* **interpreter** - A computer program that executes instructions written in a programming or scripting language. This does not require the instructions to have been previously compiled into a machine language program. 

* **compiler** - A program that converts instructions so that they can be read and executed by a computer. This also may involve translating computer code from one programming language into another. 

### Video - What is NPM?

* Makes it easy for developers to share code
* Other devs can reuse the code in their appplications
* Easy to make updates and download updates
* Solutions are referred to as packages, or sometimes modules
* Typical website will depend on hundreds of packages
* Makes it possible to compose large custom solutions out of shared code
* Easy to reuse code built by specialists outside of organization
* Easy to reuse code across multiple projects
