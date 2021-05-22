# Read-36, Code 401, 22 May 2021

## Redux

### Discussion

1. What are the advantages of storing tokens in “Cookies” vs “Local Storage”
   Option 1: Store your access token in localStorage : prone to XSS. Option 2: Store your access token in httpOnly cookie: prone to CSRF but can be mitigated, a bit better in terms of exposure to XSS. Option 3: Store the refresh token in httpOnly cookie: safe from CSRF, a bit better in terms of exposure to XSS.

2. Explain 3rd party cookies.
   Third-party cookies are cookies that are set by a website other than the one you are currently on. For example, you can have a "Like" button on your website which will store a cookie on a visitor's computer, that cookie can later be accessed by Facebook to identify visitors and see which websites he visited.

3. How do pixel tags work?
   A tracking pixel (also called 1x1 pixel or pixel tag) is a graphic with dimensions of 1x1 pixels that is loaded when a user visits a webpage or opens an email. ... The tracking pixel URL is the memory location on the server. When the user visits a website, the image with the tag is loaded from this server

### Vocabulary

- cookies: Cookies are text files with small pieces of data — like a username and password — that are used to identify your computer as you use a computer network. Specific cookies known as HTTP cookies are used to identify specific users and improve your web browsing experience.

- authoriztion: Authorization is a process by which a server determines if the client has permission to use a resource or access a file. Most of the web pages on the Internet require no authentication or authorization.

- access control: Access control is a fundamental component of data security that dictates who's allowed to access and use company information and resources. Through authentication and authorization, access control policies make sure users are who they say they are and that they have appropriate access to company data.

- conditional rendering: Conditional rendering is a term to describe the ability to render different user interface (UI) markup if a condition is true or false. In React, it allows us to render different elements or components based on a condition. This concept is applied often in the following scenarios: Rendering external data from an API.

### Preview

1. Which 3 things had you heard about previously and now have better clarity on?
   Context API, Axios, Bootstrap.

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   implement Redux in the web app.

3. What are you most excited about trying to implement or see how it works?
   Redux.

### Redux explained

Redux is a pattern and library for managing and updating application state, using events called “actions”.

It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test. On top of that, it provides a great developer experience.

Redux helps you manage “global” state - state that is needed across many parts of your application.

#### Benefits

- Technical benefits of using Redux.
- Predictable states. The state is always predictable in Redux. ...
- Ease in maintenance. ...
- Debugging is easy. ...
- Testing code is simple. ...
- Server rendering. ...
- Vast developer tools available. ...
- Great supportive community. ...
- Reusable Code.

#### Prupose

Redux is a predictable state container designed to help you write JavaScript apps that behave consistently across client, server, and native environments and are easy to test. While it's mostly used as a state management tool with React, you can use it with any other JavaScript framework or library.

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-36)
