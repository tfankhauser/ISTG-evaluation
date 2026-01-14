# ISTG Test Case Identifier
ISTG-PHY-AUTHZ-001

# Name
Unauthorized Interaction with Physical Ports

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
This test case evaluates whether the physical interfaces allow unauthorized interaction. This could include access to internal data, manipulation, or code execution. Physical ports are identified and interactively tested.

---

## Objectives
Identify exposed physical interfaces (UART, SWD, …).
Assess if interaction is possible without authorisation.
Assess if access enables reading data or device manipulation.

---

## Execution Steps
Visual inspection of the PCB to identify exposed connectors or pins.
Identify protocols of connectors via traces or continuity testing.
Connect corresponding adapter and monitor output via any serial monitor.
Attempt interaction by sending commands and assess response.

---

## Security-relevant Findings
Physical interfaces are present on both components. No interactive interface was accessible and no sensitive information was disclosed. UART interface logs boot information and SWD interfaces are locked by MCU.

---

## Expected Secure Behaviour
Physical interfaces should be protected through appropriate access control mechanisms. Interactive debugging interfaces should be disabled or locked on shipped devices. Any accessible output should be limited to non-sensitive information.

---

## Remediation Suggestions
Disable or restrict physical interfaces for production devices.
Remove unnecessary pin headers to prevent non-destructive probing.
