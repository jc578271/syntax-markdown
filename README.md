# syntax-markdown

* Podfile: `ruby`
```ruby
require_relative '../node_modules/react-native/scripts/react_native_pods'
require_relative '../node_modules/@react-native-community/cli-platform-ios/native_modules'

platform :ios, '12.4'
install! 'cocoapods', :deterministic_uuids => false

```

-------------------------------------------
* AppDelegate.mm: `objectivec`
```objectivec
#import <Firebase.h>
#import "AppDelegate.h"

#import <React/RCTBridge.h>
#import <React/RCTBundleURLProvider.h>
#import <React/RCTRootView.h>

#import <React/RCTAppSetupUtils.h>
```

-------------------------------------------
* Info.plist: `xml`
```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
  <key>CFBundleDevelopmentRegion</key>
  <string>en</string>
</dict>
</plist>

```

-------------------------------------------
* Build.gradle: `source.groovy.gradle`
```source.groovy.gradle
buildscript {
    ext {
        buildToolsVersion = "31.0.0"
        minSdkVersion = 21
        compileSdkVersion = 31
        targetSdkVersion = 31

    }
```

--------------------------------------------
* AndroidManifest.xml: `xml`
```xml
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
  package="com.basicproject">

    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.SYSTEM_ALERT_WINDOW"/>
    <uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
```

---------------------------------------------
* MainAppication.java: `java`
```java
public class MainApplication extends Application implements ReactApplication {

  private final ReactNativeHost mReactNativeHost =
      new ReactNativeHost(this) {
        @Override
        public boolean getUseDeveloperSupport() {
          return BuildConfig.DEBUG;
        }
```
