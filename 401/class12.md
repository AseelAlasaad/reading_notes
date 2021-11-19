# Readings: Socket.io

# Review, Research, and Discussion

**What is the benefit of transforming data into packets?**

share data between computers, Data packets are able to find the destination without the use of a dedicated channel


Packets are intended to transfer data reliably and efficiently. Instead of transferring a large file as a single block of data

**UDP is often refereed to as a connectionless protocol. Why is this?**


UDP is a connectionless protocol. No connection needs to be established between the source and destination before you transmit data. UDP does not have a mechanism to make sure that the payload is not corrupted

**Can a socket server application have multiple socket connections?**

Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to

**Can a socket connection application be connected to multiple socket servers?**


Yes - you need one socket for each connection

**Can an application be both a socket server and a socket connection?**

You can use the same socket for whatever you want, as long as your protocol handles it

# Term

* Observer Pattern: is used when there is one-to-many relationship between objects such as if one object is modified, its depenedent objects are to be notified automatically. 
* Listener: The listener is programmed to react to an input or signal by calling the event's handler.
* Event Handler: is a callback subroutine that handles inputs received in a program
* Event Driven Programming: The program responds to events that the user generates in interacting with GUI components.
* Event Loop: is a programming construct or design pattern that waits for and dispatches events or messages in a program
* Event Queue:The event queue is responsible for sending new functions to the track for processing
* Call Stack:is composed of stack frames (also called activation records or activation frames)
* Emit/Raise/Trigger: the client and server communicate through events
* Subscribe: is a messaging pattern where senders of messages, called publishers,
* database: is a repository of information managed by a database engine which ensures integrity of data and fast access to the data

# Preview


* Which 3 things had you heard about previously and now have better clarity on?
   
   database, event

* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  
  call stack , event queue

* What are you most excited about trying to implement or see how it works?

event handler, event queue

# Preparation Materials

**Socket.io**

Socket.IO is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface

**features of Socket.IO**

* It helps in broadcasting to multiple sockets at a time and handles the connection transparently.
* It works on all platform, server or device, ensuring equality, reliability, and speed.
* It automatically upgrades the requirement to WebSocket if needed.
* It is a custom real-time transport protocol implementation on top of other protocols.
* It requires both libraries to be used Client side as well as a server-side library.
* IO works on work-based events. there are some reserved events that can be accessed using the Socket on the server side like Connect, message, Disconnect, Ping and Reconnect.

**Why do we need Socket.IO:**

* It handle all the degradation of your technical alternatives to get full-duplex communication in real-time.
* It also handles the various support level and the inconsistencies from the browser.
* It also gives the additional feature room support for basic publish infrastructure and thinks like automatic reconnect.
