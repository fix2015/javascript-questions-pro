## [What is the precedence order between local and global variables](#what-is-the-precedence-order-between-local-and-global-variables)

### What is the precedence order between local and global variables?

In JavaScript, when a variable is declared both globally and locally, the local variable takes precedence over the global variable within the function scope.

Example:

```javascript
let name = 'Global';
function greet() {
  let name = 'Local';
  console.log(name); // 'Local'
}
greet();
console.log(name); // 'Global'
```

**Tags**: [basic](./level/basic), [JavaScript](./theme/javascript), [variables](./theme/variables)


