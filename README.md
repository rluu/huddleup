Huddle Up
=========

#### Description:

Huddle Up is a mobile applicaction which allows users to locate nearby bars and drink deals.  This app is written in Javascript with Apache Cordova.

**Important!** Huddle Up development has been suspended, 
and there have not been any releases available yet.
It is unclear when active development will continue.

#### Project contributors:

- Ryan Luu, ryanluu@gmail.com
- Avinash Kondagunta, akondagunta@gmail.com

#### Pre-requisites for building (for all platforms)

1. Install [Node.js](http://nodejs.org/).

2. Install [Apache Cordova](http://cordova.apache.org/):

  ```
npm install -g cordova
  ```


#### Steps for building this project on Mac OS X to deploy to the ios platform

These steps below assume that Apache Cordova has already been installed.

1. Install the most current version of [Xcode](https://developer.apple.com/xcode/).  As of 2014-12-07, this version is 6.1.1.  Apache Cordova requires at least version 4.6.  To determine what version of Xcode you have, run:

  ```
xcodebuild -version
  ```

  If you have just installed Xcode, make sure you also agree to the Xcode license, or else the project will encounter an error during the build.  Agreeing to the license can be done by opening Xcode.app and agreeing to the license within the GUI.  Agreeing to the license can also be done via the command-line by running the following (untested):

  ```
sudo xcrun cc
  ```

2. Install ios-sim:

  ```
npm install -g ios-sim
  ```

3. Clone the project repository from git.

  ```
git clone https://github.com/rluu/huddleup.git
  ```

4. Navigate to the project directory and add ios as a platform to build.

  ```
cd huddleup
cordova platform add ios
  ```

5. Build the project for the ios platform.

  ```
cordova build ios
  ```

6. Run the app in the ios emulator.

  ```
cordova emulate ios
  ```


#### Steps for building this project on Mac OS X to deploy to the Android platform

These steps below assume that Apache Cordova has already been installed.

1. Install [Android SDK](https://developer.android.com/sdk/).  The *Android Studio* SDK bundle is not required; the *Stand-alone SDK Tools* bundle is sufficient.

2. Extract the zip file to the filesystem.

  ```
unzip android-sdk_r23.0.2-macosx.zip
  ```

3. Change directory to the extracted directory.  Add the tools directory to the shell PATH environment variable so that the `android` and other tools can be run from other locations.

  ```
cd android-sdk-macosx
export ANDROID_SDK_TOOLS=/Users/rluu/installed/android-sdk-macosx/tools
export PATH=$ANDROID_SDK_TOOLS:$PATH
  ```

4. Run the *Android SDK Manager* by running `android` on the command-line.  From the *Android SDK Manager*, install the following items:

  - Tools:
    - Android SDK Tools
    - Android SDK Platform-tools
    - Android SDK Build-tools
  - Android 5.0 (API 21)
  - Android 4.4.2 (API 19)
  - Extras:
    - Android Support Library

  Installing all these tools and APIs should take a few hours.  When the installation is complete, you can close the *Android SDK Manager* application.

  Note: As of 2014-12-07, the most current version of Android is 5.0.  The most recent version of Apache Cordova only supports Android 4.4.2, so that is why we are installing Android 4.4.2.

5. Install [Apache Ant](http://ant.apache.org/).  You can get it either from the official website as a binary tarball, or you can use Macports or Homebrew.  Make sure that `ant` is accessible from the command-line PATH.

  ```
ant -version
  ```

6. Clone the project repository from git.

  ```
git clone https://github.com/rluu/huddleup.git
  ```

7. Navigate to the project directory and add android as a platform to build.

  ```
cd huddleup
cordova platform add android
  ```

8. Build the project for the android platform.

  ```
cordova build android
  ```

9. [TODO: Step 9 fails.  Need to add a step here to first create an Android AVD.]  Run the app in the android emulator.

  ```
cordova emulate android
  ```

#### Steps for building this project on Windows 8 to deploy to the wp8 platform


#### Initial steps taken to create the Cordova project.

