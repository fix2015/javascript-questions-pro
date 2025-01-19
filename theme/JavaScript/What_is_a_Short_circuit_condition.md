## [What is a Short circuit condition](#what-is-a-short-circuit-condition)

### What is a Short-circuit condition?

A short-circuit condition occurs when the evaluation of a logical expression stops as soon as the result is determined. This is common with logical `AND` (`&&`) and `OR` (`||`) operators.

- In an `AND` condition, if the first operand is falsy, the second operand is not evaluated.
- In an `OR` condition, if the first operand is truthy, the second operand is not evaluated.

Example:

```javascript
let a = false;
let b = true;
console.log(a && b);  // 'false', 'b' is not evaluated

**Tags**: intermediate, JavaScript, Logical Operators


