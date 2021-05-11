# Read-33, Code 401, 11 May 2021

## Context API

### Discussion

1. Describe use cases for useMemo() and useReducer()

   - `useReducer` :
     `useReducer` takes three positional arguments — a reducer, its initial state, and a function that can return the initial state — let’s call it init for now. The final argument is optional. You can just pass in the initialState as is (e.g. {count: 0}), but if you want to operate on it in any way, I’d suggest using the init function.

     Best Case Use: is best used when you are dealing with a complex object where individual properties need to be operated on.

   - `useMemo` : useMemo is similar to useCallback except that instead of memoizing a function, it memoizes a value

2. Why do custom hooks need the use prefix?
   This convention is very important. Without it, we wouldn’t be able to automatically check for violations of rules of Hooks because we couldn’t tell if a certain function contains calls to Hooks inside of it

3. What do custom hooks usually do?
   Building your own Hooks lets you extract component logic into reusable functions.

4. Using any list of custom hooks, research and name one that you think will be useful in your applications
   `useMotion` — tracks state of device's motion sensor. Because it will fit very will in out final project.

5. Describe how a hook that fetches API data might work?
   example:

   ```js
   React.useEffect(() => {
     // side effect hook
     // call API with props.greeting parameter
     setTranslation(response.data.translation);
   }, [setTranslation]);
   ```

### Vocabulary

- reducer: Basically reducers are there to manage state in an application. For instance, if a user writes something in an HTML input field, the application has to manage this UI state (e.g. controlled components).

### React Context

Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

Guide from React docs:

first you need to create a context :

`const ThemeContext = React.createContext('light');`

```js
class App extends React.Component {
  render() {
    // Use a Provider to pass the current theme to the tree below.
    // Any component can read it, no matter how deep it is.
    // In this example, we're passing "dark" as the current value.
    return (
      <ThemeContext.Provider value="dark">
        <Toolbar />
      </ThemeContext.Provider>
    );
  }
}

// A component in the middle doesn't have to
// pass the theme down explicitly anymore.
function Toolbar() {
  return (
    <div>
      <ThemedButton />
    </div>
  );
}

class ThemedButton extends React.Component {
  // Assign a contextType to read the current theme context.
  // React will find the closest theme Provider above and use its value.
  // In this example, the current theme is "dark".
  static contextType = ThemeContext;
  render() {
    return <Button theme={this.context} />;
  }
}
```

in the example above we don't need to pass any props to the button to use the theme we are simply pass it to every component.

It' is not very recommended to use context a lot in your app
because it will make the components less usable so avoid using them when you can.

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-33)
