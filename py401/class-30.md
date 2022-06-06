# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
Code Fellows Python 401

# Read: Data Structure and Analysis - Hash Tables

### Common Terminology:

- `Hash` - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.
- `Buckets` - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.
- `Collisions` - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

## Uses
- Hold unique values
- Dictionary
- Library

## Hashtables
- data structure that utilize key value pairs
- every `Node` or `Bucket` has both a key, and a value
- `hash`: ability to encode the key that will eventually map to a specific location to retrieve the value
- `O(1)` time complexity

## Structure
### Hashing
- turns a key into an integer
- deterministic: their output is determined only by their input
- same key will always produce same hash code

### Creating a Hash
- created from an array
- turn that “key” into a numeric number value
#### possible suggestion:
1. Add or multiply all the ASCII values together.
2. Multiply it by a prime number such as 599.
3. Use modulo to get the remainder of the result, when divided by the total size of the array.
4. Insert into the array at that index.

ex.

``` python
Key = "Cat"
Value = "Josie"

67 + 97 + 116 = 280

280 * 599 = 69648

69648 % 1024 = 16

Key gets placed in index of 16. 
```

## Collisions
- occurs when more than one key hashes to the same index
- “perfect hash” will never have any collisions

## Internal Methods
`Add()` - adding a new key/value pair
`Find()` - takes in a key, gets the Hash, and goes to the index location specified
`Contains()` - accept a key, and return a bool if key exists
`GetHash()` - accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed

## Bookmark and Review
- ## [Intro to Hash Tables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)
- ## [what is a hash table?](https://www.youtube.com/watch?v=MfhjkfocRR0)
- ## [basics of hash tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)
- ## [hash table wiki](https://en.wikipedia.org/wiki/Hash_table)