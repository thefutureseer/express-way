# Important things about express.js 
express-way

>  Whatever you read here and can understand is fine. 
>  We can build on that later.
>>  -Dr Daniel Tannehill

##1
Routing: 
The ability to define and manage application routes, allowing you to map URLs to specific behavior in your application.

##2
Middleware: 
The ability to use middleware functions to manipulate incoming requests and outgoing responses in your application.

#### Middleware functions: 

  Express provides a middleware system that allows you to execute arbitrary code between the time a request is received and the time a response is sent. This allows you to implement common functionality, such as logging, authentication, and data validation, in a reusable and modular way.

-   write your own:
    You can also write your own custom middleware functions to meet the specific needs of your application.

-   Body Parser: 
    A middleware that parses the incoming request body and makes it available in the request object.

-   Cookie Parser: 
    A middleware that parses incoming cookies and makes them available in the request object.

-   CORS (Cross-Origin Resource Sharing): 
    A middleware that implements cross-origin resource sharing, which allows requests to be made to a server from a different origin.

-  CSRF (Cross-Site Request Forgery): 
   A middleware that provides protection against cross-site request forgery attacks.

-   Helmet: 
    A middleware that sets HTTP headers for security purposes, such as setting the X-XSS-Protection header to prevent cross-site scripting attacks.

-   Morgan: 
    A logging middleware that logs incoming requests and their response information.

-   Serve-Static: 
    A middleware that serves static files, such as images, stylesheets, and JavaScript files.

-   Session: 
    A middleware that provides session management, allowing you to store data across multiple requests from a single client.

-   Error handler: 
    A middleware that provides custom error handling, allowing you to specify how your application should respond to errors.

-   Compression: 
    A middleware that compresses outgoing responses to reduce the amount of data that needs to be transmitted over the network.

##3 
Templating engines: 
Express provides support for using templating engines, which allow you to generate dynamic HTML content. This makes it easy to create views that can change based on the data available in your application.

##4
Templating: 
The ability to render dynamic HTML pages using templating engines, such as EJS, Pug, or Handlebars.

##5
Error handling: 
Built-in error handling mechanisms, such as handling 404 Not Found errors or 500 Internal Server Error responses.

##6
Custom error handling: 
Express provides the ability to define custom error handling middleware, which allows you to specify how your application should respond to errors. This makes it easy to implement meaningful error responses that are tailored to your specific needs.

##7
Serving static files: 
Built-in support for serving static files, such as images, CSS, and JavaScript files, from a specified directory.

##8
HTTP utility methods: 
Convenient HTTP utility methods for performing common HTTP tasks, such as sending JSON responses or redirecting users to another page.

##9
Third-party middleware: 
The ability to use a wide variety of third-party middleware to extend the functionality of your Express application.

##10
Body parsing: 
Express automatically parses incoming request bodies and makes the data available in the request object for easy access.

##11
Session management: 
Express provides easy-to-use session management capabilities, which allow you to store and retrieve user-specific data between requests.

##12
Query string parsing: 
Express provides automatic query string parsing, allowing you to easily access query string parameters in your routes.

##13
File uploads: 
Express provides support for handling file uploads, making it easy to receive and process files from clients.

##12
(Middleware from above) CORS (Cross-Origin Resource Sharing): 
Express provides built-in support for handling CORS, allowing your application to securely accept requests from other domains.

##13
Security: 
Express provides several security-related features, such as protection against cross-site scripting (XSS) attacks, cross-site request forgery (CSRF) protection, and others.

##14
API development: 
Express is a popular choice for building APIs, and provides several features that make it well-suited for API development, such as automatic JSON parsing, support for API versioning, and more.

##15
Routing with parameters: 
Express supports dynamic routing, which allows you to include variables in your route paths. This makes it easy to create routes that can respond to requests with different parameters, such as an id of a specific resource.

##16
Mounting middleware and routing functions: 
Express allows you to mount middleware and routing functions at specific paths, which provides fine-grained control over the flow of your application. This can be useful for organizing your application into smaller, more manageable parts.

##17
Redirection: 
Express provides a simple way to implement redirection in your application, which allows you to redirect users to different pages based on the status of their request.
