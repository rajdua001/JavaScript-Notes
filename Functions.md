# JavaScript Notes
##### April 27, 2020

## Functions

The functions can be invoked one ore more times. They can be provided with some inputs and they may also give back one or more outputs.

**Function declaration:**

```js
/*'a' and 'b' are the input parameters*/

function add(a, b) {
  return a + b;
}
``` 

**Function expression:**

```js
/*'a' and 'b' are the input parameters*/

var add = function(a, b) {
  return a + b;
}
```

| NOTE: |
| :-- |
|In JS, functions are values that can be assigned and passed around. They are a special type of the object value type.|

**Function as properties on objects:**

```js
var whatToSay = {
  greeting() {
    console.log("Hello");
  },
  question() {
    console.log("What's your name?");
  },
  answer() {
    console.log("My name is Raj.");
  }
}
```
