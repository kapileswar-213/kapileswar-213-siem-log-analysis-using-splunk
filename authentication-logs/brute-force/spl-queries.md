# Brute Force SPL Queries

## Detect repeated failures
```spl
index=windows EventCode=4625
| stats count by src_ip, user
| where count >= 10
| sort -count
```

## Failed and successful logons
```spl
index=windows (EventCode=4625 OR EventCode=4624)
| stats count by src_ip, user, EventCode
| sort -count
```

## Timeline
```spl
index=windows (EventCode=4625 OR EventCode=4624)
| sort 0 _time
| table _time src_ip user EventCode host
```
