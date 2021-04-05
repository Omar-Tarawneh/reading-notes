# Read-07, Code 401, 5 April 2021

## Order of Access Token

- Receive access token
- Make a request to the access token endpoint
- Receive authorization code
- Ask the client if they want to sign in via a third party
- Make a request to a third-party API endpoint
- Redirect to a third party authentication endpoint
- Register your application to get a client_id and client_secret

## Authoriztion Uses

Authoriztion code can be used to set privilages to a user, or enter information or modify them.

## Access Tokens Uses

We can use it to strict which part of our data the user or server Can access it.

## OAuth vs Basic Authentication

It's better than the basic Auth because it allows limited access to the user's data and allows accessing when authorization tokens expire.

## Vocabulary

- Client ID: Is used to identify the application. As per oAuth standard you need both Client ID & Client Secret along with user credentials to generate an access token.

- Client Secret: is a secret used by the OAuth Client to Authenticate to the Authorization Server. The Client Secret is a secret known only to the OAuth Client and the Authorization Server. Client Secret must be sufficiently random to not be guessable.

- Authentication Endpoint: is an authentication mechanism used to verify the identity of a network's external or remote connecting device.

- Token Endpoint is an HTTP endpoint that micropub clients can use to obtain an access token given an authorization code.

- API endpoint: is a point at which an application program interface connects with the software program.

- Authorization Code: is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server where the user gets a chance to see what the information the client is requesting, and approve or deny the request.

- Access Token: is an object encapsulating the security identity of a process or thread.

## Preview

- Authintication, Authorization, and basic Auth in.

- Acess Token, OAuth, Bearer

- I really like the working with Classes and async function

## JWTs

JSON Web Token (JWT) defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

### whend to use it?

- Authorization
- Information Exchange

In authentication, when the user successfully logs in using their credentials, a JSON Web Token will be returned. Since tokens are credentials, great care must be taken to prevent security issues. In general, you should not keep tokens longer than required.

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-07)
