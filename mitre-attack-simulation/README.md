# MITRE ATT&CK Threat Detection Lab

## Overview
Simulation and detection of a three-stage attack chain using the MITRE ATT&CK framework on a Windows 11 virtual machine lab environment.

## Environment
- Windows 11 Pro VM (WIN11-TARGET)
- Oracle VirtualBox
- Sysmon v15 (Olaf Hartong config)
- Splunk Enterprise 10.4

## Techniques Simulated & Detected

| Technique | MITRE ID | Tactic | Detection |
|---|---|---|---|
| PowerShell Execution | T1059.001 | Execution | Splunk SPL + Alert |
| Scheduled Task Creation | T1053.005 | Persistence | Splunk SPL + Alert |
| Masquerading | T1036.005 | Defense Evasion | Splunk SPL + Alert |

## Files
- `/report` — Full threat detection report (PDF/Word)
- `/screenshots` — Splunk detection evidence
- `/splunk-queries` — SPL detection queries for each technique

## Key Findings
- All three techniques were detected via Sysmon EventID 1 (Process Creation)
- Sysmon with Olaf Hartong config automatically tags MITRE ATT&CK technique IDs
- Single attacker actions can trigger multiple MITRE technique detections simultaneously
- Three scheduled Splunk alert rules deployed for ongoing detection capability

## Tools & References
- [MITRE ATT&CK Framework](https://attack.mitre.org)
- [Sysmon by Microsoft Sysinternals](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon)
- [Olaf Hartong Sysmon Config](https://github.com/olafhartong/sysmon-modular)
- [Splunk Enterprise](https://www.splunk.com)