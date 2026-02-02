## Attack Scenario: Unauthorized File Modification

### Objective
Validate File Integrity Monitoring (FIM) by detecting unauthorized
changes to protected system files.

### Attack Method
A system file under /etc was modified to simulate unauthorized access.

### Files Monitored
- /etc/hosts

### Detection Logic
Wazuh syscheck monitors protected directories and detects file
creation or modification using checksums.

### Observed Alerts
- Integrity checksum changed
- Severity level: 7

### SOC Analyst Action
- Confirm file change legitimacy
- Review change timestamp and user context
- Escalate if modification is unauthorized
