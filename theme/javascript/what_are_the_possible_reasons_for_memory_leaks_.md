## [What are the possible reasons for memory leaks?](#what-are-the-possible-reasons-for-memory-leaks)

### What are the possible reasons for memory leaks?

1. **Global Variables:**
   ```javascript
   var leak = 'This is a memory leak';
   ```

2. **Uncleared Intervals/Timeouts:**
   ```javascript
   setInterval(() => console.log('Leaking memory'), 1000);
   ```

3. **Detached DOM Nodes:**
   ```javascript
   const element = document.getElementById('myElement');
   element.parentNode.removeChild(element); // Still referenced in memory
   ```

4. **Closures Holding References:**
   ```javascript
   function leak() {
     let bigArray = new Array(1000000);
     return function() {
       console.log(bigArray);
     };
   }
   ```

**Tags**: advanced, JavaScript, Performance


