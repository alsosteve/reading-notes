# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 401

# Read: 01 - Node Ecosystem, TDD, CI/CD

### Array Methods

#### Array.map
The array.map() method creates a new array by calling on a function element at each index of a starting array. The new array is the same length as the starting one.

#### Array.reduce
The array.reduce() method takes in an array and produces a single value based on a callback function.

### Code snippet of superagent

#### normal Promise .then() syntax
``` javascript
 request
   .post('/api/pet')
   .send({ name: 'Manny', species: 'cat' })
   .set('X-API-Key', 'foobar')
   .set('Accept', 'application/json')
   .then(res => {
      alert('yay got ' + JSON.stringify(res.body));
   });
```
``` javascript
 request
   .get('/search')
   .then(res => {
      // res.body, res.headers, res.status
   })
   .catch(err => {
      // err.message, err.response
   });
   ```
> [Code provided by visionmedia](https://visionmedia.github.io/superage)

#### with async / await syntax
``` javascript
 request
  .post(my api call)
  .send(params) // an object of parameters that is to be sent to api 
  .end((err, res) => {
  if(!err) {
     let impVariable = res.resImpVariable;
  } else {
    console.log('error present');
   }
  });
   ```
> [Code provided by stackoverflow](https://stackoverflow.com/questions/62187645/how-do-i-use-aysnc-await-in-this-superagent-call)

### Promises

A promise an object in code that is a representation of data that is currently not available but will be.

### Are all callback functions considered to be Asynchronous? Why or Why Not?

Callback functions can asyncronus if used in asynchronous code.