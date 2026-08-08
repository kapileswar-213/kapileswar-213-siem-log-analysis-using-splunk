# DNS Log Analysis

## Use Cases
- Suspicious domains
- DNS tunneling
- DGA-like activity
- High-volume DNS requests

## Example SPL
```spl
index=dns
| stats count by src_ip, query
| sort -count
```

DNS indicators require context and should be validated with threat intelligence and endpoint activity.
