## [What are Snapshot Tests in Jest?](#what-are-snapshot-tests-in-jest)

### What are Snapshot Tests in Jest?

Snapshot tests in Jest allow you to test whether a component's output changes over time. It generates a snapshot of the component’s output and stores it. On subsequent runs, Jest compares the output to the stored snapshot to detect changes.

Example:

```javascript
import MyComponent from './MyComponent';
import { render } from '@testing-library/react';
import { toMatchSnapshot } from 'jest-snapshot';

it('matches snapshot', () => {
  const { container } = render(<MyComponent />);
  expect(container).toMatchSnapshot();
});
```

**Tags**: [intermediate](./level/intermediate), [Jest](./theme/jest), [Snapshot Testing](./theme/snapshot_testing)


