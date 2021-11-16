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
