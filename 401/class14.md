
# Readings: Event Driven Architecture

# Review, Research, and Discussion

* What’s the difference between a FIFO and a standard queue?

Standard queues provide at-least-once delivery, which means that each message is delivered at least once. FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it.

* How can the server be assured a message was properly received?

wait for the sever to acknowledge the delivery, after a certain period of time.

* What classic design pattern is best represented by event driven programming?

server-observer pattern

* How do you test an event driven system?

You can test an event driven system with test unit.


# Term

* FIFO Queue: In FIFO queues, messages are ordered based on message group ID
* Pub/Sub: Publish/subscribe messaging, or pub/sub messaging, is a form of asynchronous service-to-service communication used in serverless and microservices architectures

# Preparation Materials

AWS SNS is a publisher subscriber network, where subscribers can subscribe to topics and will receive messages whenever a publisher publishes to that topic. AWS SQS is a queue service, which stores messages in a queue.

SNS :simple notification service

SQS :simple queue service
