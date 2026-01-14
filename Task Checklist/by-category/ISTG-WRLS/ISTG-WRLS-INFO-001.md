# ISTG Test Case Identifier
ISTG-WRLS-INFO-001

# Name
Disclosure of Implementation Details

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
BHM-2025-E12, BHM-2025-E13

---

## Summary of Test Case
This test case assesses if wireless communication discloses information about implementation-specific details. This information could be used by an attacker to understand internal functionalities and plan further attacks.

---

## Objectives
Assess if implementation details are exposed through wireless channels.
Evaluate if disclosed information exceeds necessary data.
Determine the potential impact of this data.

---

## Execution Steps
Monitor wireless communication with Wireshark and the BLE adapter.
Analyse captured packages for implementation-specific details.
Assess the impact of discovered information.

---

## Security-relevant Findings
Captured BLE traffic exposed minimal implementation details, which could be used for further understanding of the functionalities, although the impact was deemed very low.

---

## Expected Secure Behaviour
Wireless interfaces and communication should only expose necessary data.

---

## Remediation Suggestions
Review information exposed by wireless communication.
Redact unnecessary information from the package flow.
