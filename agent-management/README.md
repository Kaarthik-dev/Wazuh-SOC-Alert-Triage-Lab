# Agent Management & Troubleshooting

## Objective
Onboard Linux agents into Wazuh SIEM and ensure reliable communication with
the Wazuh Manager.

## Issues Encountered
- Agent enrollment failures
- Duplicate agent ID conflicts
- Manager–agent version mismatch
- Agent appearing active but not generating alerts

## Root Causes
- Agent identity is stored on the manager
- Agent version higher than manager version
- Stale agent keys during re-enrollment

## Resolution
- Removed conflicting agents from manager
- Installed matching agent version
- Re-enrolled agent with clean identity

## Validation
- Agent status confirmed as Active
- Alerts successfully received in the dashboard

