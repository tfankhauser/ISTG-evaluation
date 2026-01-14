# ISTG Test Case Identifier
ISTG-WRLS-AUTHZ-001

# Name
Unauthorized Interaction

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
This test case evaluates wireless interfaces allow unauthorized interaction. It assesses if an unauthorized actor can perform operations that are intended for authorized contexts.

---

## Objectives
Assess if wireless interfaces are accessible without authorization.
Determine if access control of wireless interfaces is enforced.

---

## Execution Steps
Identify wireless interfaces by visual inspection or general scanning of common radio protocols.
Attempt interaction with discovered interfaces without any pairing process or authentication. 
Assess if operations are permitted and evaluate their impact.

---

## Security-relevant Findings
Identified wireless interfaces (BLE) were correctly enforcing pairing states. It was not possible to force a pairing process or directly interact with the devices.

---

## Expected Secure Behaviour
All wireless interfaces should implement authorization and authentication constraints. Direct interaction or other operations should not be possible and be rejected.

---

## Remediation Suggestions
Maintain current implementation of pairing constrictions. 
Review pairing process to ensure protection against impersonation.
