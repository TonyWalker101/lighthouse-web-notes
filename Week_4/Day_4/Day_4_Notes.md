## Summary

Learnt more about the typeof operator and how it can be used to check the data types of variables
(Source: [MkYong](https://mkyong.com/javascript/check-if-variable-is-a-number-in-javascript/))

Learnt more about the .sort() method and how it interacts with different data types;

"The default sort order is ascending, built upon converting the elements into strings, then comparing their sequences of UTF-16 code units values."

(^Source: [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort))

To .sort() an array based off the numeric value of it's elements you must use;

```javascript
let numbers = [4, 2, 5, 1, 3];
numbers.sort((a, b) => a - b);
console.log(numbers);

// [1, 2, 3, 4, 5]
```
(^Source: [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort))




