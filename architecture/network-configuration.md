# Network Configuration

All virtual machines are connected using an Internal Network called **SOC-LAB**.

| Machine | Role | IP Example |
|--------|------|------------|
| Kali Linux | Attacker | 192.16X.Xx.X |
| Windows 11 | Victim | 192.16X.Xx.X |
| Wazuh Server | SIEM | 192.1XX.Xx.X |

Steps:
1. Configure VirtualBox adapter to Internal Network.
2. Assign static or DHCP IPs within same subnet.
3. Verify connectivity using ping.