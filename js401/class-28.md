# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 401

# Read: 28 - Component Lifecycle

## Why do we not need more .html pages in a multi-page React app?
Because we use routes to connect to one app.

## If we wanted a component to show up on every page, where would we put it and why?
Outside of a route.

## What does routing do with the components that were rendered when a new route is requested
It unmounts it or hides it somewhere else so you can't see it.

## What does props.children contain?
content between the opening and closing tags of the containing component

## How do useState() and this.setState() differ?


## Vocab:
State Hook: a special function that lets you “hook into” React features.

Mounting and Un-Mounting: mounts a storage device or filesystem, making it accessible and attaching it to an existing directory structure. The umount command "unmounts" a mounted filesystem, informing the system to complete any pending read or write operations, and safely detaching it