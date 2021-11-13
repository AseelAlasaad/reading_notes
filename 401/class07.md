
# Review, Research, and Discussion

*  Register your application to get a client_id and client_secret
*  Ask the client if they want to sign in via a third party
*  Redirect to a third party authentication endpoint
*  Make a request to the access token endpoint
*  Receive access token
*  Make a request to a third-party API endpoint  
*  Receive authorization code


**What can you do with an authorization code?**

An authorization code is an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space.
The authorization code is a temporary code that the client will exchange for an access token

**What can you do with an access token?**


Access tokens are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user's data

**What’s a benefit of using OAuth instead of your own basic authentication?**

OAuth is an authentication protocol that allows you to approve one application interacting with another on your behalf without giving away your password.
OAuth  most secure flow because you can authenticate the client to redeem the authorization grant, and tokens are never passed through a user-agent. 
OAuth doesn't share password data but instead uses authorization tokens to prove an identity between consumers and service providers.

# Vocabulary Terms

* client_id: The client_id is a public identifier for apps,It must also be unique across all clients that the authorization server handles.
* client secret:A client secret is a secret known only to your application and the authorization server,It protects your resources by only granting tokens to authorized requestors. Protect your client secrets and never include them in mobile or browser-based apps.

* Authentication Endpoint:  is a security mechanism designed to ensure that only authorized devices can connect to a given network, site or service.

* Access Token Endpoint: 
A request to the token endpoint is used to exchange an authorization code for an access token. Requests to the token endpoint are authenticated using client credentials through either basic authentication or by including them as post parameters depending on the clients configuration.

* API Endpoint: URL that enables the API to gain access to resources on a server
* Authorization Code:An authorization code is an alphanumeric password that authorizes its user to enter information into a security-protected space
* Access Token:The access token represents the authorization of a specific application to access specific parts of a user's data.


# Preview

**Which 3 things had you heard about previously and now have better clarity on?**

API Endpoint

**Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

Authentication Endpoint

**What are you most excited about trying to implement or see how it works?**

API Endpoint

# Preparation Materials

**JWTs Explained** & **Intro to JWT**

What is JSON Web Token?

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.JWTs can be signed using a secret

Although JWTs can be encrypted to also provide secrecy between parties, we will focus on signed tokens. Signed tokens can verify the integrity of the claims contained within it

**What is the JSON Web Token structure?**

In its compact form, JSON Web Tokens consist of three parts separated by dots (.), which are:

* Header
* Payload
* Signature

**Are JWTs Secure?**

JWTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don't know the private key, you can't change it. Otherwise, the receiver will notice that the signature won't match anymore.

![jwt](https://i.stack.imgur.com/bOHqZ.png)   

![jwt](https://i.stack.imgur.com/IIsJ3.png)






