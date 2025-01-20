## [How do you create custom HTML element?](#how-do-you-create-custom-html-element)

### How do you create custom HTML element?

You can create a custom HTML element using the `customElements.define` method. Here's an example:

```javascript
class MyElement extends HTMLElement {
  constructor() {
    super();
    this.innerHTML = '<p>Hello, Custom Element!</p>';
  }
}

customElements.define('my-element', MyElement);

// Usage in HTML:
// <my-element></my-element>
```

This defines a new custom element `<my-element>` which can be used like a standard HTML tag.

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Web Components](./theme/web_components)


