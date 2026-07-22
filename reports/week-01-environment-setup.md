

\# Week 01 — Environment Setup



\## Status: Complete ✅



\## What was deployed

\- Kali Linux — attacker VM (192.168.100.10)

\- Windows 11 — victim endpoint (192.168.100.30)

\- Ubuntu Server 22.04 — Wazuh stack (192.168.100.20)



\## Network configuration

\- NAT adapter: internet access (10.0.2.x)

\- Host-Only adapter: lab communication (192.168.100.0/24)



\## Issues encountered and fixed

1\. All VMs got same IP 10.0.2.15 — fixed with Host-Only adapter

2\. Windows Firewall blocking ICMP — fixed with PowerShell rule

3\. Ubuntu 26.04 incompatible with Wazuh — reinstalled 22.04

4\. Root partition 100% full — LVM expanded from 39GB to 77GB

5\. Password special characters rejected — used allowed symbols



\## Wazuh stack status

\- wazuh-manager: active ✅

\- wazuh-indexer: active ✅

\- wazuh-dashboard: active ✅

\- Dashboard URL: https://192.168.100.20



\## Next week

\- Install Sysmon on Windows 11 (Olaf Hartong config)

\- Apply Wazuh rule override for full Sysmon telemetry

\- First attack simulation from Kali

