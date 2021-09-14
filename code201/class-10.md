# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 201

# Read: 10 - JS Debugging

## [JavaScript & JQuery]

### Chapter 10: Error Handling & Debugging (p. 449-486)
This chapter of the book goes over how to find errors in code and how to write code that runs more smoothly.

**_Order of execution_** To find errors, you need to know how scripts are processed. It h=must go in a single file order. 

#### Execution Contexts:

##### Executed Context	
Every statement in a script lives in one of 3 execution contexts:

1. **_Global Context_**- Code that is in the script, but not a function. There is only one in any page.

2. **_Function Content_**- Code run within a function. Each function has its own function context.

3. **_Eval Context_**- Text is executed like code in an internal function called eval(). [Not covered in book]

##### Variable Scope

* **_Global Scope_**- If a variable is declared outside a function, it can be used anywhere because it has global scope. If you do not use the var keyword when creating a variable, it is placed in global scope.

* **_Funciton-Level Scope_**- When a variable is declared within a function, it can only be used within that function. This is because it has function-level scope.