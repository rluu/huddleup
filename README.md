Huddle Up
=========

#### Description:

Huddle Up is a mobile applicaction which allows users to locate nearby bars and drink deals.  This app is written in Javascript with Apache Cordova.


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

#### Steps for building this project on Windows 8 to deploy to the wp8 platform


#### Initial steps taken to create the Cordova project.


