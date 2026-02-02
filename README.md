# Wazuh SOC Alert Triage & Detection Lab

## Overview
This project demonstrates a real-world SOC-style deployment of Wazuh SIEM, focusing on
alert triage, Linux authentication monitoring, and File Integrity Monitoring (FIM).
It reflects real SOC challenges such as agent enrollment failures, detection gaps,
and root-cause analysis.

## Environment
- SIEM Platform: Wazuh 4.7.5
- Manager OS: Ubuntu Server
- Agent OS: Ubuntu 22.04
- Virtualization: Oracle VirtualBox
- Network: NAT + Host-only
- Logs Monitored: auth.log

## Key Challenges Solved
- Wazuh installer OS compatibility restriction
- Dashboard crash due to Node.js memory limits
- Agent enrollment and duplicate agent ID issues
- Manager–agent version mismatch
- FIM baseline and realtime detection issues

## Detections Validated
- SSH authentication failures
- SSH brute-force attempts
- Privilege escalation (sudo / PAM)
- Unauthorized file modification (FIM)

## SOC Skills Demonstrated
- SIEM monitoring and troubleshooting
- Alert triage and investigation
- Linux log analysis
- File Integrity Monitoring (FIM)
- Root cause analysis and remediation

## Repository Structure
architecture/        → Wazuh & network design  
setup/               → Installation and platform issues  
agent-management/    → Agent failures & recovery  
detection-and-fim/   → Log analysis & FIM validation  
attack-scenarios/    → Simulated security events  
screenshots/         → Dashboard & alert evidence  

## Screenshots
See the screenshots directory for alert and dashboard proof.

