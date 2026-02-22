# Bug Report: Job Description Expansion Failure on Orientation Change

**Project:** LinkedIn Android Application  
**Severity:** Medium / UI  
**Environment:** Samsung M14 (Android 15), Resolution 1080 x 2408  

---

## Summary
The "See more" button in the job description section becomes unresponsive if the device orientation is changed immediately after navigating to a job offer. The issue prevents the user from reading the full job description.

## Steps to Reproduce
1. Launch the LinkedIn application.
2. Navigate to the **Jobs** tab.
3. Tap on any job posting to open the **Job Details** view.
4. Change the device orientation (Portrait -> Landscape) or (Landscape -> Portrait).
5. Attempt to tap the **"See more"** button to expand the text.
6. Rotate the device back and try to tap the button again.

## Expected Result
The job description should expand and collapse correctly regardless of any screen orientation changes.

## Actual Result
The "See more" button is completely unresponsive. The UI does not react to touch events on the expansion trigger.

---

## Technical Analysis (Logcat Insights)
[cite_start]Based on the logs provided, the issue relates to **Configuration Change** handling:

* **Layout Constraints Errors:** Multiple errors from `com.linkedin.android` indicate deprecated attributes.
* **Observation:** During `onConfigurationChanged`, layout errors coincide with the button becoming unresponsive. This suggests a failure in the View binding process.

---

## Attachments
* **Logs:** [View Logcat File](./attachments/Bug01-LinkedIn-logs.txt)
* **Screen Record:** [![Watch the video](https://img.youtube.com/vi/I4G1gm-qPLc/0.jpg)](https://youtube.com/shorts/I4G1gm-qPLc)

---

## Possible Workaround
Restarting the Activity by navigating back and re-entering the job offer restores functionality.
