# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 401

# Read: 31 - Context API

## Describe use cases useState() vs useReducer()
useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.

## Why do custom hooks need the use prefix?
Unique hooks require it because it checks for violations of the hook rules.

## What do custom hooks usually do?
Custom hooks are normal JS functions, named with the prefix 'use', that can use hooks inside of it and contain a common stateful logic to be reused in other components

## Using any list of custom hooks, research and name one that you think will be useful in your applications
useSelectableList, this is a hook that will select a single value from a list of values.

## Describe how a hook that fetches API data might work


## Vocab:

reducer:  a pure function that takes an action and the previous state of the application and returns the new state.