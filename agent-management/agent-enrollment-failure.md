## Agent Enrollment Failure

### Problem
The Wazuh agent failed to enroll with the manager
despite correct network connectivity.

### Root Cause
Agent authentication issues and stale identity data
on the manager prevented successful enrollment.

### Resolution
The agent was re-registered after cleaning old
identity data on the manager.

### Outcome
The agent enrolled successfully and began sending events.
