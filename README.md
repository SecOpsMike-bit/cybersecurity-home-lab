# 🛡️ Cybersecurity Home Lab
> SOC Analyst portfolio — detection engineering, incident response, and threat analysis projects documented from a working home lab.

**Michael Isiuwa** | Security+ | Network+ | CySA+  
📍 Toronto, ON | [LinkedIn](http://www.linkedin.com/in/michaelisiuwa)

---

## 🔧 Lab Environment

| Tool | Purpose | Status |
|------|---------|--------|
| Splunk Enterprise 10.4 | Local SIEM — log ingestion & detection | ✅ Active |
| Sysmon v15 (Olaf Hartong config) | Endpoint telemetry & ATT&CK tagging | ✅ Active |
| Elastic Security (Cloud) | EDR — endpoint detection & response | ✅ Active |
| Wireshark 4.6.5 | Network packet capture & analysis | ✅ Active |
| Nmap 7.99 | Network scanning & enumeration | ✅ Active |
| VirtualBox 7.x | Virtualisation — isolated lab environment | ✅ Active |

**Endpoint monitored:** Windows 11 (WIN11-TARGET)  
**Events ingested:** 44,000+ Windows Security & Sysmon events

---

## 📁 Projects

### ✅ Project 1 — Brute Force Detection & Investigation

Built a real-time Splunk detection rule for brute force login attempts. Simulated an attack using PowerShell, triggered the alert, and documented a full investigation report.

- **Tools:** Splunk, Windows Event Logs, PowerShell
- **Key skills:** SPL query writing, alert tuning, false positive analysis, incident reporting
- 📄 [Investigation Report](splunk/reports/)
- 🔍 [SPL Detection Query](splunk/queries/)

---

### ✅ Project 2 — MITRE ATT&CK Simulation & Detection

Built a Windows 11 VM from scratch, instrumented it with Sysmon feeding Splunk, then simulated three MITRE ATT&CK techniques and detected all three. Documented the full chain from execution to detection in a formal threat detection report.

- **Techniques:** PowerShell Execution (T1059.001), Scheduled Task Persistence (T1053.005), Masquerading (T1036.005)
- **Tools:** Splunk Enterprise, Sysmon v15, Windows 11 VM, VirtualBox
- **Key skills:** ATT&CK technique mapping, detection engineering, threat hunting, SPL query writing, incident reporting
- 📄 [Threat Detection Report](mitre-attack-simulation/report/)
- 🔍 [SPL Detection Queries](mitre-attack-simulation/splunk-queries/)
- 📸 [Detection Screenshots](mitre-attack-simulation/screenshots/)

---

## 🎯 About This Lab

This lab was built to develop hands-on SOC analyst skills beyond certifications. Every project simulates real-world scenarios — from writing detection rules to investigating alerts to producing professional incident reports.

**Background:** 10+ years in operations and logistics — bringing operational thinking, triage discipline, and stakeholder communication to cybersecurity.

---

*Updated regularly as projects are completed.*
