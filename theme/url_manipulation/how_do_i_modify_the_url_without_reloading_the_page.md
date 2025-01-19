## [How do I modify the url without reloading the page](#how-do-i-modify-the-url-without-reloading-the-page)

### How do I modify the url without reloading the page?

You can modify the URL without reloading the page using the `history.pushState()` or `history.replaceState()` methods. These methods allow you to change the URL in the browser without triggering a page reload.

Example using `pushState`:

```javascript
history.pushState(null, '', '/new-url');
console.log(window.location.href); // '/new-url'
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [URL manipulation](./theme/url_manipulation)


