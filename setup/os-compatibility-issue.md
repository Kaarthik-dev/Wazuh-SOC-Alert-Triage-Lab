## OS Compatibility Check Issue

### Problem
The Wazuh installer reported that the operating system version
was unsupported during installation.

### Root Cause
The installer performs OS version validation and did not yet
include Ubuntu 24.04 in its supported list.

### Resolution
The installation was continued by bypassing the OS compatibility
check using a documented override option.

### Outcome
The Wazuh services installed and operated correctly,
confirming this was a validation check rather than
a functional compatibility issue.
