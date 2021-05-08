# Read-31, Code 401, 8 May 2021

## Hooks API

### Discussion

1. Why do we not need more .html pages in a multi-page React app?
   Using the react-router-dom package, we can implement multiple routes in a React application. A user browsing this app feels each route is each page. So in React, multiple routes are considered as multiple pages.

2. If we wanted a component to show up on every page, where would we put it and why?
   inside the `<BrowserRouter/>`, outside the `<Route/>`, and also putting it outside the `<BrowserRouter/>` will work.

3. What does props.children contain?
   props. children does is that it is used to display whatever you include between the opening and closing tags when invoking a component.

### Vocabulary

- Composition: react Composition is a development pattern based on React's original component model where we build components from other components using explicit defined props or the implicit children prop.

- Children / Child Components: children is a special property of React components which contains any child elements defined within the component

- Hash Routing: Hash value will be handled by react router. It is used to support legacy browsers which usually doesn't support HTML pushState API It doesn't need any configuration in server to handle routes This route isn't recommended by the team who created react router package

- Link Routing: Provides declarative, accessible navigation around the application.

### Preview

1. Which 3 things had you heard about previously and now have better clarity on?
   Routing in React, React-testing-lib, BDD.

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   funcitonal components, converting class component to functional one, Hooks.

3. What are you most excited about trying to implement or see how it works?
   react-use, hooks.

### React Hooks

Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class.

Basic Hooks

- `useState`

`const [state, setState] = useState(initialState);`

useState will return intial value and a funciton to change it.

state will take the intial value that passed to useState.
The `setState` function is used to update the state.

- `useEffect`

`useEffect(didUpdate)`
Accepts a function that contains imperative, possibly effectful code.

Mutations, subscriptions, timers, logging, and other side effects are not allowed inside the main body of a function component (referred to as React’s render phase). Doing so will lead to confusing bugs and inconsistencies in the UI.

**Cleaning up an effect**
Often, effects create resources that need to be cleaned up before the component leaves the screen, such as a subscription or timer ID. To do this, the function passed to useEffect may return a clean-up function.

- `useContext`

`const value = useContext(myContext);`

Accepts a context object (the value returned from React.createContext) and returns the current context value for that context. The current context value is determined by the value prop of the nearest `<MyContext.Provider>` above the calling component in the tree.

Other Hooks to read About:

- useReducer
- useCallback
- useMemo
- useRef
- useImperativeHandle
- useLayoutEffect
- useDebugValue

[react-docs](https://reactjs.org/docs/hooks-reference.html)
[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-31)
