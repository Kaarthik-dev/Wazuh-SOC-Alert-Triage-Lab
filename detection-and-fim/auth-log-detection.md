## Authentication Log Detection

### Objective
Validate Wazuh detection of Linux authentication events using log analysis.

### Logs Monitored
- /var/log/auth.log

### Events Observed
- Successful SSH login
- Failed SSH login attempts
- sudo privilege escalation
- PAM session open/close

### Detection Logic
Wazuh parses authentication logs using decoders and rules.
Security alerts are generated based on event type and frequency.

### SOC Analyst View
Authentication alerts are used to:
- Identify brute-force attempts
- Detect unauthorized access
- Investigate privilege escalation activity
