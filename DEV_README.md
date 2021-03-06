# Airship Flutter Development

### Dev Environment
1. Install tools:
  - Android Studio
  - [Flutter](https://flutter.dev/docs/get-started/install)
  - Android studio flutter plugin

2. Make sure flutter is in the tool chain

3. Make sure flutter doctor to make sure everything is setup

### Plugin Development

1. Open the root of the project in Android Studio

2. Follow getting started guide to add the airship config and google-services.json to the `example` project

2. To edit the iOS plugin, in Android Studio right click `iOS` and click flutter -> Open iOS module in Xcode

3. To edit Android plugin in Android Studio right click `android` and click flutter -> Open Android module in Android Studio


### Plugin Structure

`android` android library module
`ios` iOS library module
`lib` plugin's dart implementation
`example` example app

Flutter communicates bidirectionally with the native layer though channels. `MethodChannels` are used
to initiate communication from dart -> native, and `EventChannel` from native -> dart.

### Troubleshooting

#### Xcode build errors

You may have to build and deploy the plugin from Android Studio before opening it in Xcode. This will trigger all the pod installs.

#### Android red symbols

If you see red symbols, you probably need to open the Android module in Android studio using the flutter tool outlined above. This will open it up as an Android project instead of flutter.



