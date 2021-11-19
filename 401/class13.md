# Readings: Message Queues

# Review, Research, and Discussion

1. What does it mean that web sockets are bidirectional? Why is this useful?


BIDIRECTIONAL. Whereas HTTP relies on a client request to receive a response from the server for every exchange, WebSockets allow for full-duplex bidirectional communication. This enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time.

3. Does socket.io use HTTP? Why?

it depends on HTTP for its initial connection setup

5. What happens when a client emits an event?

the event passing to server

7. What happens when a server emits an event?

the event passing to clients
9. What happens if a client “misses” an event?

Unhandled messages are just ignored. It's just like when an event occurs and there are no event listeners for that event. The socket receives the msg and doesn't find a handler for it so nothing happens with it.

11. How can we mitigate this?

You could avoid missing messages by always having the handlers installed and then deciding in the handlers (based on other state) whether to do anything with the message or not.

# Term

* Socket: A socket is one endpoint of a two-way communication link between two programs running on the network
* Web Socket: protocol enables interaction between a web browser (or other client application) and a web server
* Socket.io: is a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers. It has two parts: a client-side library that runs in the browser, and a server-side library for Node. js
* Client:  a person or group that uses the professional advice or services
* Server: is a piece of computer hardware or software,Typical servers are database servers, file servers, mail servers, print servers, web servers
* OSI Model: Open Systems Interconnection (OSI) model describes seven layers that computer systems use to communicate over a network
* TCP Model:  full Transmission Control Protocol/Internet Protocol, standard Internet communications protocols that allow digital computers to communicate over long distances.
* TCP: stands for Transmission Control Protocol a communications standard that enables application programs and computing devices to exchange messages over a network
* UDP: (User Datagram Protocol) is a communications protocol that is primarily used for establishing low-latency and loss-tolerating connections between applications on the 

# Preview

* Which 3 things had you heard about previously and now have better clarity on?

TCP, UDP,OSI
* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

Socket.io
* What are you most excited about trying to implement or see how it works?

Socket.io

# Preparation Materials

Rooms:
A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients

![room](https://socket.io/images/rooms.png)

You can call join to subscribe the socket to a given channel:

io.on("connection", (socket) => {
  socket.join("some room");
});

Namespaces:
A Namespace is a communication channel that allows you to split the logic of your application over a single shared connection (also called "multiplexing").

io.of("/orders").on("connection", (socket) => {
  socket.on("order:list", () => {});
  socket.on("order:create", () => {});
});

io.of("/users").on("connection", (socket) => {
  socket.on("user:list", () => {});
});
