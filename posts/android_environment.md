[Main](/index.md)

## Installing environment for android-development


1. Install Java ([JRE](http://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html) or [JDK](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html))


2. Install [Android Studio](http://developer.android.com/sdk/index.html)


3. Install needed packages from Android SDK Manager including Google USB Driver 

`Tools -> Android -> SDK Manager`

Default path for Google USB Driver - `C:\Users\Olexandr\AppData\Local\Android\sdk\extras\google\usb_driver`


4. Install [Genymotion](https://www.genymotion.com/#!/download) emulator
Install Genymotion plugin for Android Studio

    4.1. In Android Studio, go to `File > Settings`.

    4.2. Select Plugins and click Browse Repositories.

    4.3. Right-click on Genymotion and click Download and install.


5. Install USB Drivers for your device with help of next pages [1](http://developer.android.com/tools/device.html), [2](http://developer.android.com/sdk/win-usb.html), [3](http://developer.android.com/tools/extras/oem-usb.html).
If you can't find needed information for your devices in these pages, you can install driver manually

    5.1. Mount your device as usb-drive

    5.2. Open Device Manager and find your device in list

    5.3. Select `Options -> Drivers` and press Update driver...

    5.4. Select second variant - Find drivers on my computer

    5.5. Select second variant - Select driver from list of device's drivers on computer

    5.6. Select Install from drive and specify path for Google USB Driver

    5.7. In appeared list select Android ADB Interface and press Next.


*P.S.*

1. You can change device type which will be run your application

`Run -> Edit Configurations -> Target Device`


2. For running application on device you must allow in settings of device follows items:

- installing applications from unknown sources;

- debugging on USB.


