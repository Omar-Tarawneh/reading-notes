# Read-07, Code 401, 5 April 2021

## Discussion

- Basic Authoriztion vs Bearer
  The Basic and Digest authentication schemes are dedicated to the authentication using a username and a secret (see RFC7616 and RFC7617).

  The Bearer authentication scheme is dedicated to the authentication using a token and is described by the RFC6750.

- JSON Web Token
  JSON Web Token is a standard used to create access tokens for an application. It works this way: the server generates a token that certifies the user identity, and sends it to the client.

- SECRET
  you need to keep secure and becarful not to push in github but it in .env file

## Vocabulary

- encryption: is the method by which information is converted into secret code that hides the information's true meaning.

- token: coded string used to securely transfer information over the web(between two parties).

- bearer: is an HTTP authentication scheme that involves security tokens called bearer tokens.

- secret: is the key you use to encode your token which need to be secure and private for secuarity.

- JSON Web Token: is used to send information that can be verified and trusted by means of a digital signature.

## Preview

1. Authonitication and Authorizaiton, Beare & Basic Auth, and Tokens and how to with these things

2. learn more about Auth in general and how to set previlages

3. how to use session and cookies

## RBAC

Role-based access control
is nothing more than the idea of assigning system access to users based on their role within an organization.

### RBAC benfits

With the proper implementation of RBAC, the assignment of access rights becomes systematic and repeatable. Further, it is much easier to audit user rights, and to correct any issues identified.

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-08)
