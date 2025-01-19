## [How do you declare namespace](#how-do-you-declare-namespace)

### How do you declare namespace?

In JavaScript, namespaces are not natively supported, but you can simulate them using objects or modules. By declaring an object, you can encapsulate your functions and variables to avoid polluting the global scope.

Example using objects as namespaces:

```javascript
const MyNamespace = {
  myFunction: function() { console.log('Hello!'); },
  myVariable: 42
};
MyNamespace.myFunction(); // 'Hello!'
```

**Tags**: intermediate, JavaScript, namespaces


