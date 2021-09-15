# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 301

# Read: 03 - Passing Functions as Props

## Reading

### [React Docs - List and Keys](https://reactjs.org/docs/lists-and-keys.html)
1. .map() returns the values of an array as doubled values.
2. To display values in an array in JSX, you can assign the array of elements to list items.
3. Each list item needs a unique key.
4. The purpose of a key is to help React identify which items have changed, are added, or are removed.

### [The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)
1. The spread operator lets you add items to, combine, and spread out an array into a function's arguments.
2. Spread operators can:
* Copying an array
* Concatenating or combining arrays
* Using Math functions
* Using an array as arguments

3. How to combine two arrays:
``` javascript
const myArray = [`a`,`b`,`c`]
const yourArray = [`d`,`e`,`f`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // a b c d e f
```
4. How to add a new item to an array:
``` javascript
const fewFruit = ['1','2','3']
const fewMoreFruit = ['x', 'y', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "x", "y", "1", "2", "3" ]
```
5. How to combine two objects into one:
``` javascript
const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂
```

### [How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)
1. He creates a function named, increment, that passes in a person.
2. The increment function updates the person objects.

3. 
4. 