# Brute Force SPL Queries

## Detect Multiple Failed Logins

```spl
index=windows EventCode=4625
| stats count by src_ip, user
| sort -count
