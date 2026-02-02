# Wazuh SIEM Setup & Installation

## Objective
Deploy a fully functional Wazuh SIEM (Manager, Indexer, Dashboard) in a lab
environment and resolve installation and platform-level issues.

## Issues Encountered
- Unsupported OS version warning during installation
- Dashboard service failing due to Node.js memory limits
- Networking issues related to NAT and Host-only adapters

## Key Fixes
- Overrode OS compatibility check for Ubuntu 24.04
- Tuned Node.js memory allocation for Wazuh Dashboard
- Implemented dual-network setup (NAT + Host-only)

## Outcome
Wazuh Manager, Indexer, and Dashboard successfully deployed and accessible.

