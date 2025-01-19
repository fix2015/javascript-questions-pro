## [How do you check web storage browser support?](#how-do-you-check-web-storage-browser-support)

### How do you check web storage browser support?

To check if a browser supports web storage, you can check if `localStorage` or `sessionStorage` is available:

```javascript
if (typeof(Storage) !== 'undefined') {
  // Web storage is supported
} else {
  // Web storage is not supported
}
```

**Tags**: basic, web storage, browser support, JavaScript

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7448750198848769313](https://www.tiktok.com/@jsmentoring/photo/7448750198848769313)
