# SOC Level 2 – Advanced Detection Lab

An advanced Security Operations Center (SOC) lab focused on detection engineering, security monitoring, attack simulation, and threat detection using Wazuh SIEM.

This project builds on foundational SOC knowledge by implementing custom detection rules, collecting endpoint and web server telemetry, mapping detections to MITRE ATT&CK, and investigating simulated attacker activity.

## Project Overview

The lab demonstrates an end-to-end detection workflow, from collecting security logs to generating alerts and analyzing suspicious activity.

The environment integrates Windows, Linux, and an Apache web server with Wazuh to provide centralized security monitoring and detection capabilities.

### Objectives

- Centralize security telemetry from multiple operating systems.
- Develop and tune custom Wazuh detection rules.
- Detect simulated attacker behavior.
- Map detection logic to the MITRE ATT&CK framework.
- Build security dashboards for monitoring and investigation.
- Analyze alerts and document detection results.

## Technology Stack

| Technology | Purpose |
|---|---|
| Wazuh SIEM | Centralized security monitoring and detection |
| Windows | Endpoint security monitoring |
| Sysmon | Detailed Windows process and system telemetry |
| Linux | Authentication and system activity monitoring |
| Apache | Web server log collection and attack detection |
| MITRE ATT&CK | Adversary technique classification |
| Custom Wazuh Rules | Detection logic and alert generation |

## Lab Architecture

The lab uses a centralized monitoring architecture in which endpoint agents forward security events to Wazuh for analysis and alert generation.

**Log flow:**

Windows Endpoint + Sysmon ─┐  
Linux Endpoint ────────────┼──> Wazuh SIEM ──> Alerts and Dashboards  
Apache Web Server ─────────┘

> Add your final architecture diagram here when it is uploaded to the repository.

## Detection Engineering

Custom Wazuh detection rules were developed to identify selected attacker behaviors and suspicious activity.

The detection workflow includes:

- Security event collection and analysis.
- Custom rule development.
- Detection testing through controlled attack simulations.
- Rule tuning to reduce false positives.
- MITRE ATT&CK technique mapping.
- Alert investigation and triage documentation.

## Attack Simulations

The lab includes controlled simulations designed to validate detection capabilities.

Examples of attack behaviors investigated include:

- Network reconnaissance and port scanning.
- SSH brute-force attempts.
- Suspicious PowerShell execution.
- Persistence mechanisms.
- Web-based attack activity.

All simulations are intended for authorized testing within the isolated lab environment.

## Dashboards and Monitoring

Wazuh dashboards provide visibility into collected security events, detection alerts, and suspicious activity.

Screenshots of the implemented dashboards and detection results will be added to this repository.

## Project Documentation

| Resource | Description |
|---|---|
| Technical Report | Lab architecture, implementation, detections, and results |
| Detection Rules | Custom Wazuh rules and detection logic |
| Architecture Diagram | Lab components and log flow |
| Dashboard Screenshots | Monitoring and alert visualization |
| Attack Simulation Results | Simulated activity and corresponding detections |

## Key Learning Outcomes

- SIEM deployment and endpoint integration.
- Security telemetry collection and analysis.
- Detection rule development and tuning.
- MITRE ATT&CK mapping.
- Attack simulation and detection validation.
- Alert investigation and SOC triage.
- Technical security documentation.

## Security Notice

This project is intended for educational purposes and authorized defensive security testing.

All attack simulations must remain within systems owned or explicitly authorized by the operator.

## Author

**Taher Alomary**

Cybersecurity | SOC Operations | SIEM | Detection Engineering
