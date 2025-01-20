## [How do you validate an email in javascript](#how-do-you-validate-an-email-in-javascript)

### How do you validate an email in JavaScript?

To validate an email in JavaScript, you can use a regular expression. A common pattern for basic email validation looks like this:

```javascript
const email = 'test@example.com';
const regex = /^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,4}$/;
console.log(regex.test(email)); // true
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [validation](./theme/validation)

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7456043510161067296](https://www.tiktok.com/@jsmentoring/photo/7456043510161067296)
