#IOS & ANDROID Application compile locally using cordova

### Pre requirements

1. [Download Java JDK for Windows](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html  "Download Java JDK")
2. [Android JDK tools or Android studio](https://developer.android.com/sdk/index.html#download / "Android JDK tools or Android studio")

#####Require if you installed Android JDK tools
Open Android SDK manager and install next options
- SDK Platform for android-23
- Android SDK Platform-tools (latest)
- Android SDK Build-tools (latest)

### Requirements
  - Node.js 4+
  - Cordova 6+

### Installation
Install [Node.js](https://nodejs.org/en/download/stable/)

Need install cordova globally
```sh
$ npm i -g cordova@latest
```

Add platform:
```sh
cordova platform add ios --save
cordova platform add android --save
cordova platform add browser --save (open app in browser)
```

### Build for iOS

```sh
$ cordova create myApp
$ cordova build ios
$ cordova run ios
```

### Build for Android

```sh
$ cordova create myApp
$ cordova build android
$ cordova run android
```

####Add plugins
cordova plugin add {plugin name} --save

####Some cordova plugins
```
cordova-plugin-splashscreen - first screen logo displayed when you open app
cordova-plugin-transport-security - disable cross domain request
```


