\# Week 03 — Full Sysmon telemetry unlocked



\## Status: Complete ✅



\## What was done

\- Identified 74 suppressed Sysmon rules (level 0)

\- Wrote Python script to generate XML override rules

\- Promoted all 74 rules from level 0 to level 3

\- Backed up rules before applying changes

\- Restarted Wazuh Manager — all services active



\## Events now visible that were previously discarded

\- PowerShell script execution (T1059.001)

\- Reg.exe registry modification (T1112)

\- WMI process creation (T1047)

\- Netsh firewall changes (T1562.004)



\## Next week

\- First attack simulation from Kali Linux

\- nmap scan, Hydra brute force, PowerShell payload

\- Document which alerts fire and at what severity

