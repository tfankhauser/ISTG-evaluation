# ISTG Test Case Identifier
ISTG-FW-SCRT-001

# Name
Discovery of Secrets in Public Storage

---

## Access Requirements
PA-1-4 / AA-1-4

## Component
Firmware – Static Image

---

## Execution Phase
Phase 4

## Tooling
Binwalk, strings, hex editor

---

## Status
Executed

## Evidence ID
-

---

## Summary of Test Case
This test case evaluates if firmware contains hardcoded credentials or secrets stored in publicly accessible locations.

---

## Objectives
Identify credentials, tokens, or keys embedded in the files of the image. 
Assess if exposed secrets could be weaponised for unauthorized access.

---

## Execution Steps
Extract all possible information from the firmware image.
Analyse extracted strings or binaries for embedded secrets.
Assess if discovered secrets could be used maliciously.

---

## Security-relevant Findings
The firmware image did not include any credentials or keys. Extracted data did not include sensitive credentials in plaintext or identifiable encryption.

---

## Expected Secure Behaviour
Firmware images should not include plaintext secrets in files which could be extracted through static analysis of the image. Necessary credentials should be provisioned through protected channels during runtime.

---

## Remediation Suggestions
Continue the communication of secrets via secure channels during runtime. 
Ensure periodical checks for unintended artefacts in the firmware.
