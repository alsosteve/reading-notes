# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 401

# Read: 37 - Redux - Combined Reducers

## Why choose Redux instead of the Context API for global state?
Context API is a light-weight solution which is more suited for passing data from a parent to a deeply nested child and Redux is a more robust State Management solution

## What is the purpose of a reducer?
A reducer is a pure function that takes an action and the previous state of the application and returns the new state. The action describes what happened and it is the reducer's job to return the new state based on that action

## What does an action contain?
An action statement is a command used in computer programming languages that perform actions such as opening a file and saving a file

## Why do we need to copy the state in a reducer?
To save the previous state, a way to describe the unchanged part

## Vocab:
immutable state: an object whose state cannot be modified after it is created

time travel in redux: RTT will keep track of all slices in your state and move them forward or backward with time travel events

action creator: a function that literally creates an action object. In Redux, action creators simply return an action object and pass the argument value if necessary

reducer: a function which takes two arguments — the current state and an action — and returns based on both arguments a new state

dispatch: a function of the Redux store