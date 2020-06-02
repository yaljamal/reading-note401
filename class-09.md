# API Server

## press: Router Parameters

* Parameters in routes is `app.get('/places/:city', function)` 
* middleware on any route `app.get('/places/:city', getZip, function)` 
* middleware on every request `app.use(getZip)` 

## Sub Documents in Mongoose

* Subdocuments are documents embedded in other documents.

 In Mongoose, this means you can nest schemas in other schemas.
 Mongoose has two distinct notions of subdocuments: arrays of subdocuments and single nested subdocuments.

## What is a Subdocument?

Subdocuments are similar to normal documents. Nested schemas can have middleware, custom validation logic, virtuals, and any other feature top-level schemas can use. The major difference is that subdocuments are not saved individually, they are saved whenever their top-level parent document is saved.
