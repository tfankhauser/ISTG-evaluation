# ISTG Test Case Identifier
ISTG-FW[UPDT]-LOGIC-001

# Name
Rollback Protection Insufficient

---

## Access Requirements
PA-1-4 / AA-1-4

## Component
Base Station - Firmware Update Mechanism

---

## Execution Phase
Phase 4

## Tooling
Strings

---

## Status
Executed

## Evidence ID
BHM-2025-E06

---

## Summary of Test Case
This test case assesses if appropriate firmware update rollback mechanisms are in place. These ensure that the device’s functionality does not get impacted by a failed firmware update.

---

## Objectives
Identify firmware update logic.
Assess if rollback mechanisms are working correctly by triggering a failed update.

---

## Execution Steps
Analyse firmware for update mechanism rollback references. 
If possible, analyse behaviour after power outage during update process.

---

## Security-relevant Findings
Firmware strings indicate that rollback mechanisms and error handling are in place and lead to a reset of the device. No active attacks could be attempted due to legal limitations.

---

## Expected Secure Behaviour
Appropriate rollback mechanisms should be in place, that reject and prevent failed installation processes.

---

## Remediation Suggestions
Ensure that rollback mechanisms are properly enforced.
