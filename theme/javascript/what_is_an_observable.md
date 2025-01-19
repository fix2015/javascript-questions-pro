## [What is an observable](#what-is-an-observable)

### What is an observable?

An Observable is a representation of a stream of values or events that can be observed over time. Observables are the core concept in reactive programming and are widely used in libraries like RxJS to manage asynchronous operations.

An observable can emit values, complete, or throw errors.

Example:

```javascript
import { Observable } from 'rxjs';

let observable = new Observable(observer => {
  observer.next('Hello');
  observer.complete();
});
observable.subscribe(value => console.log(value));

**Tags**: advanced, JavaScript, RxJS


