# Brute Force Attack

## Objective
Detect repeated failed authentication attempts that may indicate a brute-force attack.

## Relevant Events
- 4625 - Failed Logon
- 4624 - Successful Logon

## Attack Symptoms
- Many failed attempts
- Same source IP
- Same target account
- Short attack timeframe
- Successful login after repeated failures

## MITRE ATT&CK
T1110 - Brute Force

## Investigation
1. Identify source IP.
2. Identify target account.
3. Count failed attempts.
4. Check successful authentication.
5. Review endpoint activity.
6. Check lateral movement.
7. Determine severity.
