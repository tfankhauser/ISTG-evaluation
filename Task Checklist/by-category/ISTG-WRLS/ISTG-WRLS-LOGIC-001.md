# ISTG Test Case Identifier
ISTG-WRLS-LOGIC-001

# Name
Circumvention of intended Business Logic

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
This test case assesses if wireless interfaces enforce constraints protecting the intended business logic, or if misuse leads to unintended behaviour.

---

## Objectives
Analyse intended logic workflows.
Evaluate if replayed, altered, or invalid requests lead to unintended device behaviour.

---

## Execution Steps
Capture normal wireless traffic between the devices with Wireshark and the BLE adapter.
Identify attack vectors for possible value modification or indicators of intended packet order.
Replay altered or re-ordered packets and observe device behaviour.

---

## Security-relevant Findings
The tester could not identify any flaws in the business logic of the wireless data exchange. Any attempts to send modified or altered packets got rejected by the receiving device.

---

## Expected Secure Behaviour
Constraints should be implemented, that reject any unexpected or invalid interactions.

---

## Remediation Suggestions
Review LTE transmission implementation for possible business logic flaws (out of scope).
Maintain current logic handling implementation.
