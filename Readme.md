# Android Scripts

This repository contains a collection of useful scripts for developing, testing and exploring Android apps on a Mac. They make tasks like getting a screenshot or video from your Android device as quick as clicking a button.

It automates:
* Taking a screenshot from the currently connected phone and downloading it to your Desktop
* Record a video from the currently connected phone, stop it by pressing Ctrl+C, and it will be downloaded to your Desktop
* Clear all app data from a specified application package name to test the innitial startup behavior
* Uninstall an app completely
* Run the Application Exerciser Monkey for a specified package name

I use them a lot in my daily routine, especially for augmenting bug reports with screenshots and videos, discussing design, and clearing App Data for having a clean application state.

### Prerequisites

You need to have an Android Development Environment set up before using the scripts. Specifically, the adb command has to be available on your PATH.

### Install

If you haven't done so already, head over to the [Android Studio Website](https://developer.android.com/studio/index.html) and install the SDK as described.

You should keep the script folder in a place that is easily accessible. I like to keep it in the dock of my Mac:

![script folder in dock](script_in_doc.png)

## Use

If you have everything set up as described, you just need to click (or double-click) on a script to make it run. If you want to set up a specific app, use the scripts in scripts/app_specific folder. Create a copy of the folder with the package name of your application:

```
cp -r app_specific/ com.your.application
```

The app specific scripts will use the last folder name as package name of the application.

## Author

* **Ulrich Scheller** - *Initial work* - [Website](https://www.ulrich-scheller.de/)
