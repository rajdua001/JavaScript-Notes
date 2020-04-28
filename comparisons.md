# JavaScript Notes
##### April 27, 2020

## Comparison Examples

| NOTE: |
| :--- |
|==='s checks both the value and type. All value comparisons in JS consider the type of value being compared, not just the === operator. Specifically, === disallows any sort of type converstion (aka, "coercion") in it's comparison, where other JS comparisons do allow coercion."|

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

**Special Values Comparison:**

```js
  NaN === NaN;           // false
  0 === -0;              // true
```

**Object Comparison:**

```js
[ 1, 2, 3 ] === [ 1, 2, 3 ];    // false
{ a: 42 } === { a: 42 }         // false
(x => x * 2) === (x => x * 2)   // false
```

## Coercive Comparisons:

Coercion means a value of one type being converted to its respective representation in another type to whatever extend possible.

The == operator performs an equality comparison similarly to how the === peforms it. In fact,  both operators consider the type of the values being compared. And if the comparison is between the same value type, both == and === **do exactly the same thing, no difference whatsoever.**

The == operator allows coercion before the comparison. In other word, they both want to compare values of like types, but == allows type conversions first, and once the types have been converted to be the same on both sides, then == does same thing as ===.

```js
42 == "42";             // true
1 == true;              // true
```

In both comparisons, the value types are different, so the == causes the non-number values ("42" and true) to be converted to numbers (42 and 1, respectively) before the comparisons are made.
