# New to Flutter?
Let's get started with setting up the workspace and installations.

## System Requirement
To install and run Flutter, your development environment must meet these minimum requirements:

* **Operating Systems:** MacOS,Linux (64-bit) or Windows // We'll be working on rhel-8

* **Disk Space:** 600 MB (does not include disk space for IDE/tools).

* **Tools:** Flutter depends on these command-line tools being available in your environment like bash, curl, 
file, git 2.x, mkdir, rm, unzip, which, xz-utils, zip

* **Shared libraries:** Flutter test command depends on this library being available in your environment.

* **libGLU.so.1 -** provided by mesa packages such as libglu1-mesa on Ubuntu/Debian and mesa-libGLU on Fedora.

## Installing Rhel-8
Download rhel-8 from [here](https://drive.google.com/file/d/1nZVXCVOy41LjAyOAiHMcNgFIwUlJYw16/view).

Also follow this amazing [rhel installation tutorial](https://youtu.be/JBNvnINsswo) by the founder of Linux World and RHCSA-level-22 Mr. [Vimal Daga](https://in.linkedin.com/in/vimaldaga) for technical insights while installation.

## Get the Flutter SDK
1.  Download the following installation bundle to get the latest stable release of the Flutter SDK from [here](https://flutter.dev/docs/get-started/install/linux)
2.  Extract the file in the desired location, for example:
```
$ cd ~/development
$ tar xf ~/Downloads/flutter_linux_1.17.5-stable.tar.xz
```
3.  Add the flutter tool to your path:
```
$ export PATH="$PATH:`pwd`/flutter/bin"
```

This command sets your PATH variable for the current terminal window only.


## Android Setup

Flutter relies on a full installation of Android Studio to supply its Android platform dependencies like emulator. However, you can write your Flutter apps in a number of editors; a later step discusses where we'll be writing in VSCode and use the emulator of android studio.
1.  Download and install [Android Studio](https://developer.android.com/studio#downloads).
2.  Start Android Studio, and go through the ‘Android Studio Setup Wizard’. This installs the latest Android SDK, Android SDK Command-line Tools, and Android SDK Build-Tools, which are required by Flutter when developing for Android.


We'll start with the installation of the Operating System 
follow this https://youtu.be/JBNvnINsswo
vs https://code.visualstudio.com/docs/?dv=linux64_rpm

andoid studio 

flutter sdk https://flutter.dev/docs/get-started/install/linux

rhel 8 https://drive.google.com/file/d/1nZVXCVOy41LjAyOAiHMcNgFIwUlJYw16/view
