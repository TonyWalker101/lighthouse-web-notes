## Summary 

Took a closer look into **.filter()** to learn more about them and how they can be used with arrow functions and callbacks (Source: [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter))

```javascript
const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];

const result = words.filter(word => word.length > 6);

console.log(result);
// expected output: Array ["exuberant", "destruction", "present"]
```

Learnt more about high order functions and how they are integral to **Functional Programming** ([YouTube Video by FunFunFunction](https://www.youtube.com/watch?v=BMUiFMZr7vk))

Took a closer look into **.map()** and how this method can be used with callbacks and arrow functions (Source: [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map))

```javascript
const array1 = [1, 4, 9, 16];

// pass a function to map
const map1 = array1.map(x => x * 2);

console.log(map1);
// expected output: Array [2, 8, 18, 32]
```


