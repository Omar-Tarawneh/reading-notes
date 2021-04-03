# Read-06, Code 401, 4 April 2021

## Singleton

A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance.

A single object used across systems remains constant and needs to be defined only once rather than many times.

## Singleton with Node.js

basically we create and instance of a module inside another class or model inside the **singleton** and we use that instance across all of our app for example:

```javascript
class Logger {
  constructor() {
    this.logs = [];
  }

  get count() {
    return this.logs.length;
  }

  log(message) {
    const timestamp = new Date().toISOString();
    this.logs.push({ message, timestamp });
    console.log(`${timestamp} - ${message}`);
  }
}

class Singleton {
  constructor() {
    if (!Singleton.instance) {
      Singleton.instance = new Logger();
    }
  }

  getInstance() {
    return Singleton.instance;
  }
}

module.exports = Singleton;
```

we create a logger for our app and get an instance of it inside the singleton then we export it to all other file.

## Create Middlewares like Express Uses

- Define the instance of the middleware to use it globaly
- Define where to use it at which request/response
- when the middleware should stop the request and throw the error.

## Vocabulary

- Router Middleware: The express.Router() function is used to create a new router object. This function is used when you want to create a new router object in your program to handle requests.

- Dynamic Module Loading: Dynamic loading is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory.

- Singleton Pattern: A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance

- CRUD --> REST: ![crud-rest](https://itexamanswers.net/wp-content/uploads/2020/01/2020-10-25_185415.jpg)

- Mock testing: is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules.

## Preview

- Middlewares, Data Structure and Algorithms, and noSQL databases.

- Authontication and more about mongoDB.

- Singleton I want to try it later.

### Password

It's very very likely to store all password in the database encrypted because it's the first firewall that protect you from hacker.

Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible.

### Basic access Authentication

HTTP Basic authentication implementation is the simplest technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages; rather, HTTP Basic authentication uses standard fields in the HTTP header.

## Bcrypt

Simply it's a Node package to help you hash passwords in your app.

example:

```javascript
async function checkUser(username, password) {
  //... fetch user from a db etc.

  const match = await bcrypt.compare(password, user.passwordHash);

  if (match) {
    //login
  }

  //...
}
```

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-06)
