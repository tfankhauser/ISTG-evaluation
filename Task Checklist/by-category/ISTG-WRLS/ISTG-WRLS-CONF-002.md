# ISTG Test Case Identifier
ISTG-WRLS-CONF-002

# Name
Identified Unnecessary Software

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
This test case assesses if the devices expose any unnecessary wireless services.

---

## Objectives
Enumerate all exposed wireless services.
Evaluate if these services include any characteristics that are not in use.
Determine the impact on the attack surface through their exposure.

---

## Execution Steps
Use Wireshark and the BLE adapter to passively monitor wireless traffic.
Identify all available services and characteristics.
Assess their operational relevance through comparison to expected behaviour.

---

## Security-relevant Findings
Both devices did not expose any unnecessary wireless services through the analysed wireless channels. All exposed data was required for correct operation and communication.

---

## Expected Secure Behaviour
Wireless interfaces should only expose services that are required for intended functionality.

---

## Remediation Suggestions
Maintain minimized exposure of wireless services.
