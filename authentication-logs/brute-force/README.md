# Brute Force Attack Investigation

## Objective

Detect multiple authentication failures that may indicate
a brute-force attack.

## Log Source

Windows Security Logs

## Important Event IDs

- 4625 - Failed Logon
- 4624 - Successful Logon

## Attack Symptoms

- Multiple failed logins
- Same source IP
- Same username
- Many attempts within a short period
- Successful login after multiple failures

## Investigation

1. Identify the source IP.
2. Identify the target account.
3. Count failed attempts.
4. Check the attack timeframe.
5. Look for successful authentication.
6. Check other activity from the source IP.
7. Determine whether the activity is malicious.

## MITRE ATT&CK

T1110 - Brute Force
