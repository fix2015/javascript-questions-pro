## [Why do I need to use freeze method](#why-do-i-need-to-use-freeze-method)

### Why do I need to use freeze method?

Using `Object.freeze()` is useful when you want to ensure that the object’s properties cannot be changed, helping to prevent bugs caused by unintended modifications.

Example:

```javascript
const config = { maxLimit: 100 };
Object.freeze(config);
config.maxLimit = 200; // Won't work
```

**Tags**: basic, JavaScript, objects

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7457632028364737825](https://www.tiktok.com/@jsmentoring/photo/7457632028364737825)
