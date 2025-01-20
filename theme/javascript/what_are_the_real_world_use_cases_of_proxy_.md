## [What are the real world use cases of proxy?](#what-are-the-real-world-use-cases-of-proxy)

### What are the real-world use cases of Proxy?

1. **Validation:**
   ```javascript
   const validator = {
     set(obj, prop, value) {
       if (prop === 'age' && typeof value !== 'number') {
         throw new Error('Age must be a number');
       }
       obj[prop] = value;
       return true;
     }
   };
   const person = new Proxy({}, validator);
   person.age = 25; // Valid
   person.age = 'twenty'; // Throws Error
   ```

2. **Property Access Control:**
   ```javascript
   const handler = {
     get(target, prop) {
       return prop in target ? target[prop] : 'Property does not exist';
     }
   };
   const obj = new Proxy({}, handler);
   console.log(obj.name); // 'Property does not exist'
   ```

3. **Performance Optimization:**
   - Proxy can be used to lazy-load properties or cache data dynamically.

**Tags**: [advanced](./level/advanced), [JavaScript](./theme/javascript), [Proxy](./theme/proxy)


