## [What are the conventions to be followed for the usage of switch case](#what-are-the-conventions-to-be-followed-for-the-usage-of-switch-case)

### What are the conventions to be followed for the usage of switch case?

Here are some best practices for using `switch-case` in JavaScript:

- Always include a `default` case to handle unexpected values.
- Ensure each `case` ends with a `break` statement to avoid falling through to the next case.
- Avoid using `switch-case` for complex conditions that can be handled with `if-else` statements.

Example:

```javascript
const number = 2;
switch(number) {
  case 1:
    console.log('One');
    break;
  case 2:
    console.log('Two');
    break;
  default:
    console.log('Unknown number');
}
```

**Tags**: basic, JavaScript, control structures


