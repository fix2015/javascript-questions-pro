## [How do you perform form validation using JavaScript](#how-do-you-perform-form-validation-using-javascript)

### How do you perform form validation using JavaScript?

Form validation in JavaScript can be performed by adding event listeners to the form elements and checking their values before submitting the form. You can use the `onsubmit` event or validate individual fields using the `oninput` or `onchange` events.

Example:

```javascript
const form = document.getElementById('myForm');
form.onsubmit = function(event) {
  const email = document.getElementById('email').value;
  if (!email.includes('@')) {
    alert('Please enter a valid email address');
    event.preventDefault();
  }
};
```

**Tags**: intermediate, JavaScript, forms


