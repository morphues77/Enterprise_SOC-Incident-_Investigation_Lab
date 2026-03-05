# Persistence Mechanism Simulation

Objective:
Create persistence to maintain system access.

Command:
schtasks /create /sc onlogon /tn backdoor /tr "cmd.exe"

Alternative Persistence:
Registry Run Key modification.