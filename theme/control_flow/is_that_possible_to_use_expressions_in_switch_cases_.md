## [Is that possible to use expressions in switch cases?](#is-that-possible-to-use-expressions-in-switch-cases)

### Is that possible to use expressions in switch cases?

Yes, you can use expressions in `case` statements. The expression is evaluated and compared with the `switch` value.

Example:

```javascript
const value = 10;
switch (value) {
  case 5 + 5:
    console.log('Matched 10');
    break;
  default:
    console.log('No match');
}
```

**Tags**: basic, JavaScript, Control Flow


