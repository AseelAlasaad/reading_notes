
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
* 





