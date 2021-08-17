# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 201

# Read: 06 - JS Object Literals; The DOM

## [JavaScript & JQuery]

### Chapter 3: Object Literals (p. 100-105 ONLY)

#### Objects
**_Objects_** are like data base objects. It is like a _personel folder_ that stores various forms of information. 
**_Properties_** are variables stored within an object.
**_Methods_**, like properties to variables, are what you call functions stored in an object.

``` javaScript
// example of object named hotel
var hotel = {
// these are properties
  name: 'Quay',
  rooms: 40 '
  booked: 25,
  gym: true,
  roomTypes: ['twin', 'double', 'suite'],
// this is a method
  checkAvailability: function() {
    return this.rooms - this.booked;
  }
};
```
The **_key_** is how you define the variables and functions. they are on the left side of the ':'.
The values are what is contained within the key, there are what follows the ':'.

#### Accessing an Object
There are 2 ways to acces an object, dot notations and the square bracket method.

##### Dot Notation
`var hotelName = hotel.name;`
`var roomsFree = hotel.checkAvailability();`
The property to the right of the `.` is within the object stated on the right. The variable on the left is declared to hold the information of the object called.

##### Square Bracket
`var hotelName = hotel['name'];`
`var roomsFree = hotel['checkAvailability']();`
You use this notation when:
* name of property contains special characters like a dash
* name of property is a number
* a variable is used in place of property name

### Chapter 5: Document Object Model (p. 183-242)