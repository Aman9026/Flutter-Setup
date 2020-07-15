![](https://github.com/Aman9026/Flutter-Setup/blob/master/Data/flut.jpeg)
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
![](https://github.com/Aman9026/Flutter-Setup/blob/master/Data/RHEL_8_Desktop.png)
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
To make it permanent and run flutter commands in any terminal session follow next steps for modifying 
this variable permanently for all terminal sessions are machine-specific. 
Typically you add a line to a file that is executed whenever you open a new window. For example:

1. Determine the directory where you placed the Flutter SDK. You need this in Step 3.
2. Open (or create) the rc file for your shell. For example, Linux uses the Bash shell by default, so edit $HOME/.bashrc. 
If you are using a different shell, the file path and filename will be different on your machine.
3. Add the following line and change [PATH_TO_FLUTTER_GIT_DIRECTORY] to be the path where you cloned Flutter’s git repo:
```
$ export PATH="$PATH:[PATH_TO_FLUTTER_GIT_DIRECTORY]/flutter/bin"
```
4. Run ```source $HOME/.<rc file>``` to refresh the current window, or open a new terminal window to automatically source the file.

Else you can also do the same thing in /etc/profile if you have administrator privileges.

### Run the Doctor
Run the following command to see if there are any dependencies you need to install to complete the setup (for verbose output, add the -v flag):
```
$ flutter doctor -v
```
This command checks your environment and displays a report to the terminal window. The Dart SDK is bundled with Flutter; 
it is not necessary to install Dart separately.
Once you have installed any missing dependencies, run the ```$ flutter doctor``` command again to verify that you’ve set everything up correctly.

Basically by using the doctor option you can check if we need to install further dependencies.

## Android Setup

Flutter relies on a full installation of Android Studio to supply its Android platform dependencies like emulator. However, you can write your Flutter apps in a number of editors; a later step discusses where we'll be writing in VSCode and use the emulator of android studio.
1.  Download and install [Android Studio](https://developer.android.com/studio#downloads).
2.  Start Android Studio, and go through the ‘Android Studio Setup Wizard’. This installs the latest Android SDK, Android SDK Command-line Tools, and Android SDK Build-Tools, which are required by Flutter when developing for Android.

### Add Dart Plugin to Android Studio
If you prefer to use Android Studio as your main IDE to develop Flutter, you have to set dart language support to Android Studio as shown below.

Preferences → Plugins → Browse Repository → type Dart in search bar → Install and Restart android studio.

### Add Flutter Plugin to Android Studio

Preferences → Plugins → Browse Repository → type Flutter in search bar → Install and Restart android studio.

## Set up the Android emulator
![](https://github.com/Aman9026/Flutter-Setup/blob/master/Data/ezgif.com-video-to-gif%20(1).gif)

To prepare to run and test your Flutter app on the Android emulator, follow these steps:
![](https://miro.medium.com/max/700/1*Nz0C7NC0wR73z7KcPhUVrg.gif)
* Tools → AVD Manager → Opens a window

* Select → Create Virtual Device

* Phone → [Choose Any] → [Choose System Image, typically the highest one is most preferred] → Android 8.1 → AVD Name(Pixel 2 API 27)

* Choose Graphics → Hardware → Finish

* Select Pixel 2 API 27 emulator → click on Launch AVD(start) button


## VSCode

This IDE is quite handy for managing dart code and can be easily integrated with the android emulator.

Download Visual Studio Code from [here](https://code.visualstudio.com/download), Then switch to the extension tab and search for “flutter”:
![](https://github.com/Aman9026/Flutter-Setup/blob/master/Data/0_I5vq797d25fPZ5nT.png)

The first entry in the search result list is the extension we’re looking for. 
By installing this extension we’re adding support for editing, refactoring, running, 
and reloading Flutter application, as well as support for the Dart programming language.

---

*Happy Fluttering!* :heartbeat:

***You are always welcome to add more or improve any resource in this repository by following [these](https://github.com/Aman9026/Flutter-Setup/blob/master/CONTRIBUTING.md) instructions.***
