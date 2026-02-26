# Test Plan: Booster Mechanics (Bingo: Love in Montana)

**Project:** Bingo: Love in Montana  
**Focus:** Inventory Logic and Gameplay Synchronization  
**Version:** 1.2

---

## 1. Scope of Testing
* **Core Functionality:** Activation logic, VFX/SFX, and in-game effects.
* **Inventory Economy:** Reward acquisition and deduction logic.
* **UI/UX:** Button hitbox accuracy and counter readability on various aspect ratios.
* **Negative Scenarios:** Activation with zero balance and Race Conditions via rapid tapping.

## 2. Testing Strategy
### 2.1. Testing Types
* **Positive Functional Testing:** Verifying activation according to GDD.
* **Boundary and Negative Testing:** Using the last available item and activation at match end.
* **Interruption Testing:** Incoming calls or switching network types during activation.
* **Low-end Device Performance:** Checking for FPS drops during simultaneous VFX triggers.

### 2.2. Tools
* **ADB Logcat:** Monitoring system errors and server responses.
* **Postman:** Backend API stability and response time verification.

## 3. Entry and Exit Criteria
* **Entry Criteria:** Stable build deployed and updated documentation available.
* **Suspension Criteria:** Testing stops if booster usage leads to a Crash or ANR.
* **Exit Criteria:** 100% of test cases executed with all High and Critical bugs resolved.

## 4. Test Environment
* **Hardware:** Physical Android Devices and Emulators.
* **Aspect Ratios:** Focus on 20:9 and 16:9 displays.

---

## Test Cases

| ID | Title | Scenario | Expected Result |
| :--- | :--- | :--- | :--- |
| **BL-B01** | **Race Condition** | Rapidly tap the booster button multiple times. | Booster activates once; only 1 unit is deducted. |
| **BL-B02** | **Boundary Balance** | Use the final available booster. | Balance becomes 0; icon redirects to Shop. |
| **BL-B03** | **Network Sync** | Disable internet during activation animation. | Reconnecting message appears; balance is synced after restoration. |
| **BL-B04** | **UI Responsiveness** | Tap booster button on the target device. | Button responds accurately within its boundaries. |
