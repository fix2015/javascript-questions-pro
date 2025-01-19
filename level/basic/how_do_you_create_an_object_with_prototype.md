## [How do you create an object with prototype](#how-do-you-create-an-object-with-prototype)

### How do you create an object with prototype?

You can create an object with a prototype using `Object.create()`. This allows you to specify an existing object to serve as the prototype for the new object.

Example:

```javascript
const person = { greet() { console.log('Hello'); } };
const student = Object.create(person);
student.greet(); // 'Hello'
```

**Tags**: basic, JavaScript, objects

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7458574988463983904](https://www.tiktok.com/@jsmentoring/photo/7458574988463983904)
