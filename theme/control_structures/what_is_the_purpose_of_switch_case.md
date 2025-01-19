## [What is the purpose of switch-case](#what-is-the-purpose-of-switch-case)

### What is the purpose of switch-case?

The `switch-case` statement is used to perform different actions based on different conditions. It is an alternative to multiple `if-else` statements and is more readable when there are many conditions to check.

Example:

```javascript
const fruit = 'apple';
switch(fruit) {
  case 'apple':
    console.log('Apple is selected');
    break;
  case 'banana':
    console.log('Banana is selected');
    break;
  default:
    console.log('Unknown fruit');
}
```

**Tags**: basic, JavaScript, control structures


