# Read-27, Code 401, 2 May 2021

## Props and State

### Review and Discussion

1. Does a deployed React application require a server?
   No you don't need a server for a deployed version of your
   Rect App.

2. Why do we prefer to test a React application at the behavior rather than the unit level?
   I think from my research that not the case all the time so if you have a form you need to test it as unit not it just been rendered.

3. What does npm run build do?
   When a user visits your site, each of your files will require an additional HTTP request, making your site slower to load. So to remedy this, you can create a “build” of our app, which merges all your CSS files into one file, and does the same with your JavaScript.

4. Describe the actual composition / architecture of a React application
   Components are often described as “just functions” but in our view they need to be more than that to be useful. In React, components describe any composable behavior, and this includes rendering, lifecycle, and state. Some external libraries like Relay augment components with other responsibilities such as describing data dependencies. It is possible that those ideas might make it back into React too in some form.

### Vocabulary Terms

- BDD: Behavior-driven development is an extension of test-driven development: development that makes use of a simple, domain-specific scripting language (DSL). These DSLs convert structured natural language statements into executable tests. The result is a closer relationship to acceptance criteria for a given function and the tests used to validate that functionality. As such it is a natural extension of TDD testing in general.

- Acceptance test: is way of writing acceptance criteria by giving examples of how software should behave in different scenarios. They are written in a standard format that promotes clarity, as well as allowing easy integration with automated testing.

- Mounting: is the phase in which our React component mounts on the DOM (i.e., is created and inserted into the DOM). This method is called just before a component mounts on the DOM or the render method is called. After this method, the component gets mounted.

- Build: creates a build directory with a production build of your app. Inside the build/static directory will be your JavaScript and CSS files. Each filename inside of build/static will contain a unique hash of the file contents

### Preview

1. Which 3 things had you heard about previously and now have better clarity on?
   Component, Single Page Applications, UI frameworks.

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   How to use funciton instead of classes, writing tests.

3. What are you most excited about trying to implement or see how it works?
   How to link a server to a react app.

### Materials

- setState
  React components with state render UI based on that state. When the state of components changes, so does the component UI.
  `setState()` is the only way to update state after the initial state setup.

- Handling Events
  Handling events with React elements is very similar to handling events on DOM elements.

  Regular Html:

  ```html
  <button onclick="activateLasers()">Activate Lasers</button>
  ```

  React:

  ```jsx
  <button onClick={activateLasers}>Activate Lasers</button>
  ```

- Forms
  Handling forms is about how you handle the data when it changes value or gets submitted.

  In HTML, form data is usually handled by the DOM.

  In React, form data is usually handled by the components.

  When the data is handled by the components, all the data is stored in the component state.

  You can control changes by adding event handlers in the onChange attribute

- State and lifeCycle
  Lifecycle of Components
  Each component in React has a lifecycle which you can monitor and manipulate during its three main phases.

  The three phases are: Mounting, Updating, and Unmounting.

  Mounting
  Mounting means putting elements into the DOM.

  The componentDidMount() method is called after the component is rendered.

  This is where you run statements that requires that the component is already placed in the DOM.
  The next phase in the lifecycle is when a component is updated.

  A component is updated whenever there is a change in the component's state or props

- Component and Props:
  A component is an independent, reusable code block which divides the UI into smaller pieces.
  Their are two types of them:
  Function and Class Components
  The simplest way to define a component is to write a JavaScript function:

  ```js
  function Welcome(props) {
    return <h1>Hello, {props.name}</h1>;
  }
  ```

  Props: “props” (which stands for properties) object argument with data and returns a React element.

  ```js
  class Welcome extends React.Component {
    render() {
      return <h1>Hello, {this.props.name}</h1>;
    }
  }
  ```

- Testing
  Basically, React Testing Library (RTL) is made of simple and complete React DOM testing utilities that encourage good testing practices
  So rather than dealing with instances of rendered React components, your tests will work with actual DOM nodes. The utilities this library provides facilitate querying the DOM in the same way the user would. Finding form elements by their label text (just like a user would), finding links and buttons from their text (like a user would). It also exposes a recommended way to find elements by a data-testid as an "escape hatch" for elements where the text content and label do not make sense or is not practical.

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-27)
