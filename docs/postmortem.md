# Post-Mortem Report

| Section | Content |
| ------- | ------- |
| **Incident ID / Date** | `INC-001  2025-06-??` |
| **Impact** | Users saw errors for N minutes |
| **Timeline** | *t0*, *t1*, *t2* |
| **Root Cause** | Manual kill simulated crash |
| **Lessons Learned** | Need automated restarts (restart: always) |
| **Action Items** | 1. Add healthcheck 2. Alertmanager next |
