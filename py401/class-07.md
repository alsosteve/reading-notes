# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
Code Fellows Python 401

# Read: 07 - Ten Thousand Game 2

## [Python Scope](https://realpython.com/python-scope-legb-rule/)
### Understanding Scope
- **scope** of a name defines the area of a program in which you can unambiguously access that name, such as variables, functions, objects, and so on.

- **Global scope**: The names that you define in this scope are available to all your code.

- **Local scope**: The names that you define in this scope are only available or visible to the code within the scope.

### Using the LEGB Rule for Python Scope
#### (Local, Enclosing, Global, and Built-in)
- **Local**: the code block or body of any Python function or lambda expression.

- **Enclosing**: a special scope that only exists for nested functions.

- **Global**: top-most scope in a Python program, script, or module.

- **Built-in**: special Python scope that’s created or loaded whenever you run a script or open an interactive session.

### Modifying the Behavior of a Python Scope
- **Global Name**: accessed, modified, or referenced from any place in your code

- **Local Name**: accessed and modified only from the local Python scope they were created in

- **nonlocal names**: accessed from inside nested functions, can’t be modified or updated from there

### Using Enclosing Scopes as Closures
- **closure** is an inner or nested function that carries information about its enclosing scope, even though this scope has completed its execution.

### Bringing Names to Scope With import
-

### Discovering Unusual Python Scopes
#### Comprehension Variables Scope
#### Exception Variables Scope
#### Class and Instance Attributes Scope

### Using Scope Related Built-In Functions
* `globals()` - built-in function that returns a reference to the current global scope or namespace dictionary. 

* `locals()` - updates and returns a dictionary that holds a copy of the current state of the local Python scope or namespace.

* `dir()` -get the list of names in the current Python scope.

* `vars()` - built-in function that returns the .__dict__ attribute of a module, class, instance, or any other object which has a dictionary attribute.

## [Video: Don’t be CONFUSED by BIG O notation anymore!](https://www.youtube.com/watch?v=5Uqawfl0VHQ)

## Bookmark and Review
- [Rolling Dice Examples](https://artofproblemsolving.com/wiki/index.php/Basic_Programming_With_Python#Program_Example_1_3)