# Read-37, Code 401, 23 May 2021

## Redux - Combined Reducers

### Discussion

1. Why choose Redux instead of the Context API for global state?
   So Redux works around the idea of having a central state called a store. To change the state, a component has to dispatch an action. The action is then passed on to the reducer, which changes the state of our application

2. What is the purpose of a reducer?
   A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently.

3. What does an action contain in redux?
   An action, is an object that contains the payload of information. They are the only source of information for the Redux store to be updated. Reducers update store based on the value of the action.

4. Why do we need to copy the state in a reducer?
   Then the function uses a switch statement to determine which type of action it's dealing with. If there is an unknown action, then it should return the state , so that the application doesn't lose its current state.

### Vocabulary

- immutable state: Immutable state is state that cannot be changed. Immutable objects (for which none of the state can be changed) become important when you are dealing with concurrency, the ability for more than one processor in your computer to operate on that object at the same time.

- time travel in redux: The Redux DevTools records dispatched actions and the state of the Redux store at every point in time. ... This makes it possible to inspect the state and travel back in time to a previous application state without reloading the page or restarting the app.

- action creator: An action creator is merely a function that returns an action object. Redux includes a utility function called bindActionCreators for binding one or more action creators to the store's dispatch() function.

- reducer: Reducers tell the application how to change state in response to an action. dispatch This is the name of the function you use to send actions to the store.

- dispatch: dispatch is a function of the Redux store. You call store. dispatch to dispatch an action. This is the only way to trigger a state change. With React Redux, your components never access the store directly - connect does it for you.

### Preview

#### combineReducers

he combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

The resulting reducer calls every child reducer, and gathers their results into a single state object. The state produced by combineReducers() namespaces the states of each reducer under their keys as passed to combineReducers()

Example:

```js

rootReducer = combineReducers({potato: potatoReducer, tomato: tomatoReducer})
// This would produce the following state object
{
  potato: {
    // ... potatoes, and other state managed by the potatoReducer ...
  },
  tomato: {
    // ... tomatoes, and other state managed by the tomatoReducer, maybe some nice sauce? ...
  }
}
```

You can control state key names by using different keys for the reducers in the passed object. For example, you may call combineReducers({ todos: myTodosReducer, counter: myCounterReducer }) for the state shape to be { todos, counter }.

A popular convention is to name reducers after the state slices they manage, so you can use ES6 property shorthand notation: combineReducers({ counter, todos }). This is equivalent to writing combineReducers({ counter: counter, todos: todos }).

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-37)
