# Read-03, Code 401, 29 Mar 2021

## World Cases to Change

- Authentication
- Error Handling
- Data Modelling

## Route Handler is Middleware

False

## Middleware Ended the process

you can by throwing and error or you cant but a condition and not calling the next function

## Injecting the Middleware

the middleware is active when send a request and before calling the handler of the route - the callback function.

## Express Error

Calling the callback function twice, throwing an error before the response.

## Terms and definition

- Middleware
  function that process some data which is be called before the handler

- Request Object
  The req **object** represents the HTTP **request** and has properties for the **request** query string, parameters, body, HTTP headers, and so on.

- Response Object
  The res **object** represents the HTTP **response** that an **Express** app sends when it gets an HTTP request.
- Application Middleware
  Middleware that plays a role in the function of the application.

- Routing Middleware
  Middleware that plays a role in path routing.

- TDD
  **Test Driven Development (TDD)** is software development approach in which test cases are developed to specify and validate what the code will do.

- Behavioral Testing
  **Behavioural Testing** is a **testing** of the external **behaviour** of the program, also known as black box **testing**. It is usually a functional **testing**.

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-03)
