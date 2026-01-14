# ISTG Test Case Identifier
ISTG-DES-CRYPT-001

# Name
Insecure Cryptographic Algorithms

---

## Access Requirements
PA-1 / AA-1-4

## Component
Data Exchange Services – Cloud Services

---

## Execution Phase
Phase 6 & 7

## Tooling
Android Studio, Burp Suite Proxy

---

## Status
Executed

## Evidence ID
-

---

## Summary of Test Case
This test case evaluates if data exchange services are using weak or insecure cryptographic algorithms during communication. This could lead to an attacker cracking encryption.

---

## Objectives
Identify implemented cryptographic algorithms.
Assess if they are still secure and modern.

---

## Execution Steps
Intercept network traffic to analyse TLS parameter, protocol versions and possible implemented ciphers.
Assess if the discovered configurations are still considered secure or deprecated.

---

## Security-relevant Findings
No weak or deprecated encryption mechanisms were discovered in the DES. Identified configurations were consistent with secure and modern best practices.

---

## Expected Secure Behaviour
All communication channels of the DES should employ strong and modern cryptographic mechanisms to ensure confidentiality and integrity. Parameter and configurations should be chosen according to current best practices.

---

## Remediation Suggestions
Maintain current configurations and encryption methods.
Regularly review best practices for necessary changes.
