# js-camera-capture

Vanilla JS camera capture example, working on desktop and mobile based on navigator.mediaDevices.getUserMedia().

Desgined as a basic user interface example for taking a picture and sending it to some server, here the [ntfy](https://ntfy.sh/) channel: [https://ntfy.sh/js-camera-capture](https://ntfy.sh/js-camera-capture)

If you'd like to activate the front camera on mobile as default use a different `facingMode`: 

```javascript
stream = await navigator.mediaDevices.getUserMedia({ video: { facingMode: 'user' } });
```

![image](https://github.com/do-me/js-camera-capture/assets/47481567/eb03dd4b-7458-4e99-accf-2a63a6030df0)
