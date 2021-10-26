## Summary 

Learnt about the [Array.isArray()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/isArray
) method and how to use it to define if something is an array or not.

Learnt about objects and how we must use square bracket notation to access an objects values.

Square brackets can also be used to assign new values to new or existing keys and/ or to access nested values

Learnt about how the .filter() method can only be used on an array and with an accompaying function in its brackets (Source: [w3schools](https://www.w3schools.com/jsref/jsref_filter.asp))

``` javascript
const ages = [32, 33, 16, 40];

ages.filter(checkAdult)    // Returns [32, 33, 40]

function checkAdult(age) {
  return age >= 18;
} 
```
Learnt about JSON.stringify and JSON.parse, along with multiple other ways of copying arrays (Source: [freecodecamp](https://www.freecodecamp.org/news/how-to-clone-an-array-in-javascript-1d3183468f6a/))

```
nestedNumbers = [[1], [2]];
numbersCopy = JSON.parse(JSON.stringify(nestedNumbers));

numbersCopy[0].push(300);
console.log(nestedNumbers, numbersCopy);

// [[1], [2]]
// [[1, 300], [2]]
// These two arrays are completely separate!
```
Learnt that **[...arrayYouWantToClone]** can also be used to clone an array (Source: [samanthaming](https://www.samanthaming.com/tidbits/35-es6-way-to-clone-an-array/))

Learnt that _.ToUpperCase_ can be used to capitalize all letters in a string
