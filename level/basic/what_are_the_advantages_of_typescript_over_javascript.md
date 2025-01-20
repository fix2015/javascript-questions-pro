## [What are the advantages of TypeScript over JavaScript](#what-are-the-advantages-of-typescript-over-javascript)

### What are the advantages of TypeScript over JavaScript?

TypeScript offers several advantages over JavaScript:
- **Static typing** helps catch errors early during development.
- **Better tooling support** with autocompletion and code refactoring.
- **Type inference** improves developer productivity and reduces errors.
- **Support for modern JavaScript features** like async/await, decorators, etc., even in older browsers when transpiled.

Example:

```typescript
function greet(person: string) {
  console.log(`Hello, ${person}`);
}
greet(42); // Error: Argument of type 'number' is not assignable to parameter of type 'string'.
```

**Tags**: [basic](./level/basic), [TypeScript](./theme/typescript)


