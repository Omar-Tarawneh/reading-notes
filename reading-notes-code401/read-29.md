# Read-29, Code 401, 4 May 2021

## Routing

## Discussion

1. Do child components have direct access to props/state from the parent?
   No, they don't have direct access for the parent state and props but can change them if you pass funciton to modifiy them.

2. When a component “wraps” another component, how does the child component’s output get rendered?
   They can by rendered using the `props.children` and the they will be rendered inside the `<Main/>` component.

3. Can a component, such as `<Content />`, which is a child also be used as a standalone component elsewhere in the application?
   Yes it can be used in another case that the hole idea of usability.

4. What trick can a parent use to share all props with it’s children?
   The parent can pass them directly to all children or pass a function to them to share all the states and props.

### Vocabulary

- props.children: props. children does is that it is used to display whatever you include between the opening and closing tags when invoking a component. A simple example: Here's an example of a stateless function that is used to create a component.

- Composition: is a pattern that can be used to break a complex component down to smaller components, and then composing those smaller components to structure and complete your application.

### Preview

1. Which 3 things had you heard about previously and now have better clarity on?
   Composition, Routing, class components.

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   Routing, composition, react-if

3. What are you most excited about trying to implement or see how it works?
   I want to use routing in react to render different pages.

### React Routing

React Routing is a package you need to install to use it.
For our purpose of use we gonna use the `<BrowserRouter>` and `<HashRouter>`
The `<BrowserRouter>` should be used when you have a server that will handle dynamic requests (knows how to respond to any possible URI), while the `<HashRouter>` should be used for static websites (where the server can only respond to requests for files that it knows about).

Usually it is preferable to use a `<BrowserRouter>`, but if your website will be hosted on a server that only serves static files, then the `<HashRouter>` is a good solution.

Example from React Router Dom Docs:

```js
import React from 'react';
import { BrowserRouter as Router, Switch, Route, Link } from 'react-router-dom';

export default function App() {
  return (
    <Router>
      <div>
        <nav>
          <ul>
            <li>
              <Link to="/">Home</Link>
            </li>
            <li>
              <Link to="/about">About</Link>
            </li>
            <li>
              <Link to="/users">Users</Link>
            </li>
          </ul>
        </nav>

        {/* A <Switch> looks through its children <Route>s and
            renders the first one that matches the current URL. */}
        <Switch>
          <Route path="/about">
            <About />
          </Route>
          <Route path="/users">
            <Users />
          </Route>
          <Route path="/">
            <Home />
          </Route>
        </Switch>
      </div>
    </Router>
  );
}

function Home() {
  return <h2>Home</h2>;
}

function About() {
  return <h2>About</h2>;
}

function Users() {
  return <h2>Users</h2>;
}
```

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-29)
