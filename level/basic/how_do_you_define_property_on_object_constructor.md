## [How do you define property on Object constructor](#how-do-you-define-property-on-object-constructor)

### How do you define property on Object constructor?

You can define properties on an object constructor by adding properties directly within the constructor function.

Example:

```javascript
function Person(name, age) {
  this.name = name;
  this.age = age;
}
const person = new Person('John', 30);
console.log(person.name); // 'John'
console.log(person.age); // 30
```

**Tags**: basic, JavaScript, objects


