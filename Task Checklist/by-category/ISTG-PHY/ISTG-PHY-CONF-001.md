# ISTG Test Case Identifier
ISTG-PHY-CONF-001

# Name
Usage of Outdated Software (Physical)

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
This test case identifies outdated software components through physical interaction with the device.

---

## Objectives
Identify software versions through physical interfaces. 
Determine if disclosed data contains software information.

---

## Execution Steps
Visual inspection of the PCB to identify exposed connectors or pins.
Identify protocols of connectors via traces or continuity testing.
Connect corresponding adapter or logic analyser and monitor output via serial monitor.
Monitor for software version information.

---

## Security-relevant Findings
No indicators of outdated software were discovered through physical interfaces.

---

## Expected Secure Behaviour
Production devices should not output any detailed software version information through physical interfaces. Accessible output should be limited to necessary information.

---

## Remediation Suggestions
Ensure that physical interface output does not disclose any software version information.
