# ISTG Test Case Identifier
ISTG-FW[UPDT]-AUTHZ-001

# Name
Unauthorized Update of Firmware

---

## Access Requirements
PA-1-4 / AA-1-3

## Component
Base Station - Firmware Update Mechanism

---

## Execution Phase
Phase 4

## Tooling
Burp Suite, Wireshark, UART adapter, Serial Monitor

---

## Status
Executed

## Evidence ID
-

---

## Summary of Test Case
This test case assesses if the firmware update mechanism can be executed or manipulated without required authorization.

---

## Objectives
Identify how firmware updates are conducted and communicated. 
Assess if unauthorized triggering of the update mechanism is possible.

---

## Execution Steps
Analyse the firmware for references to update mechanisms. 
Analyse network traffic for references to update endpoints or mechanisms. 
Evaluate if this information can be used to trigger an unauthorized firmware update.

---

## Security-relevant Findings
It was not possible to identify a firmware update mechanism through firmware analysis. Network traffic between the base station and the cloud could not be analysed due to legal regulation according LTE traffic.

---

## Expected Secure Behaviour
Firmware updates should only be triggered through authorized and secure channels. Any attempts to update the firmware outside of the controlled mechanisms should be rejected by the device.

---

## Remediation Suggestions
Ensure that update triggers cannot be started by an attacker. 
Continue the implementation of strict and secure update mechanisms.
