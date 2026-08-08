# Port Scanning

A host contacting many destination ports in a short period can indicate scanning.

## Example SPL
```spl
index=network
| stats dc(dest_port) as unique_ports by src_ip
| where unique_ports > 20
| sort -unique_ports
```

Validate whether the source is a scanner, administrator or authorized security tool before escalation.
