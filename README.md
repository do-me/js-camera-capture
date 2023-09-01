# js-camera-capture

Vanilla JS camera capture example, working on desktop and mobile based on navigator.mediaDevices.getUserMedia().

Designed as a basic user interface example for taking a picture and sending it to some server, here the [ntfy](https://ntfy.sh/) channel: [https://ntfy.sh/js-camera-capture](https://ntfy.sh/js-camera-capture)

There are two versions.

## Simple Version
This version displays the video stream canvas directly to the html body (which might be good for testing and simple stuff). Pretty much without CSS modifications.

![image](https://github.com/do-me/js-camera-capture/assets/47481567/eb03dd4b-7458-4e99-accf-2a63a6030df0)

## Modal Version 
For more realistic use cases. `Activate Camera` opens a modal with the canvas. The buttons have some basic styling.

![image](https://github.com/do-me/js-camera-capture/assets/47481567/b9d45501-5cc7-410c-9ee3-6ea2300e231d)

## Options

If you'd like to activate the front camera on mobile as default (instead of the rear one) use the `facingMode: 'user'` instead of `facingMode: 'environment'`: 

```javascript
stream = await navigator.mediaDevices.getUserMedia({ video: { facingMode: 'user' } });
```

## Collaboration

PR's are very welcome, especially for enhancing the UI or adding more features. However, the codebase should be kept:
- simple
- small
