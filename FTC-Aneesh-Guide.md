Requirements
-----------
- Java (SE v8)
- Android Studio (>v1)
- ftc_app (.zip)

Installation
------------
###Java
1. Download the latest version of Java from http://www.oracle.com/technetwork/java/javase/downloads/index.html. Make sure that you install both the JDK and the JRE. Follow default instructions when installing; don't change any settings.
<p align="center">
  <img src="https://github.com/Alaska47/FTC-Android-Installation-Notes/blob/master/images/java_installation.png?raw=true"/>
</p>

###Android Studio
1. Download the latest version of Android Studio along with SDK Tools from https://developer.android.com/studio/index.html. Follow all the default instructions when installing. If Android Studio asks you to open SDK Manager, do NOT open it yet. Do not check the box to open Android Studio yet.
<p align="center">
  <img src="https://github.com/Alaska47/FTC-Android-Installation-Notes/blob/master/images/android_studio_installation.png?raw=true"/>
</p>

###ftc_app
1. In order to use your FTC Robot, you need the official FTC SDK to program your robot. You can find the zip to download the FTC SDK from https://github.com/ftctechnh/ftc_app/archive/master.zip. Save the file to a place which you can easily access it from later, and where it won't be deleted accidentally (this is where you will store your robot's code as well). Unzip the file.
<p align="center">
  <img src="https://github.com/Alaska47/FTC-Android-Installation-Notes/blob/master/images/extract_ftc_app.PNG?raw=true"/>
</p>

Configuration
-------------
###Android Studio
1. Open up Android Studio. This should be your first time opening Android Studio. If it isn't, and you already have a project open, go to `File -> Close Project`. This should take you to the "Welcome Screen"
<p align="center">
  <img src="https://github.com/Alaska47/FTC-Android-Installation-Notes/blob/master/images/android_studio_welcome.png?raw=true"/>
</p>
2. Go to `Configure -> SDK Manager`. This will open up Android's SDK Manager where you can install packages that are necessary to run the ftc_app project. Next, go to the bottom right of the window and click on `Show Package Details`.
<p align="center">
  <img src="https://github.com/Alaska47/FTC-Android-Installation-Notes/blob/master/images/studio_sdk_manager.png?raw=true"/>
</p>
3. Make sure you install all the necessary packages that are described below.
    1. Select `Google APIs, Android 22`, `Android SDK Platform 22` under `Android 5.1 (Lollipop)`
    2. Select `Google APIs, Android 21`, `Android SDK Platform 21` under `Android 5.0 (Lollipop)`
<p align="center">
  <img src="https://github.com/Alaska47/FTC-Android-Installation-Notes/blob/master/images/packages_studio.png?raw=true"/>
</p>
4. Navigate to `SDK Tools` using the top bar.
    3. Select `Google USB Driver`, `Google Web Driver`, `Intel x86 Emulator Accelerator (HAXM installer` (optional)
<p align="center">
  <img src="https://github.com/Alaska47/FTC-Android-Installation-Notes/blob/master/images/packages_studio1.png?raw=true"/>
</p>
5. Click apply and wait for all the selected packages to install. After all the packages have installed, you can close the SDK Manager.
6. Once you are back at the "Welcome Screen", click on `Import project (Eclipse ADT, Gradle, etc.)`.
<p align="center">
  <img src="https://github.com/Alaska47/FTC-Android-Installation-Notes/blob/master/images/import_studio.png?raw=true"/>
</p>
7. Navigate to where you unzipped the ftc_app zip file. Wait for a couple seconds for the Grade icon to appear next to `ftc_app-master`. Once you have selected `ftc_app-master`, click `OK` and wait for the project to build, compile, and appear. 
<p align="center">
  <img src="https://github.com/Alaska47/FTC-Android-Installation-Notes/blob/master/images/gradle_import.png?raw=true"/>
</p>
8. If there are any error in compiling the project, in the bottom left corner, click on the links, and install any other packages that are needed.
<p align="center">
  <img src="https://github.com/Alaska47/FTC-Android-Installation-Notes/blob/master/images/error_grade.png?raw=true"/>
</p>
9. Finish and let the project recompile. If Android Studio notifies you about an out-of-date Gradle plugin, just click ignore.
10. Click on the `Project` tab on the left of the screen, then navigate through the directories as shown all the way to the `opmodes` folder.
<p align="center">
  <img src="https://github.com/Alaska47/FTC-Android-Installation-Notes/blob/master/images/opmodes.png?raw=true"/>
</p>
11. Right click on the `opmodes` folder, then click on `New -> Java Class`, type in `TestOpMode`, and click `OK`.
<p align="center">
  <img src="https://github.com/Alaska47/FTC-Android-Installation-Notes/blob/master/images/test_mode.png?raw=true"/>
</p>
12. Type in the code shown in the next image. This is a sample of a empty TeleOp mode template.
<p align="center">
  <img src="https://github.com/Alaska47/FTC-Android-Installation-Notes/blob/master/images/finish_code.png?raw=true"/>
</p>
13. Check out some sample code from https://github.com/Alaska47/ftc_app/tree/master/FtcRobotController/src/main/java/com/qualcomm/ftcrobotcontroller/opmodes. The files from the link are code for my team's robot last year. The relevant files are `AutoRed.java` (autonomous code) and `TeleOpRedBlue.java` (teleop code). 
<p align="center">
  <img src="https://github.com/Alaska47/FTC-Android-Installation-Notes/blob/master/images/github_code.png?raw=true"/>
</p>

If the following instructions aren't clear enough, refer to the notes that my teammates took on the process here https://github.com/Alaska47/FTC-Android-Installation-Notes/tree/master/extra_guides.
