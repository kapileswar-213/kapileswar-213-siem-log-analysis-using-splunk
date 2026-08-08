# Firewall Log Analysis

## Use Cases
- Blocked connections
- Allowed suspicious traffic
- Port scanning
- Unusual outbound traffic

## Example SPL
```spl
index=firewall
| stats count by src_ip, dest_ip, dest_port, action
| sort -count
```
