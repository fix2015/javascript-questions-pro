## [How Do You Detect Caps Lock Key Turned On or Not?](#how-do-you-detect-caps-lock-key-turned-on-or-not)

### How Do You Detect Caps Lock Key Turned On or Not?

To detect whether Caps Lock is on, you can use the `keydown` or `keypress` event and check the `event.getModifierState('CapsLock')` property.

```javascript
document.addEventListener('keydown', function(event) {
  if (event.getModifierState('CapsLock')) {
    console.log('Caps Lock is on');
  }
});
```

**Tags**: intermediate, JavaScript, event handling, keyboard events

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7449671849920761120](https://www.tiktok.com/@jsmentoring/photo/7449671849920761120)
