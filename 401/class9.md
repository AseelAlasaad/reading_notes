# Reading: Authorization/Authentication


# Review, Research, and Discussion


**What header(s) are used in authentication and authorization**


In basic HTTP authentication, a request contains a header field in the form of Authorization, where credentials is the Base64 encoding of ID and password joined by a single colon.

Proxy-Authenticate response headers define the authentication method that should be used to gain access to a resource.

**What is safe to put into a JWT**

 ID Tokens 

 Access Tokens


**How are JWTs validated**


Check signature. The last segment of a JWT is the signature, which is used to verify that the token was signed by the sender and not altered in any way.


# Vocabulary Terms


* RBAC : role-based access control
* User Roles: 
User Roles give Administrators the ability to control what users can do within the system
* JWT Token: is a JSON encoded representation of a claim(s) that can be transferred between two parties.

# Preview

**Which 3 things had you heard about previously and now have better clarity on?**

JWT

RBAC

ACL

**Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

RBAC

**What are you most excited about trying to implement or see how it works?**
ACL
