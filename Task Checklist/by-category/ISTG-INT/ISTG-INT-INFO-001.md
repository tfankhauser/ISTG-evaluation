# ISTG Test Case Identifier
ISTG-INT-INFO-001

# Name
Disclosure of Implementation Details

---

## Access Requirements
PA-4 / AA-1

## Component
Base Station — Internal Int.

---

## Execution Phase
Phase 2 & 8

## Tooling
UART Adapter, Serial Monitor

---

## Status
Executed

## Evidence ID
BHM-2025-E01

---

## Summary of Test Case
This test case assesses if internal interfaces disclose any information specific to implementation details. This information could be used by an attacker to further understand the device’s architecture or configuration.

---

## Objectives
Identify if internal interfaces expose implementation details at any point.
Evaluate if exposed information can be weaponized.

---

## Execution Steps
Connect to identified UART pins with the UART adapter.
Start monitoring with the serial monitor and power up the device to capture boot messages. 
Analyse discovered output from boot and runtime for any useful information.

---

## Security-relevant Findings
The UART interface of the LTE module on the base station disclosed minimal implementation details, such as the UART baud rate used for internal communication and references to “FOTA” (firmware-over-the-air) mechanisms. No sensitive information was exposed.

---

## Expected Secure Behaviour
Internal debugging output should be limited in production devices and should not expose any configuration data.

---

## Remediation Suggestions
Reduce information output of exposed UART interface for production devices.
If possible, disable debug UART interface completely when shipping the device.
