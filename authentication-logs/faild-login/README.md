# Failed Login Investigation

## Objective
Identify repeated authentication failures and determine whether they are benign or suspicious.

## Relevant Windows Event
- 4625 - Failed Logon

## Investigation
1. Identify user.
2. Identify source IP.
3. Count failures.
4. Check timeframe.
5. Check whether a successful login followed.
6. Investigate other activity from the source IP.
7. Determine whether the activity is malicious.

## Severity
Depends on frequency, target account, source reputation and whether compromise occurred.
