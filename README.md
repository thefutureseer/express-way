# Important things about express.js  
  

>  Whatever you read here and can understand is fine. 
>  We can build on that later.
>>  -Dr Daniel Tannehill

_NOTE_:  
Express.js is not all middleware. It is a web application framework for Node.js that provides a set of features and functions for building web applications. One of the key features of Express.js is its support for middleware, which are functions that can be used to manipulate incoming requests and outgoing responses. However, Express.js also includes other features, such as support for routing, templating, error handling, serving static files, body parsing, session management, and more.

## Middleware functions
Express provides a middleware system that allows you to execute arbitrary code between the time a request is received and the time a response is sent. This allows you to implement common functionality, such as logging, authentication, and data validation, in a reusable and modular way

-   write your own:  
    - You can also write your own custom middleware functions to 
    - meet the specific needs of your application.

-   Body Parser [express.bodyParser()]:  
    - A middleware that parses the incoming request body and makes - it available in the request object.

-   Cookie Parser [express.cookieParser()]:  
    - A middleware that parses incoming cookies and makes them : available in the request object.

-   CORS (Cross-Origin Resource Sharing):  
    - A middleware that implements cross-origin resource sharing,which allows requests to be made to a server from a different origin.

-   Morgan [express.morgan()]:  
    - A logging middleware that logs incoming requests and their response information.

-   Session [express.session()]:  
    - Express.js does not have built-in session management, but it provides a way to use middleware to handle sessions. There are many third-party middleware available, such as *express-session* , that can be used to add session management to an Express application allowing you to store data across multiple requests from a single client.

-   Error handler [express.errorHandler()]:  
    - A middleware that provides custom error handling, allowing you to specify how your application should respond to errors.

-   Compression [express.compress()]:  
    - A middleware that compresses outgoing responses to reduce the amount of data that needs to be transmitted over the network.


- Routing [express.Router()]
  - The ability to define and manage application routes, allowing you to map URLs to specific behavior in your application.

- Templating engines:  
  - Express provides support for using templating engines, which allow you to generate dynamic HTML content. This makes it easy to create views that can change based on the data available in your application.

- Templating  
- The ability to render dynamic HTML pages using templating engines, such as EJS, Pug, or Handlebars.

- Error handling  
- Built-in error handling mechanisms, such as handling 404 Not Found errors or 500 Internal Server Error responses, as well as the ability to define custom error handling middleware.

- Serving Static files [Serve-Static]  
- Built-in support for serving static files, such as images, CSS, and JavaScript files, from a specified directory.

- HTTP utility methods  
Convenient HTTP utility methods for performing common tasks, such as sending JSON responses or redirecting users to another page.

- Third-party middleware  
The ability to use a wide variety of third-party middleware to extend the functionality of your Express application

- Query string parsing [express.query()]  
Automatic query string parsing to easily access query string parameters in routes.

- File uploads  
Support for handling file uploads, making it easy to receive and process files from clients.

- Security:  
Express.js does not have built-in security features, but it provides support for security-related middleware like CORS (Cross-Origin Resource Sharing) for handling cross-domain requests and Helmet for setting security-related HTTP headers. Additionally, it provides features for body parsing and query string parsing, which can help prevent against certain types of attacks such as Cross-Site Scripting (XSS) and Cross-Site Request Forgery (CSRF) [express.csrf()]. However, it is still important to implement appropriate security measures for your application.

- API development  
Express is a popular choice for building APIs, and provides several features that make it well-suited for API development, such as automatic JSON parsing, support for API versioning, and more.

- Routing with parameters  
Supports dynamic routing, which allows you to include variables in your route paths. This makes it easy to create routes that can respond to requests with different parameters, such as an id of a specific resource.

- Mounting middleware and routing functions  
Ability to mount middleware and routing functions at specific paths for fine-grained control over the flow of the application.
This can be useful for organizing your application into smaller, more manageable parts.

- Redirection  
Express provides a simple way to implement redirection in your application, which allows you to redirect users to different pages based on the status of their request.  

- express.json()  
 - for parsing JSON request bodies

- express.urlencoded()  
- for parsing URL-encoded request bodies

- express.methodOverride()  
 - for allowing the use of HTTP methods such as PUT or DELETE in requests that use only POST and GET methods  

- express.timeout()  
 - for setting a timeout for incoming requests  
 
- express.basicAuth()  
 - for providing basic authentication for the application