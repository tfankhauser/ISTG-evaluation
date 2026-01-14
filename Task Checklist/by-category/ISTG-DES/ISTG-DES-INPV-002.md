# ISTG Test Case Identifier
ISTG-DES-INPV-002

# Name
Command or Code Injection

---

## Access Requirements
PA-1-4 / AA-1-4

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
This test case evaluates if assessed DES are vulnerable to injection attacks. These would allow an attacker to inject code or commands due to insecure input handling.

---

## Objectives
Assess if injected code or commands are executed or processed.
Determine if input is properly sanitized and handled.

---

## Execution Steps
Identify possible attack vectors in DES endpoints through network analysis.
Inject command or code payloads into discovered parameters.
Observe system behaviour, responses and error handling.
Evaluate if injected payloads are executed, processed, or rejected.

---

## Security-relevant Findings
No injection vulnerabilities were discovered in the DES within the permitted scope. Attempted payloads were consistently rejected, and no evidence of execution or processing was identified.

---

## Expected Secure Behaviour
DES processes should validate and sanitize all user input before processing and should never be interpreted as commands or code.

---

## Remediation Suggestions
Maintain current input handling and sanitization. 
Ensure “Zero-Trust” principle for all user input in future development.
