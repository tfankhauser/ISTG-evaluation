# ISTG Test Case Identifier
ISTG-PROC-AUTHZ-001

# Name
Unauthorized Access to the Processing Unit

---

## Access Requirements
PA-4 / AA-1

## Component
Sensor Unit & Base Station – MCU

---

## Execution Phase
Phase 5 & 8

## Tooling
SWD adapter, UART adapter, serial monitor, STM32CubeProgrammer

---

## Status
Executed

## Evidence ID
-

---

## Summary of Test Case
This test case is used to evaluate if unauthorized access to the processing unit is possible. This could include debugging, memory access or execution control.

---

## Objectives
Identify exposed or accessible MCU interfaces.
Assess access control of identified interfaces.

---

## Execution Steps
Identify MCU through visual inspection.
Locate potential interfaces by analysing traces and referencing corresponding data sheets.
Connect the corresponding adapter and attempt interactive connections.

---

## Security-relevant Findings
SWD debugging interfaces were discovered on both, the base station and the sensor unit. These could not be interacted with due to access control implemented on chip level.

---

## Expected Secure Behaviour
Production devices should enforce strict access control on any interactive interfaces. Unauthorized interaction should not lead to readable memory or execution control.

---

## Remediation Suggestions
Periodically verify access control to prevent accidental unlocking through firmware settings.
