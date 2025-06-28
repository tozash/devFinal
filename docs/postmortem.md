# Post-Mortem Report

| Section | Content |
| ------- | ------- |
| **Incident ID / Date** | `INC-001  2025-06-29` |
| **Impact** | Users saw 5xx errors for 3 min |
| **Timeline** | t0 20:25 kill → t1 20:26 detected → t2 20:28 fixed |
| **Root Cause** | Manual kill simulated crash |
| **Lessons Learned** | Add restart: always; set up alerts |
| **Action Items** | 1. 1 add restart: always 2 integrate Alertmanager |
