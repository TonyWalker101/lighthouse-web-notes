## Summary

Learnt the basics of CRUD: Create, Read, Update, & Delete.

Learnt about “Safe Methods” of HTTP requests - a request that has no intended effect on the server. Basically, all the read-only methods. (Source: [Wikipedia](https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol#Safe_methods))

Learnt about _idempotent_ requests - multiple identical methods using a method that has the same effect as a single such request (Source: [Wikipedia](https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol#Idempotent_methods))

^ Example, PUT and DELETE are idempotent while POST, PATCH are not since multiple POST or PATCH requests will continue to do the same task.

Learnt about the existence of attributes of HTML (Source: [MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form#attributes))

Learnt more about the _input_ attribute and why it is so important (Source: [Mozilla](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input#attributes))

Learnt of one method of generating random alphanumeric strings (Source: [Dev.to](https://dev.to/oyetoket/fastest-way-to-generate-random-strings-in-javascript-2k5a))

```javascript
Math.random().toString(20).substring(2,8);
```
^ Returns a random(Math.random) alphanumeric (_20_ parameter in toString) string 6 characters long (from index 2 to 8)