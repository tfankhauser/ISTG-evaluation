# ISTG Test Case Identifier
ISTG-DES-INPV-001

# Name
Insufficient Input Validation

---

## Access Requirements
PA-1-4 / AA-1-4

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
BHM-2025-E11

---

## Summary of Test Case
This test case evaluates if the DES are validating received input correctly before processing it.

---

## Objectives
Assess if DES enforce validation of expected formats and ranges.
Evaluate if unexpected input or malformed requests are rejected.
Determine if system behaviour can be impacted due to insufficient validation.

---

## Execution Steps
Identify input parameters in captured network traffic.
Modify and replay requests with unexpected or malformed values.
Observe system behaviour for missing validation and analyse impact.

---

## Security-relevant Findings
It was found that some DES endpoints did not validate malformed input correctly. Unexpected values were accepted and most likely processed, though it could not be further tested and exploited in the given scope.

---

## Expected Secure Behaviour
All DES endpoints should enforce validations of expected input values. Failed validation should lead to rejected requests and error handling.

---

## Remediation Suggestions
Review current input validation mechanisms of all DES endpoints. 
Ensure correct enforcement of expected formats, ranges, and types.
Unexpected inputs should be consistently rejected and non-technical errors returned.
