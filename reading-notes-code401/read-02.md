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
