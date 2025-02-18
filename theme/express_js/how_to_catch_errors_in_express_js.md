## [How to catch errors in Express.js](#how-to-catch-errors-in-expressjs)

### How to catch errors in Express.js

Use middleware to catch and handle errors in your Express applications.

```javascript
const express = require('express');
const app = express();

// Your routes here
app.get('/', (req, res) => {
  throw new Error('Oops!');
});

// Error handling middleware
app.use((err, req, res, next) => {
  console.error(err.stack);
  res.status(500).send('Something broke!');
});

app.listen(3000, () => console.log('Server running on port 3000'));
```

**Tags**: [intermediate](./level/intermediate), [JavaScript](./theme/javascript), [Express.js](./theme/express_js), [Error Handling](./theme/error_handling)


