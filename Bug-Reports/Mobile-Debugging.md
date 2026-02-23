# Mobile Debugging Skills (Android)

Technical expertise in identifying root causes of defects using Android-specific tools, developed during testing cycles at **Galaxy4Games**.

## Tools & Stack
* **ADB:** Core tool for device interaction and log extraction.
* **Android Studio:** Used for Logcat analysis and managing Virtual Devices.
* **Real Devices:** Testing stability across various hardware and OS versions.

## Essential ADB Commands
* `adb logcat *:E` — Extracting system errors and crashes.
* `adb install -r [path]` — Quick build deployment during regression testing.
* `adb shell dumpsys meminfo` — Monitoring memory consumption to detect leaks.
* `adb bugreport` — Generating full diagnostics for non-reproducible issues.

## Practical Case: Logcat Analysis
During the development of **"Match 3 Stars: PVP Champions"**, I used Logcat to debug a loading screen freeze.
* **Action:** Captured a `NullPointerException` stack trace.
* **Result:** Provided logs to developers, significantly reducing time-to-fix and ensuring stability for the next build.
