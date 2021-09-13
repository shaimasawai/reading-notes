# **APIs**
## *What is a REST API?*

An API is a set of definitions and protocols for building and integrating application software. It’s sometimes referred to as a contract between an information provider and an information user—establishing the content required from the consumer (the call) and the content required by the producer (the response). For example, the API design for a weather service could specify that the user supply a zip code and that the producer reply with a 2-part answer, the first being the high temperature, and the second being the low.  

In other words, if you want to interact with a computer or system to retrieve information or perform a function, an API helps you communicate what you want to that system so it can understand and fulfill the request. 

You can think of an API as a mediator between the users or clients and the resources or web services they want to get. It’s also a way for an organization to share resources and information while maintaining security, control, and authentication—determining who gets access to what. 

Another advantage of an API is that you don’t have to know the specifics of caching—how your resource is retrieved or where it comes from.

Regular expressions (regex or regexp) are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern (i.e. a specific sequence of ASCII or unicode characters).
Fields of application range from validation to parsing/replacing strings, passing through translating data to other formats and web scraping.
One of the most interesting features is that once you’ve learned the syntax, you can actually use this tool in (almost) all programming languages ​​(JavaScript, Java, VB, C #, C / C++, Python, Perl, Ruby, Delphi, R, Tcl, and many others) with the slightest distinctions about the support of the most advanced features and syntax versions supported by the engines).
Let’s start by looking at some examples and explanations.
``
^The        matches any string that starts with The -> Try it!
end$        matches a string that ends with end
^The end$   exact string match (starts and ends with The end)
roar        matches any string that has the text roar in it````




```
\d   matches a single character that is a digit -> Try it!
\w   matches a word character (alphanumeric character plus underscore) -> Try it!
\s   matches a whitespace character (includes tabs and line breaks)
.    matches any character ->
```

The most popular type of web API is a Representational state transfer API or RESTful API for short. To be brief, it follows an architecture that uses predefined and stateless operations to access web resources.

Using web APIs requires the use of HTTP requests. Different types of requests include GET, POST, DELETE, PATCH, etc. If you have written some code and it needs to communicate with code somewhere else, it will send an HTTP request over the internet. Next, let’s discuss the HTTP request types just mentioned. You will notice that the types are matched to verbs that are similar to their function:

* GET: Used to request data from an endpoint
* POST: Sends data to an endpoint
* DELETE: Remove data from an endpoint.
* PATCH: Update a record or data value at an endpoint.
These types of interactions are external from the local environment, and therefore, the APIs that are providing the data or services are called external APIs. It is difficult to fathom how useful it is to have the capability to access external APIs for various data and services.
As previously mentioned, external APIs offer data, services, or both. Having access to the API can be valuable, therefore, you may need to buy a subscription to use it. Don’t worry, there are still plenty of free APIs.

Furthermore, the hypothetical external API does not have unlimited resources, so letting software call the API an unlimited amount of times at no cost could render it useless. Consequently, API providers will issue secret API-keys to monitor usage over time. Using RapidAPI allows the developer to only deal with one key (RapidAPI’s key), otherwise, developers would need to have API-keys for all of their APIs. Most of the time API-keys need to be kept secret, however, some services will issue public API keys.

Soon we will learn how to use the RapidAPI dashboard to simplify our understanding of how these parts work together, but first, let’s talk about React!
