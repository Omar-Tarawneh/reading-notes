# Read-10, Code 401, 7 April 2021

## Discussion

1. Why is access control important?
   Access control is important because it is a valuable security technique that can be used to regulate who or what can view or use any given resource.

2. Describe an application that would need access control.
   Our graduation project in 301 that have a login and sign up the access control would fit into it very well actually.

3. What is a role used for?
   To set privileges to a ceratin users or the team members.

4. Why is role based access control more scalable than discretionary or mandatory access control?
   For most business applications, RBAC is superior to ACL in terms of security and administrative overhead. ACL is better suited for implementing security at the individual user level and for low-level data, while RBAC better serves a company-wide security system with an overseeing administrator.

## Vocaabulary Terms

- Authorization: is a security mechanism to determine access levels or user/client privileges related to system resources.

- Role Based Access Control: s a policy-neutral access-control mechanism defined around roles and privileges.

- Capability: is the ability to perform or achieve certain actions or outcomes.

## Preview

1. Authorization & Authentication, RBAC, Stack & Queue

2. Sockit io, Firebase, React js

3. OAuth2 is really good actually I can't wait to try it in my projects.

## Event-Driven Programming in Node.js

Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.

For better demonstration the Web browser is a set of events the client interact with - click event is triggered.

### EDP Concept

- An Event Handler is a callback function that will be called when an event is triggered.
- A Main Loop listens for event triggers and calls the associated event handler for that event.

#### EDP Example in Node.js

Imagine we’re creating a chat room. We want to alert everyone when a new user joins the chat room. We’ll need an event listener for a userJoined event. First, we’ll write a function that will act as our event listener, then we can use EventEmitters on method to set the listener.

```javascript
const EventEmitter = require('events').EventEmitter;
const chatRoomEvents = new EventEmitter();

function userJoined(username) {
  // Assuming we already have a function to alert all users.
  alertAllUsers('User ' + username + ' has joined the chat.');
}

// Run the userJoined function when a 'userJoined' event is triggered.
chatRoomEvents.on('userJoined', userJoined);
```

so When a user join we will trigger this function.

```javascript
function login(username) {
  chatRoomEvents.emit('userJoined', username);
}
```

[GitHub-Link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-11)
