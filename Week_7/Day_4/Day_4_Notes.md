## Summary

Learnt more about HTML, CSS, and the DOM.

Learnt about Chrome Devtools and how to debug JS code directly within the browser using breakpoints.

Learnt about _EDA_ (Event-Driven Architecture) - a software pattern that lends itself well to asynchronous programming in JS. EDA is essentially, if X happens, then do Y. X is the Event and Y is the Event Handler.
 
The client side (The DOM) has events like mouse clicks, hover over, on load, etc. A library used to demonstrate client side events is called JQuery.

On the server side, you can think of incoming requests as events, with callback functions being the event handlers.

Since DOM elements are nested within other elements. An event that happens in a nested element can “bubble up” and propagate throughout the rest of the DOM tree. There is an event handler called stopPropagation( ) that can be used to stop this from happening.

Example of bubbling:
```html
<style>
  body * {
    margin: 10px;
    border: 1px solid blue;
  }
</style>

<form onclick="alert('form')">FORM
  <div onclick="alert('div')">DIV
    <p onclick="alert('p')">P</p>
  </div>
</form>
```


Clicking on P, will cause a bubble up event and DIV will also be clicked, along with FORM afterwards because P is nested in DIV, which is nested in FORM

Almost all events bubble! The most deeply nested element that caused an event is called a target element and we can pin point this element with event.target

Event.stopPropagation() stops the bubbling from moving upwards.

Event.stopImmediatePropagation() stops the bubbling from moving “horizontally” across other events in the same element.

Don’t stop bubbling without a specific reason! But beware of its existence.

Capturing is rarely used in real code - it is invisible to us.

The standard DOM Event has 3 phases;

* Capturing Phase - the event goes down to the element
* Target Phase - the event reached the target element
* Bubbling  - the event bubbles back up from the element

If you click on <\p>, then the sequence is:
HTML → BODY → FORM → DIV (capturing phase, the first listener):
P (target phase, triggers two times, as we’ve set two listeners: capturing and bubbling)
DIV → FORM → BODY → HTML (bubbling phase, the second listener).

Source: [Javascript.info](https://javascript.info/bubbling-and-capturing)