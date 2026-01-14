# ISTG Test Case Identifier
ISTG-DES-SCRT-001

# Name
Access to Sensitive Data

---

## Access Requirements
PA-3 / AA-2

## Component
Data Exchange Services – Cloud Services

---

## Execution Phase
Phase 6 & 7

## Tooling
Android Studio, Burp Suite Proxy, mosquitto

---

## Status
Executed

## Evidence ID
BHM-2025-E08, BHM-2025-E09

---

## Summary of Test Case
This test case evaluates if the cloud API exposes confidential data, such as credentials, through authenticated endpoints accessible by the mobile application. The scope includes verifying whether unintended sensitive information is retrievable by clients.

---

## Objectives
Determine if API endpoints return credentials.
Assess if MQTT credentials are exposed.
Identify if the API enforces separation between user and device privileges.

---

## Execution Steps
1. Start Burp Suite and Android Studio Virtual Device set up with Burp Proxy
2. Launch the BHMs mobile application on the emulator
3. Monitor HTTP(S) traffic during legitimate usage of the application
4. Identify a request to an endpoint which returns MQTT credentials for base station
5. Extract the MQTT username, password, and client_id
6. Verify credentials using:
mosquitto_pub -d -q 1 -h <mqtt_broker> -p 8883 -t v1/devices/me/telemetry -i "<client_id>" -u "<username>" -P "<password>" -m "{temperature:25}"

---

## Security-relevant Findings
The API exposed static device specific MQTT credentials for the base station to any authenticated request. The credentials provided full publish/subscribe permissions and could allow a user to impersonate the base station and possibly influence the cloud’s behaviour. This results in a significant information disclosure vulnerability.

---

## Expected Secure Behaviour
Device-level secrets should never be accessible by client applications. API endpoints must enforce strict privilege separation and authentication.

---

## Remediation Suggestions
Replace static credentials with short-lived tokens bound to device identity. 
Prevent user-facing clients from querying device-level authentication data. 
Implement role-based access control on API endpoints.
