## [How do you detect a mobile browser](#how-do-you-detect-a-mobile-browser)

### How do you detect a mobile browser?

You can detect a mobile browser by checking the `navigator.userAgent` string for keywords like 'mobile', 'Android', or 'iPhone'.

Example:

```javascript
if (/Mobi/.test(navigator.userAgent)) {
  console.log('Mobile browser detected');
}
```

**Tags**: basic, JavaScript, mobile detection


