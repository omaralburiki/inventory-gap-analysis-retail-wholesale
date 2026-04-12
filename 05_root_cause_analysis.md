## 🔍 Root Cause Analysis

### Layer 1 — System Failures

| Why?                      | Root Cause                                         |
| ------------------------- | -------------------------------------------------- |
| Inventory inaccurate      | No real-time update mechanism in ERP               |
| ERP doesn't control stock | Built for recording, not controlling               |
| No automation             | Custom ERP built reactively, no requirement design |

### Layer 2 — Process Failures

| Gap                       | Description                                                |
| ------------------------- | ---------------------------------------------------------- |
| No stock ownership        | No person accountable for variance per branch              |
| No validation checkpoints | Items dispatched without system confirmation               |
| No cycle counting         | Physical count only at year-end — not periodic             |
| No exception handling     | If item unavailable, no escalation path — just crossed out |

### Layer 3 — Human & Behavioral Failures

| Gap                    | Description                                                   |
| ---------------------- | ------------------------------------------------------------- |
| Workarounds normalized | Staff adapted to broken process — paper became "the system"   |
| No training on ERP     | Staff used what they knew — manual always won                 |
| No process ownership   | Nobody responsible for data quality between POS and Warehouse |

### Summary: Real Root Cause

> The ERP was built to record what happened — not to control what
> should happen. Combined with zero process ownership and no
> accountability structure, manual workarounds became the default
> operating model across all 7 locations.

**This is a governance failure, not just a system failure.**
