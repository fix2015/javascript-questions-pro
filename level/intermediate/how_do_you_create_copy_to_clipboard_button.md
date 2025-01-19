## [How do you create copy to clipboard button](#how-do-you-create-copy-to-clipboard-button)

### How do you create copy to clipboard button?

You can create a 'copy to clipboard' button using the `document.execCommand('copy')` method. However, modern browsers prefer using the `Clipboard API` for better security and compatibility.

Example using `Clipboard API`:

```javascript
let copyButton = document.querySelector('#copyButton');
let textToCopy = document.querySelector('#textToCopy');

copyButton.addEventListener('click', () => {
  navigator.clipboard.writeText(textToCopy.textContent)
    .then(() => { console.log('Text copied to clipboard!'); })
    .catch(err => { console.log('Failed to copy text:', err); });
});
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [DOM](./theme/dom)


