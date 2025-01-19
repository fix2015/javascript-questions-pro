## [How to convert string to title case with javascript](#how-to-convert-string-to-title-case-with-javascript)

### How to convert string to title case with JavaScript?

You can convert a string to title case by splitting the string into words, capitalizing the first letter of each word, and then joining them back together.

Example:

```javascript
function toTitleCase(str) {
  return str.replace(/\b(\w)/g, char => char.toUpperCase());
}
console.log(toTitleCase('hello world')); // 'Hello World'
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [string manipulation](./theme/string_manipulation)

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7457578972889615648](https://www.tiktok.com/@jsmentoring/photo/7457578972889615648)
