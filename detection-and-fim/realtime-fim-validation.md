## Realtime File Integrity Monitoring Validation

### Objective
Validate realtime File Integrity Monitoring (FIM) alerts in Wazuh.

### Configuration Summary
Protected directories were monitored with realtime FIM enabled
to detect file creation and modification events.

### Validation Activity
A system file under /etc was modified to simulate unauthorized access.

### Observed Alert
- Integrity checksum changed
- Severity level: 7
- Rule group: syscheck

### SOC Analyst Action
- Verify legitimacy of file change
- Identify user context and timestamp
- Escalate if change is unauthorized
