# Read-26, Code 401, 1 May 2021

## Component Based UI

### Discussion

1. Name 5 Javascript UI Frameworks (other than React)
   Angula, Vue, Ember, Svelte3 and Ext JS by Sencha.

2. What's the difference between a framework and a library?
   The technical difference between a framework and library lies in a term called inversion of control. When you use a library, you are in charge of the flow of the application. You are choosing when and where to call the library. When you use a framework, the framework is in charge of the flow.

### Vocabulary

- Rendering: Rendering refers to showing the output in the browser. The DOM establishes parent-child relationships, and adjacent sibling relationships, among the various elements in the HTML file.

- Templates: React templates are sets of ready-to-use parts of code built using React technology for the development of dynamic user interfaces

- State: The state is an instance of React Component Class can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component.

### Preview

1. Which 3 things had you heard about previously and now have better clarity on?
   Authintication & Authorization, UI framworks, React.

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   How to consume and API using React, how to render multibile pages in SPA.

3. What are you most excited about trying to implement or see how it works?
   how to style the components in React and how it will make different from the multi pages html.

### React Framework

Simple Hello World Example using react:

```javascript
import React, { Component } from 'react';
import logo from './logo.svg';
import './App.css';

class App extends Component {
  render() {
    return (
      <div className="App">
        <h1>Hello Wolrd!</h1>
      </div>
    );
  }
}

export default App;
```

Here, the first statement is used to include the react module, next we are creating a “App” Component by creating a “App” class that extends the Component class.

Inside of “App” class we have created a render method which is a part of React.Component class, it return a Hello World!” message enclosed in `<h1></h1>` tag.

#### JSX

In React, instead of using regular JavaScript for templating, it uses JSX. JSX is a simple JavaScript that allows HTML quoting and uses these HTML tag syntax to render subcomponents. HTML syntax is processed into JavaScript calls of React Framework. We can also write in pure old JavaScript.

example of JSX: `const element = <h1>Hello, world!</h1>;`

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-26)
