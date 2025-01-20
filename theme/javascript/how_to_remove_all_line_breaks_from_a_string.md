## [How to remove all line breaks from a string](#how-to-remove-all-line-breaks-from-a-string)

### How to remove all line breaks from a string?

You can remove line breaks using the `replace()` method with a regular expression that targets line breaks (`
` or ``).

Example:

```javascript
let str = 'Hello
World
!';
let cleanedStr = str.replace(/[
]+/g, ' ');
console.log(cleanedStr);  // Output: 'Hello World !'
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Strings](./theme/strings)


