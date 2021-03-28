# Read-02, Code 401, 28 Mar 2021

## Express

## Difference between PUT and PATCH

`PUT`: is a method of modifying resource where the client sends data that updates the entire resource.

`PATCH`: is a method to apply a partial update to the resource.

## Tools to mock an API development

1. [Postman](https://learning.getpostman.com/docs/postman/mock-servers/setting-up-mock/)
2. [Wiremock](http://wiremock.org/)
3. [Mockserver](https://www.npmjs.com/package/mockserver)

## Swagger vs APIDoc.js HTTP status Codes

**Swagger**
responses:
'200':
description: OK
'400':
description: Bad request. User ID must be an intand larger than 0.
'401':
description: Authorization information is missininvalid.
'404':
description: A user with the specified ID wasfound.
'5XX':
description: Unexpected error.

**APIDoc.js**
responce:
200: ok
400: bad request
404: not found
403: forbidden
500: server error

## SOAP vs REST

**SOAP**
stands for Simple Object Access Protocol,
It’s a messaging protocol for interchanging data in a decentralized and distributed environment, and it's returned data in XML format.
Mainly use for enterprise-level web services that require high security and complex transactions. APIs for financial services;

**REST**
stands for Representational State Transfer. It’s an architectural style that defines a set of recommendations for designing loosely coupled applications that use the HTTP protocol for data transmission.
Mainly used for public APIs and it's the most populat one.

## TDD

“Test-driven development”
refers to a style of programming in which three activities are tightly interwoven: coding, testing

It can be described by the following points:

- write a “single” unit test describing an aspect of the program
- run the test, which should fail because the program lacks that feature
- write “just enough” code, the simplest possible, to make the test pass
- “refactor” the code until it conforms to the simplicity criteria
- repeat, “accumulating” unit tests over time

## CI/CD

Continious Integration / Continious Doployment
is a coding philosophy and set of practices that drive development teams to implement small changes and check in code to version control repositories frequently.
It's the best practice because it addresses the misalignment between developers who want to push changes frequently, with operations that want stable applications.

- Web Server: A web server is a computer that runs websites. It's a computer program that distributes web pages as they are requisitioned. The basic objective of the web server is to store, process and deliver web pages to the users. This intercommunication is done using Hypertext Transfer Protocol (HTTP).

- Express: it's a node js framework, used for deveoloping backend web app and APIs

- Routes: is a mechanism where HTTP requests are routed to the code that handles them. To put simply, in the Router you determine what should happen when a user visits a certain page.

- WRRC: The request/response cycle traces how a user's request flows through the app.

[GitHub](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-02)
