# Readings: CRUD

**What is a status code 100?**

everything so far is OK and that the client should continue with the request or ignore it if it is already finished.

**What is a status code 200?**

These are the success codes. They tell the client that its request was accepted

**What is a status code 300?**

These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore.

**What is a status code 400?**

These are the client error codes. They are all about invalid requests a client sent to a server.There are several causes to this, timeouts, wrong URI, missing authentication, etc.


**What is a status code 500?**

These are the server error codes. Often they indicate problems with overwhelmed servers ,sometimes they can be directly related to client requests.

**What is a status code 202?**

(HTTP) 202 Accepted response status code indicates that the request has been accepted for processing, but the processing has not been completed.


**What is a status code 308?**

308 Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore.

**What code would you use if an update didn’t return data to a client?**

204 No Content - A proper code for updates that don’t return data to the client

**What is the ‘Forbidden’ status code?**

403 Forbidden ,The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

**What is the difference beween PUT and PATCH?**

PUT is a method of modifying resource where the client sends data that updates the entire resource. It is used to set an entity’s information completely.

PATCH applies a partial update to the resource.This means that you are only required to send the data that you want to update, and it won’t affect or change anything else.