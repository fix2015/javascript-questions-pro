## [How do you convert date to another timezone in javascript](#how-do-you-convert-date-to-another-timezone-in-javascript)

### How do you convert date to another timezone in javascript?

You can use libraries like `moment.js` or the `Intl.DateTimeFormat` API to convert dates to different time zones.

Example with `Intl.DateTimeFormat`:

```javascript
const date = new Date();
const formatter = new Intl.DateTimeFormat('en-US', {
  timeZone: 'America/New_York',
  hour: 'numeric',
  minute: 'numeric'
});
console.log(formatter.format(date));
```

**Tags**: basic, JavaScript, date manipulation

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7457198473176190241](https://www.tiktok.com/@jsmentoring/photo/7457198473176190241)
