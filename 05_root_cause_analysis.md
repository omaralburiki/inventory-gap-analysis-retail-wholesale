## 5. Root Cause Analysis
 
### Layer 1 — System Failures
 
| Symptom | Root Cause | Evidence |
|---------|-----------|---------|
| Inventory is inaccurate | ERP has no real-time stock deduction mechanism | System count vs. physical count diverge within days of manual reconciliation |
| ERP does not control workflow | System was built to record transactions, not enforce them | Staff can complete a sale without any system confirmation of stock |
| No automation | ERP was built reactively without structured requirements design | No integration between POS, warehouse, and procurement modules |
 
### Layer 2 — Process Failures
 
| Gap | Description | Root Cause |
|-----|-------------|-----------|
| No stock ownership | No single person accountable for inventory variance per branch | Role not defined in org structure |
| No validation checkpoints | Items dispatched without system confirmation | Process never designed with ERP enforcement in mind |
| No cycle counting | Physical count only at year-end — not periodic | No procedure established |
| No exception handling | When items unavailable, no escalation path | Never documented as an operational scenario |
| No receiving protocol | Goods received without PO matching in system | Warehouse staff not trained on ERP receiving module |
 
### Layer 3 — Behavioral & Governance Failures
 
| Gap | Description | Impact |
|-----|-------------|--------|
| Workarounds normalized | Staff adapted to broken process — paper became "the system" | No organizational pressure to fix what appears to "work" |
| No ERP training | Staff used familiar methods — manual always replaced digital | System investment partially wasted |
| No process ownership | Nobody responsible for data quality between POS and Warehouse | Problems not escalated, not fixed |
| Management not measuring | No KPIs tracked — variance only noticed during year-end audit | No visibility into daily deterioration |
 
### Root Cause Summary
 
> **The ERP was built to record what happened — not to control what should happen.**
>
> Combined with zero process ownership, no defined accountability structure, and no measurement framework, manual workarounds became the permanent operating model across all 7 locations.
>
> **This is a governance failure, enabled by a system failure, sustained by a training failure.**
 
### 5-Whys Analysis — Inventory Variance
 
```
Why is inventory inaccurate?
└── Because stock is not deducted in real-time when dispatched
 
    Why is stock not deducted in real-time?
    └── Because the dispatch process is paper-based, not system-driven
 
        Why is the process paper-based?
        └── Because POS and warehouse systems are not integrated
 
            Why are systems not integrated?
            └── Because the ERP was built without integration requirements
 
                Why were integration requirements not defined?
                └── Because there was no structured requirements process
                    when the ERP was originally built
```
 
**Root cause:** Absence of requirements-driven ERP design from inception. Every operational failure is a downstream consequence of that one decision.
 
