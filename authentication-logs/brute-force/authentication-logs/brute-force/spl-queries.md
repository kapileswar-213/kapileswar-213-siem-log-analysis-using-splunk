# Brute Force SPL Queries

## Detect Multiple Failed Logins

```spl
index=windows EventCode=4625
| stats count by src_ip, user
| sort -count

## **Detect High Number of Failed Logins**

index=windows EventCode=4625
| stats count by src_ip, user
| where count >= 10
| sort -count

##  Check Successful Login After Failed Attempts

index=windows (EventCode=4625 OR EventCode=4624)
| stats count by src_ip, user, EventCode
| sort -count

