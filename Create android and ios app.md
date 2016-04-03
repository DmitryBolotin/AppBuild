#IOS & ANDROID Application compile locally using cordova

### Pre requirements

1. [Download Java JDK for Windows](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html  "Download Java JDK")
2. [Android JDK tools or Android studio](https://developer.android.com/sdk/index.html#download / "Android JDK tools or Android studio")

#####Require if you installed Android JDK tools
Open Android SDK manager and select next options
- SDK Platform for android-23
- Android SDK Platform-tools (latest)
- Android SDK Build-tools (latest)


### Requirements
  - Node.js 4+
  - Cordova 6+

### Installation
Need install cordova globally
```sh
$ npm i -g cordova@latest
```
Install Node.js
```sh
https://nodejs.org/en/download/stable/
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
### Icons
Icons & Splashes are placed in res folder. All icons are described in config.xml file.
Setting for icon:
<icon height="76" src="res/ios/icons/fg-76px.png" width="76" />
Setting for splash:
<splash height="480" src="res/ios/splash/640x960.png" width="320" />
readmore: https://cordova.apache.org/docs/en/latest/config_ref/images.html

#### iOS
Icons for ios are keep in res/ios folder.

####Add plugins
cordova plugin add {plugin name} --save

####Some cordova plugins
```
cordova-plugin-splashscreen - first screen logo displayed when you open app
cordova-plugin-transport-security - disable cross domain request
```


