# Bug Report: Data Loss During Analytical Model Update (Revit to Robot)

**Project:** Autodesk Integration (Revit & Robot)
**Severity:** Medium / Technical
**Environment:** Windows PC

---

## Summary
When updating an existing analytical model in Robot via the Revit integration link, some objects are lost during the transfer process, even though the model remains unchanged in Revit.

## Steps to Reproduce
1. Launch Revit and open a project with an analytical model.
2. Transfer the model to Robot Structural Analysis for the first time.
3. Perform a second transfer (Update) from Revit to Robot without making any changes to the model.

## Expected Result
The model is updated/synchronized without any data loss.

## Actual Result
The system reports that several objects were not transferred, resulting in an incomplete model in Robot.

---

## Attachments
<img width="680" height="466" alt="image" src="https://github.com/user-attachments/assets/5f25a555-2a8e-4ac8-a151-8aba741fcc6e" />
