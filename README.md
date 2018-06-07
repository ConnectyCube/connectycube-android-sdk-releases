# ConnectyCube Android SDK Releases

This repository contains binary distributions of Android products released by ConnectyCube.

If you have any questions, comments, or issues related to any products distributed via this repository then please raise an issue here on GitHub repository or contact the team by emailing support@connectycube.com.

# ConnectyCube SDK

This repository contains releases of the Android SDK for interacting with the ConnectyCube communications cloud.

It provides a simple interface to the messaging, video calling (WebRTC), push notifications, users management and cloud files storage capabilities provided by the platform. 

# Installation

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

def sdkVersion = '1.0.0'
```

And the following code to your **module's** `build.gradle` file:

```groovy
dependencies {
    //
    сompile "com.connectycube:connectycube-android-sdk-chat:$rootProject.sdkVersion" // all transitive modules will be included automatically
    сompile "com.connectycube:connectycube-android-sdk-videochat-webrtc:$rootProject.sdkVersion"
    сompile "com.connectycube:connectycube-android-sdk-storage:$rootProject.sdkVersion"
    сompile "com.connectycube:connectycube-android-sdk-pushnotifications:$rootProject.sdkVersion"
}
```

# Contact

You can reach the ConnectyCube team at any time by emailing [support@connectycube.com](mailto:support@connectycube.com).

# Licence 

ConnectyCube SDK for Android is licensed under the ConnectyCube SDK License.
