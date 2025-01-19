## [Give an example of a web worker?](#give-an-example-of-a-web-worker)

### Give an example of a web worker?

A simple web worker example:

```javascript
const worker = new Worker('worker.js');
worker.postMessage('Hello');
worker.onmessage = function(event) {
  console.log('Received from worker:', event.data);
};
```
In the `worker.js` file, you would handle the message with `onmessage` and use `postMessage` to send a response back.

**Tags**: intermediate, web workers, JavaScript

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7448739040213437729](https://www.tiktok.com/@jsmentoring/photo/7448739040213437729)
