# Failed Login SPL

## Basic search
```spl
index=windows EventCode=4625
```

## Count failures by user
```spl
index=windows EventCode=4625
| stats count by user
| sort -count
```

## Count failures by source IP
```spl
index=windows EventCode=4625
| stats count by src_ip
| sort -count
```
