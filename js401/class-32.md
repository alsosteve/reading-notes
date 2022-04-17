# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 401

# Read: 32 - Context API - Behaviors

## When you have multiple contexts, what component type should you use (class/function) and why?


## What are some good use cases for using the Context API for global state?
Good uses of Context API for global state are current authenticated user, themes, or perferred language.

## How can you best test context?
The best way to test Context is to make our tests unaware of its existence and avoiding mocks.

## Vocab:

context: React Context is a method to pass props from parent to child component(s), by storing the props in a store(similar in Redux) and using these props from the store by child component(s) without actually passing them manually at each level of the component tree.

useContext(): A hook used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level. Context defined will be available to all the child components without involving “props”.

static context: A static method or, block belongs to the class and these will be loaded into the memory along with the class.