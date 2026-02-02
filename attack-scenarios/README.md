## Attack Scenarios Overview

This directory contains simulated attack scenarios used to validate
Wazuh SIEM detection and SOC alert triage workflows.

Each scenario focuses on common, real-world security events
encountered by SOC analysts.

### Included Scenarios

- **SSH Brute Force**  
  Simulates repeated authentication failures to validate detection
  of brute-force login attempts using Linux authentication logs.

- **Unauthorized File Modification (FIM)**  
  Simulates unauthorized changes to protected system files to validate
  File Integrity Monitoring (syscheck) alerts.

Each scenario includes detection logic, observed alerts, and
SOC analyst response considerations.
