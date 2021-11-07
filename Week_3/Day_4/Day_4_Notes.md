## Summary 

Learnt about method overriding => when a subclass overrides the method of a superclass. 

The __super__ keyword allows subclasses to call methods from the superclass. For example; 

```javascript
super.method() //refers to the method of the super class 
this.method() //refers to the method of the current subclass 
```

_Getters_ => used to generate the value of a property without having to directly keep track of the property using the __get__ keyword.

_Setters_ => used to set the value of a property and to validate the data inputted into the property using the __set__ keyword.

By using the __get__ and __set__ keywords, methods of your object can be assessed as if they were properties of the object instead of methods.

    Note: not all getters and setters need to be defined using the get and set keywords. However, using them can make your code easier to read for other developers.

Learnt the difference between;

```javascript
Math.floor() // always rounds back down to lower #
Math.ceil() // always rounds up to next #
Math.round() // either rounds up or down to nearest #
Math.sqrt( ) //computes the square root of a #
```

(^Source: [PawelGrzybek](https://pawelgrzybek.com/rounding-and-truncating-numbers-in-javascript/))

Learnt more about the _.sort( )_ array method. (Source: [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort))

Learnt about _Dependency Injection_ => it means passing an object the things it needs instead of the object reaching for those things itself. This is a better design pattern because it makes code more modular and easier to test.