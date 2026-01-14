# ISTG Test Case Identifier
ISTG-PROC-SIDEC-001

# Name
Insufficient Side-Channel Protection

---

## Access Requirements
PA-4 / AA-1-4

## Component
Sensor unit & base station – MCU

---

## Execution Phase
Phase 5 & 8

## Tooling
SWD adapter, STM32CubeProgrammer, oscilloscope

---

## Status
Executed

## Evidence ID
-

---

## Summary of Test Case
This test evaluates if the MCU shows observable characteristics for side-channel attacks, that could possibly leak sensitive information. This could include timing patterns or power variations.

---

## Objectives
Identify observable characteristics of MCU.
Assess potential correlations between behaviour and characteristics.

---

## Execution Steps
Observe boot and runtime power consumption and behaviour.
Correlate characteristics with information found in firmware.
Evaluate if patterns exist and could be interpreted.

---

## Security-relevant Findings
Both MCUs did not present any characteristics for side-channel attacks. Observed behaviour and patterns was consistent and could not be correlated to specific operations.

---

## Expected Secure Behaviour
MCUs should not produce observable characteristics while processing specific operations, such as security-relevant instructions.

---

## Remediation Suggestions
Ensure that specific side-channel protection techniques are implemented.
Maintain implementation practices limiting observable characteristics.
