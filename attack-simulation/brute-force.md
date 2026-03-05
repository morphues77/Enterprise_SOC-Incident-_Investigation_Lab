# Brute Force Attack Simulation

Objective:
Simulate repeated authentication failures against the Windows host.

Tool Used:
Hydra

Command:
hydra -l administrator -P rockyou.txt smb://192.16X.Xx.X

Logs Observed:
Windows Event ID 4625 (Failed Login)
Windows Event ID 4624 (Successful Login)