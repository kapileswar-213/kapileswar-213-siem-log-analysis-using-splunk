# Windows Event Logs

## Important Events

| Event ID | Description | SOC Use |
|---|---|---|
| 4624 | Successful logon | Authentication |
| 4625 | Failed logon | Brute force |
| 4672 | Special privileges assigned | Privileged activity |
| 4688 | Process creation | Execution |
| 4697 | Service installed | Persistence |
| 7045 | Service installed | Persistence |

## Investigation Principle
Correlate authentication, process, service and network events rather than relying on one event alone.
