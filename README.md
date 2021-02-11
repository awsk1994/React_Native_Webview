# React Native Webview Example

## Library Used
 - https://github.com/awsk1994/React_Native_Webview_Example

## Steps
1. npm install --save react-native-webview
2. Might need to link app: read https://github.com/react-native-webview/react-native-webview/blob/master/docs/Getting-Started.md
3. Add component:
```js
<WebView
  source={{ uri: 'https://infinite.red' }}
  style={{ marginTop: 20 }}
/>
```

<img src="./img/example.jpg" height="300px"/>

### Solution to Flipper-Folly problem

1. This issue is caused by an update to the "Flipper-Folly" pod-spec. If you'd like to keep Flipper enabled, you can override the version in your Podfile:

```
cd ios
vim PodFile
replace use_flipper! with use_flipper!({ 'Flipper-Folly' => '2.3.0' })
```

 - Source: https://github.com/facebook/react-native/issues/30836

2. rm -rf PodFile.lock -> pod install

Source: https://github.com/invertase/react-native-firebase/issues/3673