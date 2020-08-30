## TCP Servers

* Given the examples of front-end events such as button click, window resize, form submit, etc, what are some examples of back-end events?
  * Some examples of back-end events would be a request/response cycle to an API, the addition of some information to a database, local storage management, and user authentication. 
* Why are events sometimes better than asynchronous actions with callbacks?
  * When something needs to be repeated over and over such as a button click
* What does an EventEmitter instance do?
  * Similar to an object instance involving a constructor, an EventEmitter instance is an object that calls all functions attached to the event synchronously.
  * [resource](https://nodejs.org/api/events.html#:~:text=All%20objects%20that%20emit%20events,events%20emitted%20by%20the%20object.&text=The%20following%20example%20shows%20a%20simple%20EventEmitter%20instance%20with%20a%20single%20listener.)
* When is a program’s call stack, event queue, and event loop    active?
  * A program's call stack, event queue, and event loop are active as soon as a program is run. The first event is added to the call stack, which triggers other events to be added and subtracted from the stack as appropriate. When a callstack is fully completed, the event loop begins over again. 

### Vocabulary

* Observer Pattern - An observer patter is a relationship between objects in which if one object is modified, all of its dependent objects are automatically modified as well. The observer pattern uses a subject, observer, and client. 
  * [resource](https://www.tutorialspoint.com/design_pattern/observer_pattern.htm)
* Listener - A function that is built to wait for an event to occur, which in turn reacts by calling an event handler
  * [resource](https://www.computerhope.com/jargon/e/event-listener.htm#:~:text=An%20event%20listener%20is%20a,for%20an%20event%20to%20occur.&text=The%20listener%20is%20programmed%20to,specific%20to%20Java%20and%20JavaScript.)
* Event Handler - An event handler, upon instruction from an event listener, is a block of code that runs when an event takes place. 
  * [resource](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)
* Event Driven Programming - Event driven programming is a type of programming in which the flow is dictated by events like user actions, program loading, text entry and submission, etc. 
  * [resource](https://dzone.com/articles/what-is-event-driven-programming-and-why-is-it-so)
* Event Loop - An event loop is a model that is built to execute code, collect and process events, and execute tasks. 
  * [resource](https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop)
* Call Stack - A call stack is the lists of functions that take place when an event takes place within an application. Events are added to the callstack as they are called, and removed after they peform their duty. 
* Emit/Raise/Trigger - The emit function raises a specified event and triggers it 
  * [resource](https://www.tutorialsteacher.com/nodejs/nodejs-eventemitter)
* Subscribe - Subscriber functions define how to obtain and generate values or messages to be published Calling a subscribe method, which passes an **observer** object.
  *[resource](https://angular.io/guide/observables#:~:text=The%20subscriber%20function%20defines%20how,for%20the%20notifications%20you%20receive.)
* Database - A database is a structure for storing data. Some databases store data organized similar to a spreadsheet, which other databases store un-ordered objects. 
