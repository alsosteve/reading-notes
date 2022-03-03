# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 401

# Read: 39 - Redux - Additional Topics

## What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?
with thunk middleware to handle the asyncronus http request to an API.

## When using a thunk/async action that dispatches the actual action, which do you export from your reducer?
the function

## Vocab:
middleware: provides a third-party extension point between dispatching an action, and the moment it reaches the reducer.

thunk: middleware that allows you to write action creators that return a function instead of an action. The thunk can be used to delay the dispatch of an action.