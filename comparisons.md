# JavaScript Notes
##### April 27, 2020

## Comparison Examples

| NOTE: |
| :--- |
|==='s checks both the value and type. All value comparisons in JS consider the type 
of value being compared, not just the === operator. Specifically, === disallows any sort of type converstion (aka, "coercion") in it's comparison, where other JS comparisons do allow coercion."

```js
3 === 3.0;              // true
"yes" === "yes";        // true
"null" === "null;       // true
false === false;        // true

42 === "42";             // false
"hello" === "Hello";     // false
true === 1;              // false
0 === null;              // false
"" === null;             // false
null === undefined;      // false
```
