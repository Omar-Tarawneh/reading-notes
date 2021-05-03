# Read-28, Code 401, 3 May 2021

## Component Composition

### Review, Research and Discussion

1. Can a parent component access the state of a child component?
   In React we can access the child's state using Refs. we will assign a Refs for the child component in the parent component. then using Refs we can access the child's state.

2. What can be passed along in a prop variable?
   You can pass any Data type you want also you can pass functions.

3. How can a child component “know” the state of another component?
   By passing a funciton to these component and change the state accrodingly or just return it as it's.

### Vocabulary Terms

- component props: Properties which is object argument that conatains data or functions.

- component state: The state is an instance of React Component Class can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component.

- application state: In the simplest terms, it is a JavaScript object that represents the part of a component that can change

### Preview

1. Which 3 things had you heard about previously and now have better clarity on?
   Components, State, useState.

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   converting the class component to function components and other hooks.

3. What are you most excited about trying to implement or see how it works?
   I want to try the props the passing the functions.

### Perperation

#### React Recap

- Component Lifecycle
  A component can only be in one stage at a time. It starts with mounting and moves onto updating. It stays updating perpetually until it gets removed from the virtual DOM. Then it goes into the unmounting phase and gets removed from the DOM.

  The lifecycle methods allow us to run code at specific points in the component’s life or in response to changes in the component’s life.

- Update
  This phase is triggered every time state or props change. Like in mounting, getDerivedStateFromProps is called (but no constructor this time!).

- Unmounting
  Our component lived a good life, but all good things must come to an end. The unmounting phase is that last stage of the component lifecycle. When you remove a component from the DOM, React runs componentWillUnmount right before it gets removed. You should use this method to clean up any open connections such as WebSockets or intervals.

- Props Children
  It's recommended that you pass all element inside the component as `props.children`.
  Example:

  ```js
  function WelcomeDialog() {
    return (
      <FancyBorder color="blue">
        <h1 className="Dialog-title">Welcome</h1>
        <p className="Dialog-message">Thank you for visiting our spacecraft!</p>
      </FancyBorder>
    );
  }
  ```

- Inheritance
  As mentioned in the React Docs DON'T USE INHERITANCE it's not recommended because the props and companent give you all the flexibilities you need.

- React testing library
  In the example from the docs you basically render the component and try to test some behavior in it.
  Example from the Docs:

  ```js
  test('handles server error', async () => {
    server.use(
      rest.get('/greeting', (req, res, ctx) => {
        return res(ctx.status(500));
      })
    );

    render(<Fetch url="/greeting" />);

    fireEvent.click(screen.getByText('Load Greeting'));

    await waitFor(() => screen.getByRole('alert'));

    expect(screen.getByRole('alert')).toHaveTextContent(
      'Oops, failed to fetch!'
    );
    expect(screen.getByRole('button')).not.toHaveAttribute('disabled');
  });
  ```

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-28)
