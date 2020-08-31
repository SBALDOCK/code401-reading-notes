## Socket.io

* What is the benefit of transforming data into packets?
* UDP is often referred to as a connectionless protocol. Why is this?
  * It is considered connectionless because, as opposed to TCP, it continuously sends data to a recipient regardless of whether they receive them or not. Simply, it does not establish a connection before sending data. The packets that UDP sends are called datagrams. UDP is typically used for streaming media. 

* Can a socket server application have multiple socket connections?
  * A socket listens on a single port. Multiple connections on the same server can share a server-side PORT if they have different client-side PORTs.
  * [resource](https://stackoverflow.com/questions/11129212/tcp-can-two-different-sockets-share-a-port/11129641#:~:text=5%20Answers&text=A%20server%20socket%20listens%20on%20a%20single%20port.&text=Multiple%20connections%20on%20the%20same,system%20resources%20allow%20it%20to.)

* Can a socket connection application be connected to multiple socket servers?
  * Yes, you can use one socket per server to achieve this. 
  *[resource](https://stackoverflow.com/questions/5402019/connecting-to-multiple-servers-from-a-single-client-socket-c#:~:text=If%20your%20program%20is%20a,socket%20at%20all%2C%20just%20connect%20.&text=I%20think%20you%20are%20using,(%20aren't%20you%3F).&text=Then%20reuse%20port%20is%20not,part%20the%20start%20the%20connection.)

* Can an application be both a socket server and a socket connection?
  * Only if utilizing two different ports. Or if the sockets won't be using the port simultaneously. 
  * [resource](https://www.quora.com/Can-you-make-a-client-socket-and-a-server-socket-in-one)

### Vocabulary

* **OSI Model** - Open Systems Interconnection Model - A conceptual model that characterizes and standardizes the communication functions of a telecommunication or computing system regardless of its internal architecture or technology. It provides interoperability of diverse communication systems using standard communication protocols
  * [resource](https://en.wikipedia.org/wiki/OSI_model)

* **TCP Model** - Transmission Control Protocol - A version of the OSI model that contains four layers, as opposed to the seven layers in the OSI model. The layers are 
  * Process/Application
  * Host-to-host/Transport
  * Internet
  * Network Access/Link
  * [resource](https://www.geeksforgeeks.org/tcp-ip-model/)

* **TCP** - Transmission Control Protocol - Provides reliable and error-free communication between end systems. It performs sequencing and segmentation of data. Has a lot of overhead due to its features
  * [resource](https://www.geeksforgeeks.org/tcp-ip-model/)

* **UDP** - User Datagram Protocol - A connectionless protocol that works just like TCP but assumes error-checking and recovery services are not required. It continuously sends datagrams to recipient whether they reeive them or not. Considered less reliable than TCP since it cannot guarantee delivery. 
  * [resource](https://www.privateinternetaccess.com/blog/tcp-vs-udp-understanding-the-difference/)

* Packets - Formatted units of data carried by a packet-switched network. They consist of control information and user data. The data is known as the payload. The control information delivers data (instructions) for delivering the payload. In the OSI, this is known as the network layer (layer 3)
  * [resource](https://en.wikipedia.org/wiki/Network_packet)

* Socket - One endpoint of a two-way communication link between programs running on a network. It is bound to a port number so that the TCP layer can identify the application that data is supposed to be sent to. An endpoint is a combination of an IP address and a port number. 
  * [resource](https://docs.oracle.com/javase/tutorial/networking/sockets/definition.html#:~:text=Definition%3A,address%20and%20a%20port%20number.)