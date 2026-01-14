# ISTG Test Case Identifier
ISTG-WRLS-INFO-003

# Name
Disclosure of User Data

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
BHM-2025-E14

---

## Summary of Test Case
This test case evaluates if wireless communication exposes user-related data outside of authorized contexts. This data could include account information, other identifiable data, or sensor values.

---

## Objectives
Assess if wireless channels expose data that can be correlated or interpreted as user data.
Evaluate if disclosed data can be linked to specific users or user actions.

---

## Execution Steps
Monitor wireless traffic with Wireshark and the BLE adapter.
Analyse captured packages, focusing on data exchange packets.
Evaluate if data can be interpreted meaningfully and correlates to user-related information.

---

## Security-relevant Findings
It was discovered that the data exchange between the two devices is unencrypted and interpretation of the content was attempted but not verified. If correct, sensor measurements including body temperature and movement could be exposed without any restrictions and could be passively sniffed.

---

## Expected Secure Behaviour
User-related data should not be exposed to unauthorized and unauthenticated actors. Appropriate measures should be in place to encrypt information and access control should limit exposure of data.

---

## Remediation Suggestions
Implement BLE encryption between sensor unit and base station using current best practices. 
If encryption is not possible, data should be obfuscated to obstruct interpretation.
