\# Week 04 — First attack simulation detected



\## Status: Complete ✅



\## Attack chain executed

\- Phase 1: Nmap port scan → discovered SSH port 22 open

\- Phase 2: Hydra brute force → cracked password in <1 second

\- Phase 3: Successful SSH logon from Kali to Windows 11



\## Detection results

| Attack | Detected | Event ID | Rule |

|---|---|---|---|

| Network logon | ✅ YES | 4624 | 67023 |

| Session destroyed | ✅ YES | 4634 | 67023 |



\## Key learning

\- logonType 3 = network logon = suspicious if unexpected source IP

\- logonType 5 = service = normal, ignore



\## Next week

\- PowerShell payload simulation

\- Custom brute force correlation rule

