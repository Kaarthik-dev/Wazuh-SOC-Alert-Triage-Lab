## Attack Scenario: SSH Brute Force

### Objective
Simulate repeated SSH authentication failures to validate Wazuh detection
of brute-force login attempts.

### Attack Method
Multiple failed SSH login attempts were generated against a Linux host
using invalid usernames.

### Logs Involved
- /var/log/auth.log

### Detection Logic
Wazuh monitors authentication failures via log analysis.
Repeated failures trigger high-severity alerts mapped to brute-force behavior.

### Observed Alerts
- sshd: Attempt to login using a non-existent user
- PAM: User login failed
- Alert severity increased with repeated attempts

### SOC Analyst Action
- Identify affected host and source IP
- Correlate failed attempts within a time window
- Escalate if threshold is exceeded
