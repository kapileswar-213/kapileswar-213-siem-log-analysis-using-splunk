# Encoded PowerShell

Encoded PowerShell requires additional investigation because encoding can hide command content.

## Investigation
1. Capture full command line.
2. Identify parent process.
3. Identify user.
4. Decode only in an authorized analysis environment.
5. Examine resulting behavior.
6. Correlate with file and network events.
