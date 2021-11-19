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
