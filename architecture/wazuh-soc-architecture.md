[ Linux Agent ]
     |
     |  (Logs, FIM, Syscheck)
     |
[ Wazuh Manager ]
     |
     |  (Alerts / Events)
     |
[ Wazuh Indexer ]
     |
     |  (Search / Dashboards)
     |
[ Wazuh Dashboard ]

Agent OS (Ubuntu 22.04)
Manager (Wazuh Manager)
Indexer (OpenSearch)
Dashboard (Web UI)
Protocols:
TCP 1514 (agent → manager)
HTTPS 443 (dashboard)
