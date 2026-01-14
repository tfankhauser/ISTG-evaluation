# ISTG Test Case Identifier
ISTG-WRLS-SCRT-001

# Name
Access to Sensitive Data

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
This test case evaluates if the wireless interfaces disclose sensitive data such as credentials, tokens, or cryptographic keys.

---

## Objectives
Identify if wireless interfaces transmit security-relevant information.
Evaluate if it is possible to extract secrets from wireless traffic.

---

## Execution Steps
Monitor wireless traffic with Wireshark and the BLE adapter, including the pairing process and data exchange.
Analyse packet data for sensitive data such as tokens or credentials.
Assess if pairing process is implemented insecurely, e.g. through repeated usage of the same secret.

---

## Security-relevant Findings
The analysed wireless traffic did not show any sensitive information, credentials, tokens, or keys. No information was discovered, that could lead to a compromise of authentication or encryption.

---

## Expected Secure Behaviour
Security-relevant data should not be exposed through wireless interfaces without proper protection mechanisms in place, such as encryption.

---

## Remediation Suggestions
Maintain current implementation of pairing process.
