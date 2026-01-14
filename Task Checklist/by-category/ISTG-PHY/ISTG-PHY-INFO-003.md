# ISTG Test Case Identifier
ISTG-PHY-INFO-003

# Name
Disclosure of User Data

---

## Access Requirements
PA-4 / AA-1

## Component
Sensor Unit & Base Station — Physical Int.

---

## Execution Phase
Phase 2

## Tooling
UART Adapter, SWD Adapter, Multimeter, Logic Analyser, Serial Monitor

---

## Status
Executed

## Evidence ID
-

---

## Summary of Test Case
This test case evaluates if physical interfaces disclose user data at runtime.

---

## Objectives
Determine if user data can be accessed without authorization.

---

## Execution Steps
Visual inspection of the PCB to identify exposed connectors or pins.
Identify protocols of connectors via traces or continuity testing.
Connect corresponding adapter or logic analyser and monitor output via serial monitor.
Monitor for meaningful disclosed data.

---

## Security-relevant Findings
Physical interfaces did not disclose any user data.

---

## Expected Secure Behaviour
User data should not be accessible through physical interfaces.

---

## Remediation Suggestions
Collected or processed user data should only be accessible by authorized users or processes.
