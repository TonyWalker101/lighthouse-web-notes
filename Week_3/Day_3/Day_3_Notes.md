## Summary

Learnt about Classes, the constructor method, and the concept of inheritance in OOP and how it can be used to eliminate duplication in code.

```javascript
class Person {
  constructor(name, email) {
    this.name = name;
    this.email = email;
  }
  
  sayHi() {
    return `Hi my name is ${this.name}`;
  }
}

const tony = new Person();
```

Learnt about how to throw an error and catch it in chai (Source: [Chaijs](https://www.chaijs.com/api/assert/#method_throws))

```javascript
assert.throws(function(){functionYoureThrowing}, 'Error thrown must have this same message');
```



