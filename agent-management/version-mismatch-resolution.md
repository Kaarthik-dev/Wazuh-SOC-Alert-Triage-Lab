## Problem
Agent enrollment failed despite correct configuration.

## Root Cause
Agent version (4.x) was higher than manager version (4.7.5).
Wazuh requires agent ≤ manager version.

## Fix
- Removed old agent from manager
- Installed matching agent version
- Re-enrolled agent

## Validation
Agent status: Active
Alerts received in dashboard
