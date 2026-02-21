Bug Report: Special Offer Window Scaling Issue
Project: Bingo: Love in Montana Severity: Medium / UI Environment: Samsung M14 (Android 15), Resolution: 1080 x 2408 (20:9 Aspect Ratio)

Summary
The "Super Offers" popup window does not scale correctly to the device screen format, causing parts of the window to be cut off.

Steps to Reproduce
Launch the application.
Wait for the main menu to load.
Click on the "Super Offers" icon/banner on the left side of the screen.
Expected Result
The "Super Offers" window should be fully visible, properly scaled, and centered within the display area without losing any UI elements.

Actual Result
The window is rendered too large for the current display format. As a result, the edges of the window (including the 'Close' button or offer details) are clipped outside the screen boundaries.

Professional Insight
This issue is likely related to the high aspect ratio of the Samsung M14. The UI layout needs an anchor adjustment or a responsive scaling script to handle displays longer than 16:9 or 18:9.

Attachments:
image
