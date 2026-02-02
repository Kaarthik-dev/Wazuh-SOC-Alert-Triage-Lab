# Detection Engineering & File Integrity Monitoring

## Authentication Log Monitoring
Monitored Linux authentication logs (auth.log) to detect:
- SSH login failures
- Successful authentication events
- Privilege escalation using sudo and PAM

## File Integrity Monitoring (FIM)
Configured syscheck to monitor critical directories such as /etc
with baseline initialization and realtime detection enabled.

## Challenges
- No alerts due to missing FIM baseline
- Misunderstanding between log analysis and file integrity monitoring

## Resolution
- Initialized FIM baseline correctly
- Enabled realtime monitoring and content change reporting

## Outcome
Unauthorized file modifications successfully generated integrity alerts.

