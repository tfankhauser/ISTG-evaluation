# ISTG Test Case Identifier
ISTG-WRLS-CRYPT-001

# Name
Insecure Cryptographic Algorithms

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
BHM-2025-E15

---

## Summary of Test Case
This test case assesses if wireless interfaces and communication use appropriate cryptographic methods to maintain the confidentiality and integrity of the transmitted data.

---

## Objectives
Identify implemented cryptographic mechanisms of wireless communication.
Compare identified encryption methods against current cryptographic best practices.

---

## Execution Steps
Capture wireless traffic with Wireshark and BLE adapter.
Analyse captured packets for indicators of encryption.
Identify encryption methods by comparing data structures.

---

## Security-relevant Findings
During analysis it was found, that the BLE communication of the devices was not employing any encryption method. The transmitted plaintext data was captured passively, and interpretation attempts were made but could not be verified.

---

## Expected Secure Behaviour
Wireless interfaces should implement strong and modern cryptographic mechanisms for data exchange.

---

## Remediation Suggestions
Adjust the data transmission implementation to apply modern and secure encryption methods. 
Review best practices for wireless data transmission.
If encryption is not technically feasible, data should be obfuscated to prevent passive sniffing and interpretation.
