# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 401

# Read: 27 - useState() Hook

## How does React differ from vanilla JS/HTML/CSS?
Plain JS apps usually start with the initial UI created on the server (as HTML), whereas React apps start with a blank HTML page, and dynamically create the initial state in JavaScript. React requires you to break your UI into components, but plain JS apps can be structured in any way you see fit.

## What is the primary difference between a function component and a class component?
A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element. A class component requires you to extend from React. Component and create a render function which returns a React element. There is no render method used in functional components.

## Vocab:
Functional Components: just a plain JavaScript function that accepts props as an argument and returns a React element

Children / Child Components: a more specific part inside a parent component. 