# ISTG Test Case Identifier
ISTG-FW[UPDT]-CRYPT-003

# Name
Insecure Transmission of Firmware Updates

---

## Access Requirements
PA-1-4 / AA-1-4

## Component
Base Station - Firmware Update Mechanism

---

## Execution Phase
Phase 4

## Tooling
Wireshark, Burp Suite

---

## Status
Executed

## Evidence ID
BHM-2025-E05

---

## Summary of Test Case
This test case assesses if firmware updates are only transmitted through secure channels.

---

## Objectives
Identify the transport channel for firmware updates.
Assess if the discovered channel uses appropriate encryption.

---

## Execution Steps
Analyse firmware for references to update transmission protocols or endpoints.
Assess observable network traffic.
Evaluate if observed traffic is encrypted properly or can be intercepted.

---

## Security-relevant Findings
No firmware update traffic could be observed on permitted protocols. This indicates the firmware updates are transmitted over LTE, which is deemed secure, in combination with discovered references for encryption of the LTE channel.

---

## Expected Secure Behaviour
Firmware updates should only be transmitted through encrypted and authenticated channels. This is done to prevent interception or tampering during transmission.

---

## Remediation Suggestions
Maintain current transport mechanisms.
Ensure that no insecure fallback mechanisms are implemented that could be exploited.
