In Express, 
# the .use() method  

## Provided by the express module.  
The implementation of .use() is a simple function:  
### adds a middleware function to an internal array of middleware functions.  
When a request is received, Express processes the middleware functions in the order in which they were added, calling each function in turn with the req, res, and next objects.

Here is a simplified version of the .use() function in Express _under the hood_:

        const express = require('express');
        const app = express();

        app.middleware = [];

        app.use = function(fn) {
          this.middleware.push(fn);
        };

        app.handle = function(req, res) {
          let i = 0;

          function next() {
            const fn = app.middleware[i++];
            if (!fn) {
              return;
            }
            fn(req, res, next);
          }

          next();
        };

        app.listen = function(port) {
          // code to start the HTTP server and listen for incoming requests
        };