# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 401

# Read: 33 - Login and Auth

## Why is the Context API useful?
Context API can share data with multiple components, without having to pass data through props manually.

## Can a component outside of a provider get its context?
The `useContext()` hook lets a component outside of a provider get its context.

## What are some common use cases for using the Context API?
Authentication

## Describe “Context Hell”
Context hell is unorganized code from nesting multiple context and passing it down to the children.

## Vocab:

global state: the data that is shared between all the components within a React application.

global context: the fallback context in JavaScript.

provider: configurable service where we can set input per application.

consumer: the fallback context in JavaScript.