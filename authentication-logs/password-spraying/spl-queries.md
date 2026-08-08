# Password Spraying SPL

```spl
index=windows EventCode=4625
| stats dc(user) as unique_users count by src_ip
| where unique_users >= 5
| sort -unique_users
```

Investigate the source IP, targeted users, timeframe and whether any account later authenticated successfully.
