## [What are the uses of closures?](#what-are-the-uses-of-closures)

### What are the uses of closures?

Closures allow a function to retain access to its outer scope, even after the outer function has returned. Common uses include:

1. **Data Encapsulation:**
   ```javascript
   function counter() {
     let count = 0;
     return function() {
       return ++count;
     };
   }
   const increment = counter();
   console.log(increment()); // 1
   console.log(increment()); // 2
   ```

2. **Event Handlers:**
   ```javascript
   function setupEventListener() {
     let name = 'ClickMe';
     document.addEventListener('click', function() {
       console.log(`Button ${name} clicked`);
     });
   }
   setupEventListener();
   ```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Closures](./theme/closures)


