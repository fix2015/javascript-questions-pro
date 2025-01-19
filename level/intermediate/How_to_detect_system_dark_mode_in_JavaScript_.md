## [How to detect system dark mode in JavaScript?](#how-to-detect-system-dark-mode-in-javascript)

### How to detect system dark mode in JavaScript?

Use the `matchMedia` method with the `(prefers-color-scheme)` media query.

Example:
```javascript
const isDarkMode = window.matchMedia('(prefers-color-scheme: dark)').matches;

if (isDarkMode) {
  console.log('Dark mode is enabled');
} else {
  console.log('Light mode is enabled');
}
```

#### Listen for Changes:
```javascript
const mediaQuery = window.matchMedia('(prefers-color-scheme: dark)');

mediaQuery.addEventListener('change', event => {
  if (event.matches) {
    console.log('Dark mode activated');
  } else {
    console.log('Light mode activated');
  }
});
```

**Tags**: intermediate, JavaScript, Web APIs


