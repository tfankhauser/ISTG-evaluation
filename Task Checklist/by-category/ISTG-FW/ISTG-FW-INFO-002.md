# ISTG Test Case Identifier
ISTG-FW-INFO-002

# Name
Disclosure of Implementation Details

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
BHM-2025-E02, BHM-2025-E03

---

## Summary of Test Case
This test case evaluates if the firmware discloses implementation details, that could be weaponised by an attacker.

---

## Objectives
Identify implementation details inside of the firmware image.
Assess the risk of the exposed details.

---

## Execution Steps
Perform static analysis of the firmware with binwalk and strings.
Inspect outputs for meaningful information.
Identify implementation details or references to modules or mechanisms.

---

## Security-relevant Findings
The firmware image included implementation details such as module names, service identifiers and references to communication and update mechanisms. No sensitive information such as credentials were disclosed.

---

## Expected Secure Behaviour
Firmware images should have limited exposure of implementation details. Any identifiers should be abstracted or obfuscated to reduce the value to an attacker.

---

## Remediation Suggestions
Reduce exposure of internal identifiers where feasible.
Obfuscate necessary information in the firmware image.
