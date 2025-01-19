## [What are the restrictions of web workers on DOM?](#what-are-the-restrictions-of-web-workers-on-dom)

### What are the restrictions of web workers on DOM?

Web workers run in a separate thread and cannot directly access or modify the DOM. They are designed for heavy computations and background tasks. To interact with the DOM, workers communicate with the main thread using message passing via `postMessage()`.

**Tags**: advanced, web workers, DOM, JavaScript

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7448725365574372641](https://www.tiktok.com/@jsmentoring/photo/7448725365574372641)
