## Message Queues

* What does it mean that web sockets are bidirectional? Why is this useful?
  * Bidirectional means they perform two-way communication between the server and browser. It allows efficient data push from the server to the client. 
  * It is useful for users to pull data and dynamically update content on web pages. 
  * [resource](https://medium.com/@IgnoreIntuition/bi-directional-communication-with-websocket-e9a41b8936a4)

* Does socket.io use HTTP? Why? 
  * Yes, socket.io servers attach to an HTTP server so that it can serve its own client code using socket.io libraries. Also, this provides other transports aside from websockets for scenarios when websockets aren't supported, required, or wanted. 
  * [resource](https://stackoverflow.com/questions/37836130/socket-io-why-does-it-need-an-http-server#:~:text=The%20premise%20on%20which%20your,%2C%20which%20it%20isn't.&text=Even%20when%20websockets%20can%20be,%2Fsocket.io.js%20.)

* What happens when a client emits an event?
  * When an event is invoked, socket.io passes a socket object to the function. This is passed to the server through websockets. 
  * [resource](https://stackoverflow.com/questions/48332454/how-does-socket-io-on-the-client-listen-to-events-emitted-from-server)

* What happens when a server emits an event?
  * If the client has an event listener prepared to listen for the server event, the event will be triggered. Otherwise, it'll be a missed message. 

* What happens if a client “misses” an event?
  * If a client misses an event, the event simply does not take place. Unhandled events are ignored. 
  * [resource](https://stackoverflow.com/questions/32816290/what-happens-with-unhandled-socket-io-events)

* How can we mitigate this?
  * This can be mitigated by always having event handlers installed and having them decide whether to do anything with a missed message. Alternatively, you can obtain the list of callbacks from the socket and use it to compare to the incoming message header. 
    * [resource](https://stackoverflow.com/questions/32816290/what-happens-with-unhandled-socket-io-events)


### Vocabulary

* Web Socket - A communications protocol using a single TCP channel. Although distinct from HTTP, it is designed to work over HTTP ports 443 and 80 and is thus compatible with HTTP. It enables interaction between a web browswer and a web server with lower overhead than HTTP. 
  * [resource](https://en.wikipedia.org/wiki/WebSocket)

* Socket.io - A JavaScript library for realtime web applications, enabling bi-directional communication between a client and server. It has a client-side library running in the browser and a server-side library for Node.js. Socket.io is event driven. It provides the ability to impleletn real-time analytics, binary streaming, instant messaging, and document collaboration. 
  * [resource](https://en.wikipedia.org/wiki/Socket.IO)

* Client - A piece of hardware or software that accesses services made available by a server as part of the client-server model. If the client is on a separate system than the server, the client accesses services by way of a network. It relies on sending a request to another program or computer hardware/software. Web browsers are web clients that connect to web servers and retrieve web pages for display. 
  * [resource](https://en.wikipedia.org/wiki/Client_(computing))

* Server - A piece of computer hardware or software that provides functionality for clients. Servers provide service such as sharing data resources among multiple clients and performing computation for a client. A single server can serve multiple clients, just as a single client can use multiple servers. Most servers are database servers, file servers, mail servers, application servers. 
  * [resource](https://en.wikipedia.org/wiki/Server_(computing))