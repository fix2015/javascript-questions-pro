## [How Do You Receive Server-Sent Event Notifications?](#how-do-you-receive-server-sent-event-notifications)

### How Do You Receive Server-Sent Event Notifications?

To receive Server-Sent Event (SSE) notifications, you need to create an `EventSource` object in JavaScript, which listens for events sent by the server. For example:

```javascript
const eventSource = new EventSource('https://example.com/sse');
eventSource.onmessage = function(event) {
  console.log('New message:', event.data);
};
```

**Tags**: [intermediate](./level/intermediate), [Server-Sent Events](./theme/server_sent_events), [notifications](./theme/notifications), [web technologies](./theme/web_technologies)

**URL**: [https://www.tiktok.com/@jsmentoring/photo/7448989685881376033](https://www.tiktok.com/@jsmentoring/photo/7448989685881376033)
