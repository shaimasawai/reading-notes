# *HTTP Status Codes*
The HTTP specification defines many status codes we can use when responding to our clients. Some APIs only use the most basic codes and define their own error signaling mechanisms on top of it; others want to make full use of HTTPs collection of codes to tell their clients what’s going on. If you belong to the latter, this article is for you. This guide walks through the various CRUD operations and which status codes you should be using for clean API design.

## *HTTP Status Codes*
A status code is a number higher than 100 and smaller than 600 that is part of a HTTP response. The first digit defines the class of the status. A status code comes with a reason phrase. The code is for programmatic recognition the phrase is for humans to understand what happened.

## *Stus ClassesPermalink*
### 100 - 199
These are informational status codes; they usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. Like using a different protocol or telling the client that its request will fail before they start sending the body

### 200 - 299
These are the success codes. They tell the client that its request was accepted. In case of asynchronous processing of a request (202), this doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending.
### 300 - 399
These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore. This can have multiple reasons, be temporary or permanent, but the client has to issue a request to the new location.

## *UPDAT*
An update can be implemented with an HTTP PUT or PATCH method. The difference lies in the amount of data the client has to send to the backend.

PUT requires the client to send an entire representation of a resource to update it. (Replace the old one with the new one)

PATCH requires the client only send parts of the representation of the resource to update it. (Add, update or delete these parts in the old version)
## *DELETE*
The delete action can be implemented with the HTTP DELETE method.
**tus Codes**

200 OK - Some people think a delete function of any kind should return the deleted element, so a representation of the deleted element can be included in the response body.

204 No Content - The most fitting status code for this case. It’s better to reduce traffic and simply tell the client the deletion is complete and return no response body (as the resource has been deleted).

202 Accepted - If the deletion is asynchronous and takes some time, which is the case in distributed systems, it can be appropriate to return this code with some information or URL to tell the client when it will be deleted.
## *API Changes*
If our API lives long enough, sooner or later it will change its structure. It’s best practice to avoid breaking changes and the redirection class of status codes can help with this because some clients follow their Location header automatically.
## *Errors*
The next important part of an API is its errors. Many API frameworks use 500 and 404 status codes by default when something went wrong, but depending on the situation, often there are more descriptive ones.

500 means Internal Server Error, which can be anything from a missing header field the backend accessed without checking its existence to an unreachable third party service the backend wanted to call



