# Readings: Event Driven Applications

# Review, Research, and Discussion

**Why is access control important?**

 Access controls limit access to information and information processing systems.
 because it is a valuable security technique that can be used to regulate who or what can view or use any given resource

**Describe an application that would need access control.**
 * Login credentials
 * PINs and one-time passwords
 * Virtual private network (VPN) access to internal networks.

**What is a role used for?**

A role is a collection of privileges that can be granted to one or more users or other roles

**Why is role based access control more scalable than discretionary or mandatory access control?**

it provides for defining and maintaining roles

# Vocabulary Terms

* Authorization :Authorization is the process of giving someone permission to do or have something.
* Role Based Access Control: is an approach that uses the job functions performed by individual users within the organization to determine their appropriate access levels
* Capabilities: capabilities is what a person has the ability or knowledge to do

# Preview


* Which 3 things had you heard about previously and now have better clarity on?

  role based access control

* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

  role based access control

* What are you most excited about trying to implement or see how it works?

  Capabilities

# Preparation Materials

**Event Driven Programming**

Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.

Every time you interact with a webpage through it’s user interface, an event is happening. When you click a button a click event is triggered. When you press a key a keydown event is triggered. These events have associated functions that, when triggered, are executed to make a change to the user interface in some way

Event-Driven Programming makes use of the following concepts:

* An Event Handler is a callback function that will be called when an event is triggered.
* A Main Loop listens for event triggers and calls the associated event handler for that event.

EventEmitter
Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away. Of course, creating our own version of EventEmitter wouldn’t be much of a challange, and in fact there are several modules published on npm such as EventEmitter2 and EventEmitter3 which promise a faster performance than the native EventEmitter.

Those are both worth checking out if your project needs to run faster than EventEmitter will allow. They are both built to allow for syntax that is almost identical to what we’ll use for EventEmitter so learning one will make it easy to work with all of them.

We access the EventEmitter class through the events module. Once imported we’ll need to create a new object from the class to start using it.

**Node docs: events**

Much of the Node.js core API is built around an idiomatic asynchronous event-driven architecture in which certain kinds of objects (called "emitters") emit named events that cause Function objects ("listeners") to be called.