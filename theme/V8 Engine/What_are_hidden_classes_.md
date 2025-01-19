## [What are hidden classes?](#what-are-hidden-classes)

### What are hidden classes?

Hidden classes are an optimization technique used by JavaScript engines like V8 to enhance object property access performance. Instead of directly associating objects with their properties, the engine creates a hidden class to represent the object's structure.

#### Key Points:
1. **Dynamic Nature of JavaScript Objects:**
   - JavaScript objects can have properties added or removed dynamically, making static optimization challenging.

2. **Hidden Class Mechanism:**
   - When an object is created, a hidden class is assigned to it.
   - Adding or removing properties results in the creation of a new hidden class.

3. **Optimization:**
   - If objects share the same hidden class, the engine can use fast property lookups.

Example:
```javascript
function Example() {
  this.a = 1;
  this.b = 2;
}

const obj1 = new Example();
const obj2 = new Example();
// Both obj1 and obj2 share the same hidden class.
```

**Tags**: advanced, JavaScript, V8 Engine


