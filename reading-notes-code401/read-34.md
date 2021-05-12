# Read-33, Code 401, 11 May 2021

## `<login />` and `<Auth />`

### Discussion

1. Why is the Context API useful?
   is a way for a React app to effectively produce global variables that can be passed around. This is the alternative to "prop drilling" or moving props from grandparent to child to parent, and so on. Context is also touted as an easier, lighter approach to state management using Redux.

2. Can a component outside of a provider get its context?
   React context is available only when the UI is available. This means that on background tasks you can't access it. But that doesn't mean that you can't access it "outside" of components.

3. What are some common use cases for using the Context API?

   - Themes. The ability to set the theme is one of the best UX. ...
   - Multilingual application. To implement multiple languages in app we have to change the text in every component and replace with the translated text. ...
   - Authorisation: setting the user role and info.

4. Describe "Context Hell"
   When using the context API, splitting global state properties so as not to share a “god object” creates “Context hell,” a layer of countless contexts wrapping your React application

### Vocabulary

- global state: provides a way to pass data through the component tree having to pass props down manually at every level, managing state in multiple components that are not directly connected

- global context: Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user,

- provider: Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes. The Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers.

- consumer: A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component.

### Preview

#### Role-Based Access Control (RBAC)

Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

Advantages from RBAC:

- Reducing administrative work and IT support.
- Maximizing operational efficiency
- Improving compliance.

To See:

- [react-cookies](https://www.npmjs.com/package/react-cookies).
- [react-cookie](https://www.npmjs.com/package/react-cookie)

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-34)
