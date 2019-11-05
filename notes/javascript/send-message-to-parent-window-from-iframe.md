# Send message to parent window from iframe or popup

Browsers provide the `window.postMessage` API for sending simple messages from an iframe to the parent window.  

To send a message:
```javascript
  window.parent.postMessage(JSON.stringify({ 
    src: window.location.toString(), 
    context: 'iframe.resize', 
  }), '*');
```

To listen for a message:
```javascript
window.addEventListener("message", function(e) { 
  console.log(e) 
}, false);
```

Read the [MDN documentation](https://developer.mozilla.org/en-US/docs/Web/API/Window/postMessage). Beware of the security implications.