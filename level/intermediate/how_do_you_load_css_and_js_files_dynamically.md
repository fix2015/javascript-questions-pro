## [How do you load CSS and JS files dynamically](#how-do-you-load-css-and-js-files-dynamically)

### How do you load CSS and JS files dynamically?

You can dynamically load CSS and JavaScript files by creating `link` and `script` elements and appending them to the document's `head`.

Example for loading a CSS file:

```javascript
const link = document.createElement('link');
link.rel = 'stylesheet';
link.href = 'style.css';
document.head.appendChild(link);
```

Example for loading a JS file:

```javascript
const script = document.createElement('script');
script.src = 'script.js';
document.body.appendChild(script);
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [DOM manipulation](./theme/dom_manipulation)


