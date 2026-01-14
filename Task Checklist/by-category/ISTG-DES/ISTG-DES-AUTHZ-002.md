# ISTG Test Case Identifier
ISTG-DES-AUTHZ-002

# Name
Privilege Escalation in DES

---

## Access Requirements
PA-1-4 / AA-2-3

## Component
Data Exchange Services – Cloud Services

---

## Execution Phase
Phase 6

## Tooling
Android Studio, Burp Suite Proxy

---

## Status
Executed

## Evidence ID
-

---

## Summary of Test Case
This test case assesses if the DES implement authorization separation between privilege levels.

---

## Objectives
Identify possible privilege levels.
Assess if privileged interaction is restricted to privileged roles.
Evaluate if it is possible to manipulate the separation mechanisms to execute higher-privileged functionalities.

---

## Execution Steps
Identify DES endpoints and channels and observable privilege levels.
Attempt to interact with them in a lower-privileged context. 
Evaluate if there are ways to gain a higher privilege context by manipulating requests or communication.

---

## Security-relevant Findings
No privilege escalation vulnerabilities were discovered, due to the lack of identified authorization levels. Only one authenticated context was observed; unauthorized interaction was assessed in ISTG-DES-AUTHZ-001.

---

## Expected Secure Behaviour
Data exchange services should implement strict separation between authorization roles. It should not be possible to perform operations meant for higher-privileged contexts.

---

## Remediation Suggestions
Ensure that authorization separation is implemented in all channels. 
Avoid a “one-role-only” permission management.
