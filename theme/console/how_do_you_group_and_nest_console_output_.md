## [How do you group and nest console output?](#how-do-you-group-and-nest-console-output)

### How do you group and nest console output?

You can group and nest console output using `console.group` and `console.groupEnd`:

```javascript
console.group('Outer Group');
console.log('Message in Outer Group');
console.group('Inner Group');
console.log('Message in Inner Group');
console.groupEnd();
console.groupEnd();
```

Output:
```
Outer Group
  Message in Outer Group
  Inner Group
    Message in Inner Group
```

**Tags**: intermediate, JavaScript, Console


