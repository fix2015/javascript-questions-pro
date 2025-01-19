## [What are the common use cases of observables](#what-are-the-common-use-cases-of-observables)

### What are the common use cases of Observables?

Observables are useful for handling asynchronous events and streams of data. Common use cases include:

- Handling multiple values over time (e.g., user inputs, WebSocket data, server responses)
- Managing asynchronous sequences, like HTTP requests or animations
- Implementing reactive programming patterns

Example using RxJS for handling HTTP requests:

```javascript
import { of } from 'rxjs';

of('Data loaded').subscribe(data => console.log(data));
```

**Tags**: advanced, JavaScript, RxJS


