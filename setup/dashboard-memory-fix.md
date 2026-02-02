## Wazuh Dashboard Memory Issue

### Problem
The Wazuh Dashboard service failed to start and crashed
during initialization.

### Root Cause
The dashboard is Node.js-based and exceeded default memory
allocation limits on the virtual machine.

### Resolution
Node.js memory limits were adjusted to align with the
available VM resources.

### Outcome
The dashboard service started successfully and remained stable
after the memory adjustment.
