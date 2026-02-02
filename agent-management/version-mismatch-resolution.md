## Manager–Agent Version Mismatch

### Problem
Agent enrollment failed after installation despite
correct configuration.

### Root Cause
The installed agent version was higher than the
manager version, which is unsupported.

### Resolution
The agent was downgraded to match the manager version
and re-enrolled.

### Outcome
The agent connected successfully and alerts were received.
