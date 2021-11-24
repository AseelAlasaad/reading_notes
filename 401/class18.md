# Readings: AWS: API, Dynamo and Lambda

# Review, Research, and Discussion

* What are serverless functions?

 serverless function is a programmatic function written by a software developer for a single purpose

 * If you were to create a system that emulated Lambda functions, how would you do it?

 When starting designing, and building serverless functions, you might wonder how to deploy your function into the cloud. With AWS, there are some ways we can deploy, test and invoke your function:

Using the AWS Console Management: we can create Lambda function, upload code, add triggers, and test your Lambda function manually

* Describe how a CDN works

 CDN is a network of servers that distributes content from an “origin” server throughout the world by caching content close to where each end user is accessing the internet via a web-enabled device.

  content delivery network (CDN) refers to a geographically distributed group of servers which work together to provide fast delivery of Internet content. A CDN allows for the quick transfer of assets needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

  
# Term

* Serverless Functions: serverless function is a programmatic function written by a software developer for a single purpose
* Cloud Storage: is a cloud computing model that stores data on the Internet through a cloud computing provider 
* CDN: CDN is a network of servers that distributes content from an “origin” server throughout the world by caching content close to where each end user is accessing the internet via a web-enabled device.


# Preview


* Which 3 things had you heard about previously and now have better clarity on?

 Cloud Storage
* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

 Serverless Functions
* What are you most excited about trying to implement or see how it works?

 Serverless Functions

# Amazon API Gateway

Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

How does API Gateway work?

API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends. It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services. It can also generate API references from your definitions and make them available to your users as API documentation.

# What is DynamoDB?

DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS). 

How it works

Amazon DynamoDB is a fully managed, serverless, key-value NoSQL database designed to run high-performance applications at any scale. DynamoDB offers built-in security, continuous backups, automated multi-region replication, in-memory caching, and data export tools.