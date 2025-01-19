## [What is a proxy object](#what-is-a-proxy-object)

### What is a proxy object?

A Proxy object is used to define custom behavior for fundamental operations (e.g., property lookup, assignment, function invocation) on another object. It is used for tasks like validation, logging, or access control.

Example:

```javascript
const person = {
  name: 'John'
};
const handler = {
  get: function(target, prop) {
    if (prop === 'name') {
      return 'Jane';
    }
    return prop;
  }
};
const proxyPerson = new Proxy(person, handler);
console.log(proxyPerson.name); // 'Jane'
```

**Tags**: basic, JavaScript, objects

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7458050469735320865](https://www.tiktok.com/@jsmentoring/photo/7458050469735320865)
