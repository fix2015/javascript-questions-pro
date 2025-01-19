## [What are default values in destructuring assignment](#what-are-default-values-in-destructuring-assignment)

### What are default values in destructuring assignment?

Default values in destructuring assignment allow you to assign a default value to a variable if the value being destructured is `undefined`. This is useful when destructuring objects or arrays with missing values.

Example with array:

```javascript
let [x = 10, y = 20] = [5];
console.log(x, y);  // Output: 5 20
```
Example with object:

```javascript
let { name = 'Guest', age = 25 } = { name: 'John' };
console.log(name, age);  // Output: John 25
```

**Tags**: intermediate, JavaScript, Destructuring


