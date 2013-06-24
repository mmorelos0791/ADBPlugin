# ADB Plugin

ADB Plugin is a Chrome Extension that runs ADB daemon and enables remote debugging for mobile. With it, you do not need to download the Android SDK or run ADB yourself from the command line. This extension is experimental and currently only works on Mac.

# How to run (Windows & Mac OS)
- For Windows, make sure you have ADB communication [https://dl.google.com/android/repository/usb_driver_r07-windows.zip](driver) installed.
- Visit **[github.com/repenaxa/ADBPlugin/raw/master/out/npADBPlugin-crx.crx](https://github.com/repenaxa/ADBPlugin/raw/master/out/npADBPlugin-crx.crx)** and download extension.
- Go to `about:extensions` and drop that file there.
- Click little Android icon next to address bar.

# How to build (Mac)
- Get FireBreath at [firebreath.org/display/documentation/Download](http://www.firebreath.org/display/documentation/Download)
- Place ADBPlugin under `firebreath/projects/ADBPlugin`
- Run `./prepmac.sh && xcodebuild ARCHS=i386 ONLY_ACTIVE_ARCH=NO -configuration Release -project build/FireBreath.xcodeproj`
- The build will be available at `build/projects/ADBPlugin/gen/npADBPlugin-crx.crx`.
- There is a pre-built version available at [github.com/repenaxa/ADBPlugin/raw/master/out/npADBPlugin-crx.crx](https://github.com/repenaxa/ADBPlugin/raw/master/out/npADBPlugin-crx.crx) for convenience. 
