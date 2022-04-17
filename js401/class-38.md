# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 401

# Read: 38 - Redux - Asynchronous Actions

## How granular should your reducers be?
very?

## Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
pro

## Name a strategy for preventing the abovE
combine reducer

## Vocab:
store: A store holds the whole state tree of your application.

combined reducers: a helper function turns an object whose values are different reducing functions into a single reducing function.