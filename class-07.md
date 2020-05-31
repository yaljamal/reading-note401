# Express

* it is has response ans reqest
* reqest (req.params.thing)

> thing this sent from the form 

* respons ( sending data back to the browser)

> it has methods like send() and status()

* Express Middleware

> Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. 

* Types of middleware: Application and Route
1. Application Middleware

 - Error Handling
 - Bringing in other routes
 - Applies Defaults
 - JSON, Body and Form Parsing
 - Runs on every request

2. Route Middleware

 * Dealing with specific things for a route

* CRUD Operations with REST and Express

 - CREATE => app.post('/resource')
 - READ => app.get('/resource')
 - UPDATE => app.put('/resource/:id')
 - DESTROY => app.get('/resource/:id') // delete

* how we can test the srever 

 supertest => this is will hit the routes as though your server was running, without actually starting it

* Third Party Middleware 

### Most Common :

 - body-parser : This is used to parse the body of requests which have payloads attached to them. To mount body parser (npm install --save body-parser)
 - cookie-parser :   (install --save cookie-parser)
 - express-session : It creates a session middleware with the given options

### SuperTest 

> it is using to test the server  to install it npm install supertest --save-dev 
