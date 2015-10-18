Antox
=====

<img src="http://i.imgur.com/PvY7zCQ.jpg" width="230px" height="400px"/><img src="http://i.imgur.com/Hmnjpv3.png" width="230px" height="400px"/><img src="http://i.imgur.com/jApGiZQ.png" width="230px" height="400px"/>

Antox is an Android 2.3+ client for Tox. It aims to bring the full multimedia support Tox offers to your device, although it's still currently in heavy development. Antox is currently available for alpha testing on Google Play and F-Droid.

###Current development

I am too busy with my final year of university to continue working on Antox. You can find a maintained fork with new features being added [here](https://github.com/subliun/Antox).

###Getting Antox

To get Antox on Google Play, join the [Google+ Community](https://plus.google.com/communities/103125800027884896310), and follow the instructions given.

To get Antox on F-Droid, add https://antox.me/fdroid/repo to your repo list. Please note this repo and domain are not controlled by me.

###What Is Currently Working

- One to one messaging
- File transfers
- Avatars

###Translating Antox
You can localize the application via github pull request or by requesting a new language or join an existing translation team on [Transifex](https://www.transifex.com/projects/p/antox/). Please note that translation updates from Transifex are usually delayed.

###Compiling Antox From Source with IntelliJ IDE
- Download https://developer.android.com/sdk/installing/studio.html
- In Android Studio, go to Help>Check For Updates. As of writing, the latest version of AS is 0.8.1
- In Android Studio again, go to Tools>Android>SDK Manager. Make sure you're using the latest SDK tools and SDK Build tools.
- Clone the Antox repo
- To import the project, go to File>Import Project. Select the build.gradle file in the root of the Antox folder
- Download tox dependencies by running `./download-dependencies.sh`
- Install the Scala plugin in IntelliJ, restart, and wait for IntelliJ to set itself up
- Connect your phone in developer mode and click Run in Android Studio. It will install Antox on to your phone and run it automatically.

###Compiling Scala Antox From Source via CLI
- Download android sdk http://developer.android.com/sdk/index.html and unpack
- Set the environmental variable ANDROID_HOME to point to it
- Add $ANDROID_HOME/tools and $ANDROID_HOME/platform-tools to your PATH environmental variable
- run the command `android` and use it to install SDK Platform for API 10, and the latest SDK tools and SDK build tools, and Android Support Library
- Clone the Antox repo
- Download tox dependencies by running `./download-dependencies.sh`
- Connect your phone with USB in developer mode and run `./gradlew installDebug` from the root Antox directory. It will install Antox on to your phone, and you can now run it.
- Run `adb logcat` to display the logs of your USB connected phone, to read error messages and crash logs etc.


*The Android robot is reproduced or modified from work created and shared by Google and used according to terms described in the Creative Commons 3.0 Attribution License.*

