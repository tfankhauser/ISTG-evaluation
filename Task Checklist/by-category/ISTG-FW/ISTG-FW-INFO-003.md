# ISTG Test Case Identifier
ISTG-FW-INFO-003

# Name
Disclosure of Ecosystem Details

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
BHM-2025-E02

---

## Summary of Test Case
This test case evaluates if the firmware image discloses details about the device’s ecosystem, such as backend services, API endpoints, or dependencies.

---

## Objectives
Identify references to backend services, API endpoints or other third-party dependencies.
Assess the value of discovered references and if they can be weaponised.

---

## Execution Steps
Extract strings or other information from firmware.
Identify references to API endpoints or other backend services.
Assess the value of discovered information.

---

## Security-relevant Findings
The firmware image included strings representing API endpoints and communication services such as MQTT references. No credentials or other sensitive information was discovered. The discovered information allows further understanding and mapping of the ecosystem but does not enable direct access.

---

## Expected Secure Behaviour
Firmware images should not disclose unnecessary details. Where possible, references to endpoints or services should be abstracted or obfuscated to reduce the value to an attacker.

---

## Remediation Suggestions
Minimize plaintext / hardcoded identifiers and references where possible. 
Avoid embedding descriptive strings in the firmware (obfuscation).
