## Summary

Learnt the difference between a **for...in** (iterates though arrays) loop and a **for...of** loop (iterates through object keys)

Learnt how to use [.includes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/includes) to loop through arrays

Learnt about the **.forEach()** method and how it can be used instead of regular for loops to iterate arrays (Source: [dmitripavultin](https://dmitripavlutin.com/foreach-iterate-array-javascript/))

``` javascript
const colors = ['blue', 'green', 'white'];
function iterate(item, index) {
  console.log(`${item} has index ${index}`);
}
colors.forEach(iterate);
// logs "blue has index 0"
// logs "green has index 1"
// logs "white has index 2"
```
Learnt more about arrow functions and about how they _cannot_ be used with the **this** method (Source: [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this))

``` javascript
const test = {
  prop: 42,
  func: function() {
    return this.prop;
  },
};

console.log(test.func());
// expected output: 42
```
Watched a video on arrow functions and how they can be used
(Source: [Fun Fun Function](https://youtu.be/6sQDTgOqh-I))


