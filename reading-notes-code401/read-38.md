# Read-38, Code 401, 23 May 2021

## Redux - Asynchronous Actions

### Discussion

1. How granular should your reducers be?
   would say that the default solution would be that a change of any of those attributes would trigger a separate kind of action
2. Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
   When your reducer has finished and returned the new application state, asyncDispatch will trigger store. dispatch with whatever action you give to it. You might try using a library like redux-saga.

3. Name a strategy for preventing the above
   having a specific names the represent the reducer will solve it.

### Vocabulary

- store:A store is an immutable object tree in Redux. A store is a state container which holds the application's state. Redux can have only a single store in your application. Whenever a store is created in Redux, you need to specify the reducer.

- combined reducers: It turns out that Redux lets us combine multiple reducers into one that can be passed into createStore by using a helper function named combineReducers . The way we combine reducers is simple, we create one file per reducer in the reducers directory. We also create a file called index. js inside the reducers directory.

### Preview

#### async action

Writing an Async Function Middleware#
Both of the middleware in that last section were very specific and only do one thing. It would be nice if we had a way to write any async logic ahead of time, separate from the middleware itself, and still have access to dispatch and getState so that we can interact with the store.

What if we wrote a middleware that let us pass a function to dispatch, instead of an action object? We could have our middleware check to see if the "action" is actually a function instead, and if it's a function, call the function right away. That would let us write async logic in separate functions, outside of the middleware definition.

Example async function middleware

```js
const asyncFunctionMiddleware = (storeAPI) => (next) => (action) => {
  // If the "action" is actually a function instead...
  if (typeof action === 'function') {
    // then call the function and pass `dispatch` and `getState` as arguments
    return action(storeAPI.dispatch, storeAPI.getState);
  }

  // Otherwise, it's a normal action - send it onwards
  return next(action);
};
```

#### Redux Thunk

Redux Thunk is middleware that allows you to return functions, rather than just actions, within Redux. This allows for delayed actions, including working with promises. One of the main use cases for this middleware is for handling actions that might not be synchronous, for example, using axios to send a GET request.

What's a thunk?
A thunk is a function that wraps an expression to delay its evaluation.

Example:

```js
// calculation of 1 + 2 is immediate
// x === 3
let x = 1 + 2;

// calculation of 1 + 2 is delayed
// foo can be called later to perform the calculation
// foo is a thunk!
let foo = () => 1 + 2;
```

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-38)
