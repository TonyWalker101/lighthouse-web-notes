## Summary

Learnt about assertion (*assertEqual*) and what it means to debug your own code (Source: [MDN](https://developer.mozilla.org/en-US/docs/Web/API/console/assert))

``` javascript
const errorMsg = 'the # is not even';
for (let number = 2; number <= 5; number += 1) {
    console.log('the # is ' + number);
    console.assert(number % 2 === 0, {number: number, errorMsg: errorMsg});
  
}
// output:
// the # is 2
// the # is 3
// Assertion failed: {number: 3, errorMsg: "the # is not even"}
// the # is 4
// the # is 5
// Assertion failed: {number: 5, errorMsg: "the # is not even"}
```

Learnt how to create strings from arrays without using __.join()__

``` javascript

let joinList = arr => {
  let answer = ``;
  for (let i = 0; i < arr.length; i ++) {
    let x = arr[i];
    answer += `${x}`;
    if (i === arr.length - 1) {
      return answer;
    } else {
      answer += `, `;
    }
  } return answer 
}; 
```

Learnt how to incur a random integer from two values (Source: [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random))

``` javascript
function getRandomInt(min, max) {
  min = Math.ceil(min);
  max = Math.floor(max);
  return Math.floor(Math.random() * (max - min) + min); //The maximum is exclusive and the minimum is inclusive
}
```
Command line arguments and how to use them in code (and how to skip the first two elements of _process.argv_ using i = 2)

``` javascript
const args = process.argv;

let sum = () => {
  let answer = 0;
  for (let i = 2; i < args.length; i ++) {
    answer += (Number(args[i]));
  }
  return answer;
};

console.log(sum());
```