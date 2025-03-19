[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner2-direct.svg)](https://stand-with-ukraine.pp.ua)

# ConnectyCube Android SDK Releases

This repository contains binary distributions of Android products released by ConnectyCube.

If you have any questions, comments, or issues related to any products distributed via this repository then please raise an issue here on GitHub repository or contact the team by emailing [support@connectycube.com](mailto:support@connectycube.com).

## ConnectyCube SDK

This repository contains releases of the Android SDK for interacting with the ConnectyCube communications cloud.

It provides a simple interface to the messaging, video calling (WebRTC), push notifications, users management and cloud files storage capabilities provided by the platform. 

[Getting Started with ConnectyCube Android SDK](https://developers.connectycube.com/android/)

## Installation

The ConnectyCube Android SDK can be installed directly into your application by importing sdk artifacts via Gradle.

Add the following code to your project's **build.gradle** file:

```groovy
allprojects {
    repositories {
        maven {
            url "https://github.com/ConnectyCube/connectycube-android-sdk-releases/raw/master/"
        }
    }
}

```

And the following code to your **module's** `build.gradle` file:

For **V2** :

```groovy
def sdkVersion = '2.0.0'

dependencies {
implementation "com.connectycube.sdk:connectycube-android:$sdkVersion"
}

```

For **V1** :

```groovy
def sdkVersion = '1.9.2'

dependencies {
    //
    implementation "com.connectycube:connectycube-android-sdk-chat:$sdkVersion" // all transitive modules will be included automatically
    implementation "com.connectycube:connectycube-android-sdk-videochat:$sdkVersion"
    implementation "com.connectycube:connectycube-android-sdk-storage:$sdkVersion"
    implementation "com.connectycube:connectycube-android-sdk-pushnotifications:$sdkVersion"
}
```

## Have an issue?

Join our [Discord](https://discord.com/invite/zqbBWNCCFJ) for quick answers to your questions

## Community

- [Blog](https://connectycube.com/blog)
- X (twitter)[@ConnectyCube](https://x.com/ConnectyCube)
- [Facebook](https://www.facebook.com/ConnectyCube)

**Want to support our team**:<br>
<a href="https://www.buymeacoffee.com/connectycube" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

# License 

ConnectyCube SDK for Android is licensed under the ConnectyCube SDK License.
