## [How do you copy properties from one object to other](#how-do-you-copy-properties-from-one-object-to-other)

### How do you copy properties from one object to other?

You can copy properties from one object to another using `Object.assign()` or the spread operator.

Example using `Object.assign()`:

```javascript
const obj1 = { name: 'John' };
const obj2 = Object.assign({}, obj1);
console.log(obj2); // { name: 'John' }
```
Example using the spread operator:

```javascript
const obj2 = { ...obj1 };
console.log(obj2); // { name: 'John' }
```

**Tags**: basic, JavaScript, objects

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7458032154656673056](https://www.tiktok.com/@jsmentoring/photo/7458032154656673056)
