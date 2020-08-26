# Classes, Inheritance, Functional Programming

### Name 3 Advantages to Test Driven Development
  * Writing tests first requires deep consideration of what the end goal of the code is
  * Fast feedback - Creating a short development cycle with tests up front provides quick feedback
  * Reduced time spent on rework - Short development cycles and regular testing reduces the need to go back and rework elements that were otherwise missed through a standard development cycle
  [dzone](https://dzone.com/articles/20-benefits-of-test-driven-development)
### In what case would you use beforeEach() or afterEach()?
  * Use **beforeEach()** if one test is changing the setup for the next test, as it resets conditions for the next test each time
  * Use **afterEach()** when some type of cleanup needs to happen after each test runs
### What is the one downside of Test Driven Development?
  * TDD tends to take more work up front writing code and tests and can be difficult for a larger organization to implement
  * [mediumarticle](https://medium.com/@stevenpcurtis.sc/test-driven-development-tdd-the-advantages-and-disadvantages-5347899ead90)
### What's the primary difference between ES6 classes and constructor/prototype classes?
  * The primary difference is the structure of syntax, or syntactic sugar. ES6 classes are easier to read and interpret. Additionally, it works better with inheritance if you want various objects to inherit a parent attribute. 
### Name the use case for a static method?
  * If you need a method to compare various objects in a single class, build a static method that belongs to the class itself. For instance, if you had a bunch of animals in an animal class and needed to compare a feature such as fur, you could use a static method to do this. 
### Write an example of a Higher Order function and describe the use case it solves
  * `let random = function() {
    return Math.randon
  }`
  * This function identifies a random number. Higher order functions are essentially functions that run other functions. 
### Vocabulary

* **Functional Programming** - The process of building software using pure functions, avoiding shared state, mutable data, and side-effects. Functional programming is delcarative rathe rthan imperative. It can be contrasted with object-oriented programming. 
* **Pure Function** - A function whose return value is based only on its inputs and has no other dependencies or effects on a program. The function always returns the same value for the same intputs. 
* **Higher-order Function** - A function that takes a function as an argument, or returns a function. Contrast with first order functions, which don't take a function as an argument. 
* **Immutable State** - A state that cannote be modified after creation.
* **Object** - A data type that can include multiple properties and methods, including other objects. Most languages define objects as classes. 
* **Object-oriented programming (OOP)** - A programming methodology based on objects, instead of just functions and procedures. Objects are organized into classes, which allow individual objects to be grouped together. This makes it easier for programmers to structure and organize their programs.
* **Class** - Specifies how instances (objects) are created and how they behave
* **Prototype** - A type of object to which additional properties can be attached to it which will be shared across all instances of it's constructor function. 
* **Super** - Javascript keyword used by a child class to call it's parent's constructor function. 
* **Inheritance** - Methods from a parent class are copied to a derived (child) class. Inheritance is uppprted by using the prototype object. 
* **Constructor** - A moetho of a class for creating and initializing an object of that class
* **Instance** - An object that has been created and exists in memory. 
* **Context** - Refers to the object within a function being executed.
* **this** - Within a constructor, refers to the object that will be created when the constructor is run. 
* **Test Driven Development (TDD)** - Programming practice which involves developing tests for every small functionality of an application. It instructs developers to write new code only if an automated test has failed. This avoids duplication of code. 
* **Jest** - Javascript testing framework with a focus on simplicity
* **Continuous Integration (CI)** - A coding philosophy and set of practices that drive development teams to implement small changes as a mechanism to integrate and validate changes. 
* **Unit Test** - Software testing method where individual units of source doe are tested to determine whether they are fit for use. 

[home](README.md)


