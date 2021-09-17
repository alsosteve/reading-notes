# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 301

# Read: 05 - Putting it all together

## Reading

### [React Docs - Thinking In React](https://reactjs.org/docs/thinking-in-react.html)
1. The single responsibility principle is a rule or guideline that says that a component should only do one thing.

2 .A static version of your application is a build that has no interactivity. You don’t use state at all.

3 .Once the static version of your app is up you should identify the minimal representation of UI state.

4. The three questions to find if something is state are: 
* Is it passed in from a parent via props? If so, it probably isn’t state.
* Does it remain unchanged over time? If so, it probably isn’t state.
* Can you compute it based on any other state or props in your component? If so, it isn’t state.
> answers provided by reactjs.org

5. To find where your state needs to live you should consider the following: 
* Identify every component that renders something based on that state.
* Find a common owner component (a single component above all the components that need the state in the hierarchy).
* Either the common owner or another component higher up in the hierarchy should own the state.
* If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

### [Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)
1. A higher-ordered function takes other functions as arguments or return them.
2. On line 2 bellow, the greater function will return a function that calculates if m is greater than n and then return true or false.
``` javascript
function greaterThan(n) {
  return m => m > n;
}
let greaterThan10 = greaterThan(10);
console.log(greaterThan10(11));
// → true
```
3. 