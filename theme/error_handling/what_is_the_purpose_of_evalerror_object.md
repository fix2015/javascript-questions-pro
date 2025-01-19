## [What is the purpose of EvalError object](#what-is-the-purpose-of-evalerror-object)

### What is the purpose of EvalError object?

`EvalError` is an error object that is thrown when an issue occurs with the `eval()` function. It is rarely used today as `eval()` is generally avoided due to security concerns. The `EvalError` object provides information about errors related to code evaluation.

Example:

```javascript
try {
  throw new EvalError('Eval error');
} catch (e) {
  console.log(e.message);  // Output: Eval error
}
```

**Tags**: intermediate, JavaScript, Error Handling


