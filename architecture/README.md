# Wazuh SIEM Architecture

## Objective
Define and document the architecture of the Wazuh SIEM lab, including
component roles, data flow, and network segmentation from a SOC perspective.

---

## Architecture Overview

The lab is designed as a **centralized SIEM deployment** with one Wazuh Manager
and one Linux endpoint agent.

Components:
- **Wazuh Manager** – Log analysis, rule processing, and alert generation
- **Wazuh Indexer (OpenSearch)** – Stores and indexes security events
- **Wazuh Dashboard** – SOC analyst interface for alert triage and investigation
- **Wazuh Agent (Linux)** – Collects logs and file integrity data from the endpoint

---

## Network Design

The environment uses a **dual-adapter network model** to balance connectivity
and security:

- **NAT Adapter**
  - Provides internet access for package installation and updates
  - Isolates the VM from direct inbound connections

- **Host-Only Adapter**
  - Enables secure access from host to Wazuh Dashboard
  - Allows manager–agent communication within a private subnet

This design mirrors common **SOC lab and enterprise test environments**.

---

## Data Flow

1. Linux agent collects:
   - Authentication logs (`/var/log/auth.log`)
   - File integrity events (syscheck)
2. Agent sends events securely to Wazuh Manager (TCP 1514)
3. Manager processes logs using decoders and rules
4. Alerts are indexed in OpenSearch
5. SOC analysts investigate alerts using Wazuh Dashboard

---

## Security Considerations

- Agent–manager communication restricted to required ports
- No direct internet exposure of SIEM services
- Host-only network limits attack surface
- Principle of least privilege applied at OS level

---

## Diagram

Refer to the architecture diagram in this directory:
- `wazuh-architecture.png`
- `network-design.png`

