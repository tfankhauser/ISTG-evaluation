# ISTG Test Case Identifier
ISTG-WRLS-INFO-002

# Name
Disclosure of Ecosystem Details

---

## Access Requirements
PA-2-4 / AA-1-4

## Component
Sensor unit & base station – BLE interface

---

## Execution Phase
Phase 6

## Tooling
nRF52840 Dongle, Wireshark

---

## Status
Executed

## Evidence ID
-

---

## Summary of Test Case
This test case evaluates if the wireless interfaces disclose any information that could lead to a broader understanding of the devices’ ecosystem. This could include backend services or device roles.

---

## Objectives
Assess if wireless communication discloses ecosystem-related information.
Evaluate if discovered information exceeds functionally necessary data.

---

## Execution Steps
Monitor wireless traffic with Wireshark and the BLE adapter.
Analyse captured packages for ecosystem-related information, such as backend descriptors or endpoints.
Evaluate the potential impact of discovered data and if it is technically required.

---

## Security-relevant Findings
No ecosystem-related information was found in the captured BLE packages.

---

## Expected Secure Behaviour
Wireless interfaces should not disclose any unnecessary information about the surrounding ecosystem. Only details that are required for normal operation should be transmitted.

---

## Remediation Suggestions
Review BLE communication for unnecessary references.
Maintain restrictive information transmission.
