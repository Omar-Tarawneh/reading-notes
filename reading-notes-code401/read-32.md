# Read-32, Code 401, 9 May 2021

## Custom Hooks

### Discussion

1. What does a component’s lifecycle refer to?
   Components are created (mounted on the DOM), grow by updating, and then die (unmount on DOM).

2. Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect?
   useCallback will help in avoiding regeneration of functions when the functional component re-renders. However there isn't much of a performance difference caused by recreation of functions. You are specifying a function as a dependency to useEffect .

3. Why are functional components preferred over class components?
   The essence of why I find functional components superior is this: you can ramp complexity incrementally . ... In the case of the functional component, I pretty much could. I might have to look up the ReactDOM. render call, but otherwise we are just dealing with a JavaScript function and JSX

4. What is wrong with the following code?
   all the Hooks should by at the top of the function and can't be used in block of codes like if or for loops.

### Vocabulary

- state hook: A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.

- effect hook: The Effect Hook lets you perform side effects in function components:

- reducer hook: use sometimes to manage the state of the application. It is very similar to the useState hook, just more complex.

### Preview

1. Which 3 things had you heard about previously and now have better clarity on?
   Hooks, functional component, custom hooks.

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   useReducer, and other hooks that can I use.

3. What are you most excited about trying to implement or see how it works?
   Functional component in general, there is a lib I want to see if I can take benifit from it also :).

#### Custom Hooks React

A custom hook allows you to extract some components logic into a reusable function. A custom hook is a Javascript function that starts with use and that call can other hooks. ... We are just refactoring our code into another function to make it reusable.

for Example:

```js
const useDocumentTitle = (title) => {
  useEffect(() => {
    document.title = title;
  }, [title]);
};
```

##### useReducer

`useReducer` is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

links for Review:
[custom hooks](https://www.telerik.com/blogs/everything-you-need-to-create-a-custom-react-hook)
[async hooks](https://dev.to/vinodchauhan7/react-hooks-with-async-await-1n9g)
[useReducer Hook](https://reactjs.org/docs/hooks-reference.html#usereducer)
[react custom hooks](https://reactjs.org/docs/hooks-custom.html)

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-32)
