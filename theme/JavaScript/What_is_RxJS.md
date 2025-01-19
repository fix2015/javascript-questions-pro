## [What is RxJS](#what-is-rxjs)

### What is RxJS?

RxJS (Reactive Extensions for JavaScript) is a library for reactive programming using Observables. It enables you to compose asynchronous and event-based programs using operators like `map`, `filter`, `merge`, and more.

RxJS allows you to work with streams of data in a declarative manner, making it easier to manage complex asynchronous flows.

Example:

```javascript
import { from } from 'rxjs';
from([1, 2, 3]).subscribe(x => console.log(x));
```

**Tags**: advanced, JavaScript, RxJS


