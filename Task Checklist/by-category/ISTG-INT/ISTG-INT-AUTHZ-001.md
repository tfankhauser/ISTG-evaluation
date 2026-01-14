# ISTG Test Case Identifier
ISTG-INT-AUTHZ-001

# Name
Unauthorized Interaction with Internal Interfaces

---

## Access Requirements
PA-4 / AA-1

## Component
Sensor Unit & Base Station — Internal Int.

---

## Execution Phase
Phase 2 & 8

## Tooling
UART Adapter, SWD Adapter, Multimeter, Logic Analyser, Serial Monitor

---

## Status
Executed

## Evidence ID
-

---

## Summary of Test Case
This test case evaluates if internal interfaces allow for unauthorized interaction providing access to internal functionalities or sensitive information.

---

## Objectives
Assess if internal interfaces can be interacted with without authentication.
Assess if authorisation methods can be bypassed.

---

## Execution Steps
Identify internal interfaces by inspecting traces or measuring continuity.
Assess possible connections and interactions with the corresponding adapters. 
If access control is present, identify possible bypasses.

---

## Security-relevant Findings
No interaction with internal interfaces was possible, as connections were integrated into the PCB directly and no non-destructive connection methods were identified.

---

## Expected Secure Behaviour
Only necessary internal interfaces should be enabled and protected by access control mechanisms. Non authorised interaction should not be possible.

---

## Remediation Suggestions
Ensure the use of lock mechanisms for internal interfaces.
Ensure that communication channels between PCB components are not easily accessible.
