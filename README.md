### this is a fork of pushy-receiver plugin, it should work with

>>> @fcarreno/cordova-plugin-intent@1.0.9

1. on server, send your message with payload

```js
pushy.sendPushNotification({ payload: 'string os jsonstring' })
```

2. on client register your event

window.plugins.intentShim.onIntent(intent => {
  console.log(intent.extras.payload)
})
