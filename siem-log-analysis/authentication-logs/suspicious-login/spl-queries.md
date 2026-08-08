# Suspicious Login SPL

```spl
index=windows EventCode=4624
| stats count by user, src_ip, host
| sort -count
```
