## [Give an example of statements affected by automatic semicolon insertion?](#give-an-example-of-statements-affected-by-automatic-semicolon-insertion)

### Give an example of statements affected by automatic semicolon insertion

Automatic Semicolon Insertion (ASI) can lead to unexpected behavior when a semicolon is inserted incorrectly.

Example:
```javascript
function test() {
  return
  {
    key: 'value'
  };
}

console.log(test()); // undefined
```

Explanation:
- ASI inserts a semicolon after `return`, so the object is never returned. The correct version:

```javascript
function test() {
  return {
    key: 'value'
  };
}

console.log(test()); // { key: 'value' }
```

**Tags**: advanced, JavaScript, Syntax


