# Use `postMessage` API to send messages to Service Worker

Assuming your page is controlled by a Service Woker, you can access it via the `navigator.serviceWorker.controller` property and use the `postMessage` API to send a message.

```js
navigator.serviceWorker.controller.postMessage({myMessage: "hello"});
```

Inside your service worker code, you can listen for that message with:

```js
self.addEventListener('message', (event) => {
  // ...
})
```

See service worker [documentation](https://developer.mozilla.org/en-US/docs/Web/API/ServiceWorkerContainer).