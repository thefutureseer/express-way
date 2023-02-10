# req (request) object 
## incoming HTTP request 
### Properties and Mehods sent from client (u.i.) to server

The req object is a representation of an incoming 
HTTP request in an Express application. It contains 
information about the request, such as the URL, headers, 
query parameters, and any data sent in the request body.

Here is a list of popular properties and methods available 
on the req object in an Express application:

### Lets start with:
PROPERTIES (accessed using dot notation):

1. req.baseUrl: 
the base URL for the request, if the application is 
mounted at a path.

2. req.body: 
>an object containing the request body parsed from 
JSON, URL encoded, or any other body parser middleware added 
to the application. 

>It is used to access the data sent in a POST or PUT request, for example to create or update a resource in a REST API. However, the contents of req.body are not automatically populated. To access the contents of the request body, you must use a middleware such as body-parser that parses the incoming request and populates the req.body property.

3. req.cookies: 
an object containing the cookies sent in the request.

4. req.fresh: 
a Boolean indicating whether the request is "fresh", 
meaning it has not been modified since the client last 
requested it.

5. req.hostname: 
the hostname of the request.

6. req.ip: 
the IP address of the client making the request.

7. req.ips: 
an array of IP addresses from the client making the request, 
if the application is behind a proxy.

8. req.method: 
>is a string that represents the HTTP method of the incoming request, such as GET, POST, PUT, DELETE, etc. This property is used to determine the type of operation being performed in the request, for example to determine if a request is a GET or a POST. With the information in req.method, you can define different behavior for different HTTP methods in your Express application.

9. req.originalUrl: 
the original URL of the request, including the query string.

10. req.params: 
> an object that contains the values of any parameters in the URL path. 
> For example, in a route defined as /users/:id, the id value can be accessed through req.params.id. This property is commonly used to access URL path parameters, such as the value of an ID in a REST API endpoint.

11. req.path: 
> A string that represents the URL path of the incoming request. This property is used to determine the resource being requested in a REST API, for example to determine if a request is for the /users endpoint or the /users/:id endpoint.
If the URL for the incoming request is https://www.example.com/users/123, req.path would contain the value /users/123.

12. req.protocol: 
the protocol of the request (e.g., 'http' or 'https').

13. req.query: 
>an object containing the values of any query _string_ parameters in the URL. For example, in a URL like /users?sort=desc, the value of the _sort_ query string parameter can be accessed through req.query.sort. This property is commonly used to access query string parameters, such as the values of filters or sorting criteria in a REST API endpoint.

14. req.route: 
the route object for the current request, if a matching route was found.

15. req.secure: 
a Boolean indicating whether the request was made over a 
secure connection (e.g., HTTPS).

16. req.signedCookies: 
an object containing signed cookies sent in the request.

17. req.xhr: 
a Boolean indicating whether the request was made via an XMLHttpRequest (i.e., an AJAX request).

18. req.headers: 
> an object that contains the HTTP headers for the incoming request, which can provide information about the request such as the type of request, the user-agent of the client making the request, and any authentication information.

used to access request headers, such as the Accept-Language or Authorization headers.


## METHODS (called using dot notation):

### Popular methods:

1. req.accepts([types]): 
>returns the first content-type that is accepted by the client, as indicated by the "Accept" header in the incoming request. The req.accepts method takes an array of content-types as its argument, and returns the first content-type in the array that is acceptable to the client, or false if none of the content-types are acceptable.

2. 
req.acceptsCharsets([charsets]): 
returns the first accepted charset in the specified array, or 
false if no match is found.

3. 
req.acceptsEncodings([encodings]): 
returns the first accepted encoding in the specified array, or 
false if no match is found.

4. 
req.acceptsLanguages([languages]): 
returns the first accepted language in the specified array, or 
false if no match is found.

5. 
req.get(field): 
returns the value of the specified header field.

6. 
req.is(type): 
returns true if the specified type is acceptable, otherwise false.
