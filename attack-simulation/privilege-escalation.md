# Privilege Escalation Simulation

Objective:
Demonstrate unauthorized elevation of privileges.

Command:
net localgroup administrators testuser /add

Detection:
Windows Event ID 4732 – User added to Administrator group.