## [How do get the timezone offset from date](#how-do-get-the-timezone-offset-from-date)

### How do you get the timezone offset from date?

You can get the timezone offset from a `Date` object in JavaScript using the `getTimezoneOffset()` method. This method returns the difference between UTC and the local time, in minutes.

Example:

```javascript
const date = new Date();
const offset = date.getTimezoneOffset();
console.log(offset); // Logs the timezone offset in minutes
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [Date](./theme/date)


