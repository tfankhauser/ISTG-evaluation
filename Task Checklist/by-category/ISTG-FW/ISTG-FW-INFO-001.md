# ISTG Test Case Identifier
ISTG-FW-INFO-001

# Name
Disclosure of Binaries or Source Code

---

## Access Requirements
PA-1-4 / AA-1-4

## Component
Firmware – Static Image

---

## Execution Phase
Phase 4

## Tooling
Binwalk, strings, file, hex editor

---

## Status
Executed

## Evidence ID
-

---

## Summary of Test Case
This test case assesses if the attacker can gain access to firmware binaries or source code.

---

## Objectives
Identify if firmware image includes binaries.
Evaluate if firmware includes source code or debugging symbols.

---

## Execution Steps
Obtain the firmware image.
Use binwalk to identify file structures and artefacts.
Use strings to extract any meaningful strings in the firmware image. 
Analyse outputs of binwalk and strings for source code or extractable binaries.

---

## Security-relevant Findings
No source code or binaries were found in the firmware image. All extractable data consisted of unusable compiled binaries and no source-level artefacts.

---

## Expected Secure Behaviour
Production firmware on the device should not contain any source code or other plain artefacts. Compiled binaries should be packaged and stripped to protect against reverse-engineering.

---

## Remediation Suggestions
Continue the current practice of firmware distribution.
