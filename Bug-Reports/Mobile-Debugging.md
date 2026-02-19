# Technical Skills: Mobile Debugging (Android)

In my role as a Junior QA Engineer at **Galaxy4Games** and during various testing activities, I use a technical approach to identify the root causes of defects on the Android platform.

### Tools & Environment
* **Android Studio:** Used for managing virtual devices (Emulators) and analyzing real-time system output via Logcat.
* **Real Devices:** Testing on various hardware to ensure stability across different Android versions.
* **ADB (Android Debug Bridge):** My primary command-line tool for device interaction and debugging.

### Essential ADB Commands I Use
To provide developers with high-quality data, I utilize the following commands:

* `adb logcat *:E` – To filter and capture system errors and application crashes.
* `adb install -r [path_to_apk]` – For efficient build deployment and re-installation during regression testing.
* `adb shell dumpsys meminfo [package_name]` – To monitor memory usage and identify potential leaks in game scenes.
* `adb bugreport` – To generate comprehensive diagnostic files for complex, non-reproducible issues.

### Practical Application (Galaxy4Games Experience)
While testing **"Match 3 Stars: PVP Champions"**, I encountered a freeze during the level loading screen. By using **ADB Logcat**, I successfully captured a `NullPointerException`. 

This allowed me to:
1. Provide a specific stack trace to the development team.
2. Reduce the debugging time for the engineers.
3. Verify the fix efficiently in the next build.

---
