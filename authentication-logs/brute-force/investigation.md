# Brute Force Investigation

## Alert
Multiple failed authentication attempts were detected against the admin account.

## Evidence
Five failed attempts from the same source IP were followed by a successful login.

## Analysis
The pattern is suspicious because repeated failures were followed by successful authentication.

## MITRE ATT&CK
T1110 - Brute Force

## Severity
High until the successful login is validated.

## Response
1. Validate the account owner.
2. Review source IP and endpoint.
3. Check post-login activity.
4. Reset credentials if compromise is confirmed.
5. Review lateral movement.
6. Document findings.
