# ISTG Test Case Identifier
ISTG-DES-INFO-003

# Name
Disclosure of User Data

---

## Access Requirements
PA-1 / AA-1-4

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
This test case evaluates if the communication of the data exchange services exposes user specific data in an unauthorized context.

---

## Objectives
Determine if user information is exposed to unauthorized actors.
Assess if separation between data of different users is separated correctly.

---

## Execution Steps
Intercept DES communication and inspect for user-related data.
Attempt to access user data outside of authorized context via request manipulation.
Assess if exposed data should be accessible.

---

## Security-relevant Findings
The DES did not show any unauthorized disclosure of user-related data. This information was only accessible in an authorized context.

---

## Expected Secure Behaviour
Authorization controls must be in place, preventing unauthorized access to user data. These access control mechanisms should be enforced on all related endpoints.

---

## Remediation Suggestions
Review access control mechanisms for user-specific data endpoints.
Maintain current implementation for future development.
