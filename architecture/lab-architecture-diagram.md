                +----------------------+
                |      Kali Linux      |
                |      (Attacker)      |
                |  Hydra Brute Force   |
                +----------+-----------+
                           |
                           | Internal Network
                           |
+--------------------------+---------------------------+
|                                                      |
|                  SOC LAB NETWORK                     |
|                                                      |
+-----------+--------------------------+---------------+
            |                          |
            |                          |
+-----------v-----------+     +--------v--------+
|      Windows 11       |     |      Wazuh      |
|      (Victim)         |     |   SIEM Server   |
|                       |     |                 |
|  Sysmon Installed     |---->| Log Collection  |
|  Event Logs Generated |     | Alert Detection |
+-----------------------+     +-----------------+

Attacker → Brute Force → Windows Logs Generated → Wazuh Collects Logs → Alert → SOC Investigation