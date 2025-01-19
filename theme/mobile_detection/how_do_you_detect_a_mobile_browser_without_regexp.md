## [How do you detect a mobile browser without regexp](#how-do-you-detect-a-mobile-browser-without-regexp)

### How do you detect a mobile browser without regexp?

You can detect a mobile browser without using regular expressions by checking for specific properties in `navigator` or `window` objects, such as `navigator.platform` or `window.innerWidth`.

Example:

```javascript
if (navigator.platform.indexOf('iPhone') !== -1) {
  console.log('iPhone detected');
}
```

**Tags**: basic, JavaScript, mobile detection

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7457202437292674337](https://www.tiktok.com/@jsmentoring/photo/7457202437292674337)
