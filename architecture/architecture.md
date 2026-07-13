# Home SOC Lab Architecture

## Overview

This project simulates a small SOC environment using:

- Kali Linux as attacker machine
- Windows 11 as monitored endpoint
- Ubuntu Server as SIEM server
- Wazuh as security monitoring platform


## Components

| System | Role |
|---|---|
| Kali Linux | Attack simulation |
| Windows 11 | Endpoint monitoring |
| Ubuntu Server | Wazuh SIEM |
| Wazuh | Detection and alerting |


## Data Flow

Kali Linux generates security events.

Windows and Linux agents collect telemetry.

Wazuh Manager analyzes logs and generates alerts.

The SOC analyst investigates detected activity.
