## [How do you trim a string at the beginning or ending](#how-do-you-trim-a-string-at-the-beginning-or-ending)

### How do you trim a string at the beginning or ending?

You can use the `trimStart()` and `trimEnd()` methods to remove whitespace from the beginning or the end of a string, respectively. Alternatively, `trim()` removes whitespace from both ends.

Example:

```javascript
let str = '   Hello World!   ';
console.log(str.trimStart());  // Output: 'Hello World!   '
console.log(str.trimEnd());    // Output: '   Hello World!'
```

**Tags**: basic, JavaScript, String Manipulation


