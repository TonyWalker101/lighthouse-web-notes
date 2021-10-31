## Summary

Learnt about recursions. Recursive functions must have a recursive case (what happens when the stopping condition is false) and a base case (what happens when the stopping condition is true)

When creating recursive functions it can be helpful to create the stopping condition (the base case) first before moving onto the recursive case itself.

Example of recursion (Source: [MDN](https://developer.mozilla.org/en-US/docs/Glossary/Recursion)):

```javascript
def recurse(x):
   if x > 0:
       print(x)
       recurse(x - 1)

recurse(10)
```

Any iteration (loop) problem can be solved using recursion and vice versa.

Learnt the difference between unit testing (testing a specific function), integration testing (testing how a program and a database, for example, work together), and functional testing (testing a program in it's entirety - including how a user would use the program) (Source: [Codeutopia](https://codeutopia.net/blog/2015/04/11/what-are-unit-testing-integration-testing-and-functional-testing/))

During lecture we took a closer look into callback backs and higher order functions;

```javascript
object.method(function) 
```
In the above example, the method is the higher order function (**HOF**) because it's taking a function (the _callback_ function in this case) as an argument

```javascript
array.map(x => x + 2)
```

In this exmaple;

array = object

.map = method of the array (function of an object, in this case array) and the **HOF** in this case

x => x + 2 = the _callback function_ in this case. the HOF is taking in this callback function (in arrow notation) as an argument and running it agasint every element of the array

