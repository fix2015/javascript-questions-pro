## [How do you return all matching strings against a regular expression](#how-do-you-return-all-matching-strings-against-a-regular-expression)

### How do you return all matching strings against a regular expression?

You can use the `match()` method with a regular expression to return all matching substrings in a string. The `g` flag in the regular expression allows the method to match all occurrences, not just the first one.

Example:

```javascript
let str = 'abc123 def456 ghi789';
let matches = str.match(/\d+/g);
console.log(matches);  // Output: ['123', '456', '789']
```

In this example, `\d+` is a regular expression that matches one or more digits, and the `g` flag ensures that all matches are returned in an array.

**Tags**: intermediate, JavaScript, Regular Expressions


