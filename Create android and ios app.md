#IOS & ANDROID Application compile locally using cordova

### Pre requirements 
```sh
1. Download Java JDK
http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html (for Windows)
2. Android JDK tools or Android studio
3.0. Require if you installed Android JDK tools(Open Android SDK manager and select next options):
3.1. "SDK Platform" for android-23
3.2. "Android SDK Platform-tools" (latest)
3.3. "Android SDK Build-tools" (latest)
```

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


