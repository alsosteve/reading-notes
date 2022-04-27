# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
Code Fellows Python 401

# Read: 08 - Ten Thousand Game 3

## [List Comprehensions](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)
- In Python, List Comprehensions are a more compact way to create and manage lists
- faster and more flexible than for loops

### Syntax

``` python
my_new_list = [ expression for item in list ]
```
three main parts(in square brackets):
1. `expression` - expression we’d like to carry out
2. `item` - object that the expression will work on
3. `list` - iterable list of objects to build our new list from

### Create a List with range()

#### Creating a list with list comprehensions

``` python
# construct a basic list using range() and list comprehensions
# syntax
# [ expression for item in list ]
digits = [x for x in range(10)]

print(digits)
```

#### Output
``` python
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```

- the first `x` doesn't do anything(just records a number)
- second `x` is the item created

### Create a List Using Loops and List Comprehension in Python

#### Comparing list creation methods in Python

##### For Loop

``` python
# create a list using a for loop
squares = []

for x in range(10):
    # raise x to the power of 2
    squares.append(x**2)

print(squares)
```

##### List Comp

``` python
# create a list using list comprehension
squares = [x**2 for x in range(10)]

print(squares)
```

#### Output
``` python
[0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```

- List comprehension reduces the amount of code needed to produce the same output

### Multiplying Parts of a List

``` python
# create a list with list comprehensions
multiples_of_three = [ x*3 for x in range(10) ]

print(multiples_of_three)
```

#### Output
``` python
[0, 3, 6, 9, 12, 15, 18, 21, 24, 27]
```

``` python
# create a list with list even numbers
even_numbers = [ x for x in range(1,20) if x % 2 == 0]
```

### Show the first letter of each word using Python

``` python
# a list of the names of popular authors
authors = ["Ernest Hemingway","Langston Hughes","Frank Herbert","Toni Morrison",
    "Emily Dickson","Stephen King"]

# create an acronym from the first letter of the author's names
letters = [ name[0] for name in authors ]
print(letters)
```

#### Output
``` python
['E', 'L', 'F', 'T', 'E', 'S']
```

##### Separating the characters in a string

``` python
# use list comprehension to print the letters in a string
letters = [ letter for letter in "20,000 Leagues Under The Sea"]

print(letters)
```

#### Output
``` python
['2', '0', ',', '0', '0', '0', ' ', 'L', 'e', 'a', 'g', 'u', 'e', 's', ' ', 'U', 'n', 'd', 'e', 'r', ' ', 'T', 'h', 'e', ' ', 'S', 'e', 'a']
```

### Lower/Upper case converter using Python

``` python
lower_case = [ letter.lower() for letter in ['A','B','C'] ]
upper_case = [ letter.upper() for letter in ['a','b','c'] ]

print(lower_case, upper_case)
```

#### Output
``` python
['a', 'b', 'c'] ['A', 'B', 'C']
```

### Print numbers only from a given string

``` python
# user data entered as name and phone number
user_data = "Elvis Presley 987-654-3210"
phone_number = [ x for x in user_data if x.isdigit()]

print(phone_number)
```

#### Output
``` python
['9', '8', '7', '6', '5', '4', '3', '2', '1', '0']
```

### Parsing a file using list comprehension

- you can even read files usung list comprehension

``` txt
Hold fast to dreams
For if dreams die
Life is a broken-winged bird
That cannot fly.
-Langston Hughes
```

``` python
# open the file in read-only mode
file = open("dreams.txt", 'r')
poem = [ line for line in file ]

for line in poem:
    print(line)
```

#### Output
``` python
Hold fast to dreams

For if dreams die

Life is a broken-winged bird

That cannot fly.

-Langston Hughs
```

### Using functions in list comprehensions

#### adding arguments

``` python
# list comprehension with functions
# create a function that returns a number doubled
def double(x):
    return x*2

nums = [double(x) for x in range(1,10)]
print(nums)
```

#### Output
``` python
[2, 4, 6, 8, 10, 12, 14, 16, 18]
```

#### using filters
``` python
# add a filter so we only double even numbers
even_nums = [double(x) for x in range(1,10) if x%2 == 0]
print(even_nums)
```

#### Output
``` python
[4, 8, 12, 16]
```

#### complex arguments
``` python
nums = [x+y for x in [1,2,3] for y in [10,20,30]]
print(nums)
```

#### Output
``` python
[11, 21, 31, 12, 22, 32, 13, 23, 33]
```

## [Audio: Debugging with PySnooper](https://www.pythonpodcast.com/pysnooper-python-debugging-episode-241/)

## Bookmark and Review
- [Primer on Decorators](https://realpython.com/primer-on-python-decorators/)