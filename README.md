<img width="192" height="192" alt="bhp_launcher" src="https://github.com/user-attachments/assets/de9b0609-d223-4f91-80c1-81722feea3c9" />





Battery health and cycle count reader for compatible Samsung Galaxy devices



Battery Health Plus is a simple app for Samsung Galaxy devices that can display the battery's **health percentage** and **cycle count** without root access or ADB 

The app reads battery information from Samsung's built-in SysDump logs and presents the useful values in a clean interface.

## Features

* 🔋 Battery health percentage
* 🔄 Battery cycle count
* 📱 Designed for Samsung Galaxy devices with One UI inspired theme
* 🔓 No root required
* 💻 No ADB required for normal use
* 📜 Battery check history
* 🌙 Light and dark theme support
* 🔒 Battery information is processed locally on your device

## How It Works

Samsung stores battery statistics inside its diagnostic dumpstate logs.

Battery Health Plus searches these logs for Samsung battery values including:

* `mSavedBatteryAsoc` — battery health percentage
* `mSavedBatteryUsage` — battery usage value used to calculate cycle count

Cycle count is calculated as:

```text
mSavedBatteryUsage / 100
```

For example:

```text
mSavedBatteryUsage : 25340
```

is displayed as approximately:

```text
253.4 cycles
```

## How to Use

1. Download and install the APK below.
2. Open Battery Plus and select the log folder, if there's no folder create one named with "log"
3. Tap Start, then press # in the Phone app.
4. Scroll down and tap “Run dumpstate & copy to sdcard”, then OK.
5. Once report generation finishes, return to Battery Plus and tap Check.



   Note:
   
          1)to check latest readings repeat above steps again

          2)after checking battery health you can delete generated files in log folder

## Download

Download the latest APK from the **Releases** section of this repository.

## Compatibility

Battery Health Plus is intended primarily for **Samsung Galaxy devices** that provide the required battery information through Samsung SysDump.

## Important

Battery health values are reported by Samsung's battery management system

Battery Health Plus is an independent project and is **not affiliated with, endorsed by, or sponsored by Samsung Electronics**.

## Issues

If Battery Health Plus does not detect your battery information, open an issue and include:

* Galaxy model
* One UI version
