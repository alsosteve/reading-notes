# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 401

# Read: 03 - Express REST API

## Reasons to use custom middleware:
1. Authentication
2. Logging data
3. security

## True or false: The route handler is middleware?
False

## In what ways can a middleware function end the process and send data to the browser?
You can send a 404 status to end the process.

## At what point in the request lifecycle can you “inject” middleware?
When the request reaches the server.

## What can cause express to error with “Request headers sent twice, cannot start a second response”

## Vocab:

Middleware : Software which lies between an operating system and the applications running on it.

Request Object: The main entry point for an application to issue a request to the Library.

Response Object: The response returned after making a request.

Application Middleware: 

Routing Middleware: The way in which the client requests are handled by the application endpoints.

Test Driven Development: The practice of creating tests before developing the actual code. 

Behavioral Testing:  Testing of the external behaviour of the program.