# Sysmon Log Analysis

Sysmon provides detailed endpoint telemetry.

## Important Events
- Event ID 1 - Process Creation
- Event ID 3 - Network Connection
- Event ID 6 - Driver Loaded
- Event ID 7 - Image Loaded
- Event ID 8 - CreateRemoteThread
- Event ID 10 - Process Access
- Event ID 11 - File Created

## Investigation Chain
Process -> Parent Process -> Command Line -> User -> Network -> File Activity

A single Sysmon event should be investigated in context.
