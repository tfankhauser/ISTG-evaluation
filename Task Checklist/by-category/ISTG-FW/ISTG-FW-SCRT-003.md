# ISTG Test Case Identifier
ISTG-FW-SCRT-003

# Name
Usage of Hardcoded Credentials

---

## Access Requirements
PA-1-4 / AA-1-4

## Component
Firmware – Static Image

---

## Execution Phase
Phase 4

## Tooling
Binwalk, strings, hex editor, Ghidra

---

## Status
Executed

## Evidence ID
-

---

## Summary of Test Case
This test case evaluates if the firmware source code includes plaintext credentials, that could be extracted and used for unauthorized access.

---

## Objectives
Identify hardcoded usernames, passwords, or other credentials in the firmware.
Evaluate if discovered credentials can be used maliciously.

---

## Execution Steps
Extract strings or decompile firmware image with Ghidra.
Analyse if the source code includes hardcoded credentials. 
Assess if identified credentials are valid and can be used to gain unauthorized access.

---

## Security-relevant Findings
No hardcoded credentials were discovered during static analysis and decompilation.

---

## Expected Secure Behaviour
Firmware images should not include plaintext secrets in the source code which could be extracted through static analysis of the image. Necessary credentials should be provisioned through protected channels during runtime.

---

## Remediation Suggestions
Continue the communication of secrets via secure channels during runtime. 
Ensure periodical checks for unintended artefacts in the firmware.
