# Read-41, Code 401, 29 May 2021

## Reac Native

### Discussion

1. Compare and Contrast Redux Toolkit with Redux “Ducks”
   Redux Toolkit is our official, opinionated, batteries-included toolset for efficient Redux development. ... It also includes the most widely used Redux addons, like Redux Thunk for async logic and Reselect for writing selector functions, so that you can use them right away.
   Ducks is a way to bundle reducers, action types, and actions into the same file. Rather than splitting up related code, it can be packaged into redux modules.

2. What is the principle advantage of Redux Toolkit
   Redux Toolkit makes it easier to write good Redux applications and speeds up development, by baking in our recommended best practices, providing good default behaviors, catching mistakes, and allowing you to write simpler code.

### Vocabulary Terms

- Redux Toolkit Slices: A function that accepts an initial state, an object full of reducer functions, and a "slice name", and automatically generates action creators and action types that correspond to the reducers and state. This API is the standard approach for writing Redux logic.

- Namespace: Programming paradigm of providing scope to identifiers (names of types, functions, variables, etc) to prevent collisions between them.

### Preparation Materials

#### React Native Basics

React Native is a JavaScript framework for writing real, natively rendering mobile applications for iOS and Android. It’s based on React, Facebook’s JavaScript library for building user interfaces, but instead of targeting the browser, it targets mobile platforms. In other words: web developers can now write mobile applications that look and feel truly “native,” all from the comfort of a JavaScript library that we already know and love. Plus, because most of the code you write can be shared between platforms, React Native makes it easy to simultaneously develop for both Android and iOS.

Example:

```js
// React Native Counter Example using Hooks!

import React, { useState } from 'react';
import { View, Text, Button, StyleSheet } from 'react-native';

const App = () => {
  const [count, setCount] = useState(0);

  return (
    <View style={styles.container}>
      <Text>You clicked {count} times</Text>
      <Button onPress={() => setCount(count + 1)} title="Click me!" />
    </View>
  );
};

// React Native Styles
const styles = StyleSheet.create({
  container: {
    flex: 1,
    justifyContent: 'center',
    alignItems: 'center',
  },
});
```

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-41)
