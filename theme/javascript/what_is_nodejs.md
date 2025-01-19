## [What is nodejs](#what-is-nodejs)

### What is Node.js?

Node.js is a JavaScript runtime built on Chrome's V8 JavaScript engine. It allows developers to run JavaScript code outside of a browser, typically for building server-side applications.

Example:

```javascript
// A simple Node.js server
const http = require('http');
const server = http.createServer((req, res) => {
  res.write('Hello, world!');
  res.end();
});
server.listen(3000);
```

**Tags**: basic, JavaScript, runtime


