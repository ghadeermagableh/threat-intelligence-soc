# Threat Intelligence-Driven SOC Use Case

> A functional SOC lab using Wazuh SIEM, VirusTotal, and custom 
> MITRE ATT&CK-mapped detection rules to simulate and detect real cyberattacks.

## Overview
This project implements a Threat Intelligence-driven Security Operations 
Center (SOC) using Wazuh as the SIEM platform, integrated with VirusTotal 
and AbuseIPDB for live IOC enrichment.

## Methodology
  <img width="975" height="535" alt="image" src="https://github.com/user-attachments/assets/778b3d86-9172-4c15-857d-6f95d31d9229" />

## Attack Scenarios Simulated
| Attack | MITRE Technique | Detection Rule |
|--------|----------------|----------------|
| Web Discovery | T1595 | Wazuh Rule 31122 |
| SQL Injection | T1190 | Custom Rule 100512 |
| Privilege Escalation | T1068 | Custom Rule 101201 |
| Data Exfiltration | T1041 | Sysmon EID 1+3 |

## Tools Used
- Wazuh SIEM (Manager + Agent)
- Microsoft Sysmon
- VirusTotal API
- AbuseIPDB API
- Kali Linux (attacker)
- Windows Server 2022 (victim)

## Key Results
- Reduced false positives significantly through threshold-based tuning
- Achieved full kill-chain correlation across 4 attack stages
- MITRE ATT&CK mapped alerts with live threat intelligence enrichment

## Dashboard
https://192.168.3.126/app/dashboards#/view/0969d370-3a49-11f1-868a-1ff0013a4dfa?embed=true&_g=%28filters%3A%21%28%29%2CrefreshInterval%3A%28pause%3A%21t%2Cvalue%3A0%29%2Ctime%3A%28from%3Anow-1y%2Cto%3Anow%29%29&show-top-menu=true&show-query-input=true&show-time-filter=true
