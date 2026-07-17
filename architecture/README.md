# 🛡️ Home SOC Lab

> Building a functional Security Operations Center from scratch 
> using 100% open-source tools — documented week by week.

![Architecture](architecture/architecture-diagram.drawio.png)

---

## 🎯 Project Goal

Most SOC learning resources teach theory.
This project builds the real thing.

The goal is to deploy a complete attack-detect-respond pipeline 
in a home lab — simulating real threats, detecting them with 
production-grade tools, and responding as a SOC analyst would.

**Target environment:** Small and Medium-sized Businesses (SMB)  
**Approach:** Build it, break it, document everything.

---

## 🏗️ Architecture

### Phase 1 — Core Detection (Current)

| Machine | Role | Tools |
|---|---|---|
| Kali Linux | Attacker simulation | Nmap · Hydra · PowerShell |
| Windows 11 | Victim endpoint | Wazuh Agent · Sysmon · Windows Event Logs · FIM |
| Ubuntu Server 22.04 | SIEM / EDR | Wazuh Manager · Wazuh Indexer · Wazuh Dashboard |

**Detection cycle:**
