## [How do you perform language specific date and time formatting](#how-do-you-perform-language-specific-date-and-time-formatting)

### How do you perform language-specific date and time formatting?

In JavaScript, you can use the `Intl.DateTimeFormat` object to format dates and times according to a specific locale. It allows you to customize the date and time formatting styles (e.g., short, long, etc.) and even customize how individual date parts (like day, month, year) are displayed.

Example:

```javascript
const date = new Date();
const formatter = new Intl.DateTimeFormat('en-US', { year: 'numeric', month: 'long', day: 'numeric' });
console.log(formatter.format(date)); // 'December 21, 2024'
```

**Tags**: basic, JavaScript, internationalization


