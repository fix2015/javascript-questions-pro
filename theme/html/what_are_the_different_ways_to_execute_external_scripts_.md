## [What are the different ways to execute external scripts?](#what-are-the-different-ways-to-execute-external-scripts)

### What are the different ways to execute external scripts?

1. **Using `<script>` Tag:**
   - Include the script in your HTML file.
   ```html
   <script src="script.js"></script>
   ```

2. **Dynamically Injecting Scripts:**
   - Use JavaScript to add scripts to the DOM.
   ```javascript
   const script = document.createElement('script');
   script.src = 'script.js';
   document.body.appendChild(script);
   ```

3. **Using `import` (ES Modules):**
   - Load scripts as ES modules.
   ```javascript
   import { myFunction } from './script.js';
   myFunction();
   ```

4. **Using `require` (Node.js):**
   - Load scripts in Node.js environments.
   ```javascript
   const module = require('./script.js');
   module.myFunction();
   ```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [HTML](./theme/html)


