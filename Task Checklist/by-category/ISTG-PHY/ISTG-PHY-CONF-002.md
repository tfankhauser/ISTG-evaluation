# ISTG Test Case Identifier
ISTG-PHY-CONF-002

# Name
Presence of Unnecessary Functionalities

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
This test case determines if unnecessary functionalities are present and accessible via physical functionalities, that are not required and could increase the attack surface.

---

## Objectives
Identify physical interfaces or components that are not required.
Determine if such functionalities could be exploited.
Assess if the physical attack surface is appropriately minimized.

---

## Execution Steps
Visual inspection of the PCB to identify exposed connectors or pins.
Identify protocols of connectors via traces or continuity testing.
Connect corresponding adapter or logic analyser and monitor output via serial monitor.
Monitor for unused features and possible interaction.

---

## Security-relevant Findings
No unnecessary functionalities were discovered due to limited access to the interfaces. All assessed physical features appeared to be consistent with the intended requirements of the device.

---

## Expected Secure Behaviour
Production devices should have minimized physical functionality exposure. Any necessary interfaces should be appropriately restricted.

---

## Remediation Suggestions
Remove unnecessary connectors or headers for production devices.
Protect remaining interfaces with access controls.
