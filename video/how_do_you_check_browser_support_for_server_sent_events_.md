## [How Do You Check Browser Support for Server-Sent Events?](#how-do-you-check-browser-support-for-server-sent-events)

### How Do You Check Browser Support for Server-Sent Events?

To check if the browser supports Server-Sent Events, you can check for the `EventSource` object:

```javascript
if (typeof(EventSource) !== 'undefined') {
  // SSE is supported
} else {
  // SSE is not supported
}
```

**Tags**: [basic](./level/basic), [Server-Sent Events](./theme/server_sent_events), [browser support](./theme/browser_support)

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7449149383142018336](https://www.tiktok.com/@jsmentoring/photo/7449149383142018336)
