## [Is Node.js completely single threaded](#is-nodejs-completely-single-threaded)

### Is Node.js completely single threaded?

No, Node.js is not completely single-threaded. While the event loop and most of the JavaScript code execution are single-threaded, Node.js uses multiple threads for I/O operations and certain asynchronous tasks. For example, it uses the libuv library to handle file system operations and network requests in parallel.

However, JavaScript code execution in Node.js runs on a single thread, making it lightweight and efficient for handling I/O-bound tasks.

**Tags**: intermediate, Node.js, JavaScript


