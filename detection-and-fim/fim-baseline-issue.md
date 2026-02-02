## FIM Baseline Initialization Issue

### Problem
File Integrity Monitoring alerts were not generated despite modifying
files under protected directories.

### Root Cause
FIM requires a baseline of file hashes before changes can be detected.
Without an initialized baseline, no comparison occurs and no alerts
are generated.

### Key Insight
Modifying a file before a baseline exists does not trigger an alert.
This is expected behavior, not a failure.

### SOC Relevance
Understanding FIM baselines prevents false assumptions during
incident investigation and reduces false negatives.
