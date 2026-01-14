# ISTG Test Case Identifier
ISTG-DES-AUTHZ-001

# Name
Unauthorized Interaction with Data Exchange Services

---

## Access Requirements
PA-1-4 / AA-1

## Component
Data Exchange Services – Cloud Services

---

## Execution Phase
Phase 6 & 7

## Tooling
Android Studio, Burp Suite Proxy

---

## Status
Executed

## Evidence ID
-

---

## Summary of Test Case
This test case evaluates if the Data Exchange Services enforce proper access control.

---

## Objectives
Identify access control mechanisms of DES.
Assess if there are ways to bypass them.

---

## Execution Steps
Identify DES endpoints and channels of the ecosystem by monitoring network traffic.
Attempt to interact with discovered endpoints without authentication.
Assess if access control is implemented correctly and if it could be bypassed.

---

## Security-relevant Findings
Authorization control was implemented properly and no unauthenticated or unauthorized interaction was possible. No bypass for these mechanisms was discovered.

---

## Expected Secure Behaviour
Communication channels and endpoints should only be accessible with correct authentication and authorization, verified by the recipient.

---

## Remediation Suggestions
Maintain current access control mechanisms.
Ensure that newly added functionalities also implement these mechanisms.
