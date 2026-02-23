Regression Checklist: Bingo: Love in Montana

Phase: Gold Master 

Device Focus: Samsung M14 (Android 15), 20:9 Aspect Ratio 

1. Functional Gameplay Logic

Victory Flow: Verify that completing a Bingo card triggers the "Victory" screen and grants correct XP/Coins.

Defeat Flow: Verify that losing a game triggers the "Lose" screen, offers a "Continue" option, and grants correct XP/Coins.

Inventory Management: Confirm that all boosters activate correctly and are deducted from the inventory upon use.

Story Progression: Verify that "Montana Story" unlock mechanics function correctly upon reaching specific level milestones.

2. Technical & Mobile-Specific Testing

Call Interruption: Receive an incoming call during an active match; verify the game pauses and resumes without data loss.

Network Resilience (Offline Mode): Disconnect the internet during gameplay; verify the game transitions to offline mode gracefully.

Session Recovery: Disconnect during a match and reconnect; verify the game session continues from the last saved state.

Backgrounding Performance: Minimize the app for 2 minutes (Background state); verify the session is maintained upon returning.

Hardware Optimization: Verify the app does not trigger "High Battery Usage" or "Overheating" warnings after 30 minutes of continuous play.

3. UI, UX & Localization

Dynamic Scaling: Verify all pop-ups and UI elements are centered and not cut off on 20:9 aspect ratio screens.

Localization Integrity: Scan all screens to ensure no raw "localization keys" are visible to the user.

Fallback Language: Verify that if the device language is not supported, the game automatically defaults to English.
