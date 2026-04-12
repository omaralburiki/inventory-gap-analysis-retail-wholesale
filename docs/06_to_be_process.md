## ✅ TO-BE Process (Proposed Solution)

### Improved Sales Fulfillment Workflow

[POS Staff] → System shows LIVE stock availability
↓
[POS Staff] → Confirms order digitally (only available items)
↓
[System] → Generates picking list → Sent to Warehouse screen/device
↓
[Warehouse Staff] → Picks items using barcode scanner
→ System confirms dispatch in real-time
↓
[Invoice] → Auto-generated based on confirmed dispatch
↓
[Inventory] → Updated automatically — no manual entry

---

## ⚠️ Implementation Constraints & Risks

### Known Constraints

| Constraint             | Detail                                                                                  |
| ---------------------- | --------------------------------------------------------------------------------------- |
| Custom ERP limitations | Existing system may not support native integration — API or middleware needed           |
| SKU complexity         | 10,000+ SKUs with multi-origin duplicates require normalization BEFORE automation       |
| Staff readiness        | Warehouse and POS staff trained on paper — digital shift requires structured onboarding |
| Budget sensitivity     | Mid-sized trading company — full WMS replacement not feasible short-term                |

### Risk Register

| Risk                                   | Probability | Impact | Mitigation                                             |
| -------------------------------------- | ----------- | ------ | ------------------------------------------------------ |
| ERP integration failure                | Medium      | High   | Pilot in 1 branch before full rollout                  |
| Staff resistance to change             | High        | High   | Change champion per branch + phased training           |
| Barcode not readable (damaged/missing) | Medium      | Medium | Manual override protocol + re-labeling SOP             |
| Data migration errors (SKU cleanup)    | High        | High   | Freeze new SKU creation during normalization phase     |
| System downtime during transition      | Low         | High   | Paper fallback SOP maintained for 90 days post-go-live |

---

## 🔄 Change Management Plan

| Phase         | Action                                         | Owner           |
| ------------- | ---------------------------------------------- | --------------- |
| Pre-launch    | Communicate why — not just what                | Branch Managers |
| Training      | Role-based: POS staff, Warehouse staff, Buyers | Operations Lead |
| Pilot         | 1 branch, 30 days, measure variance daily      | Systems Team    |
| Feedback loop | Weekly review — capture exceptions             | Process Owner   |
| Full rollout  | Only after pilot KPIs confirmed                | Management      |

---

## ❌ Failure Scenarios & Exception Handling

| Scenario                                                  | What Happens Now (AS-IS)                        | What Should Happen (TO-BE)                                                           |
| --------------------------------------------------------- | ----------------------------------------------- | ------------------------------------------------------------------------------------ |
| Item shows available in system but physically missing     | Customer discovers at warehouse — order delayed | System triggers stock discrepancy alert → supervisor notified before order confirmed |
| Barcode damaged or unreadable                             | Not applicable — no barcodes used               | Manual override with supervisor approval → incident logged                           |
| System downtime                                           | Operations continue on paper — data lost        | Paper fallback SOP → data re-entered within 2 hours with timestamp                   |
| Same product exists under 3 different SKUs (multi-origin) | Staff picks wrong SKU — counted separately      | SKU normalization with primary code + origin attribute                               |
| Customer requests substitution                            | Handled verbally — not recorded                 | Substitution logged in system → demand data preserved                                |
| Partial delivery dispatched                               | Invoice adjusted manually — no audit trail      | System records partial fulfillment → backorder created automatically                 |

---

## 👤 Process Ownership Model

| Process Step             | AS-IS Owner              | Gap                    | TO-BE Owner                           |
| ------------------------ | ------------------------ | ---------------------- | ------------------------------------- |
| Draft order creation     | POS Staff                | No validation          | POS Staff + System check              |
| Stock availability check | Nobody                   | Critical gap           | System (automated)                    |
| Physical picking         | Warehouse Staff          | No system confirmation | Warehouse Staff + Scanner             |
| Inventory deduction      | Nobody (delayed)         | Root cause of variance | System (real-time on dispatch)        |
| Discrepancy reporting    | Nobody                   | Never escalated        | Warehouse Supervisor                  |
| Purchasing decisions     | Buyers (manual estimate) | No reliable data       | Buyers + Live inventory dashboard     |
| Monthly reconciliation   | Accounts team            | Too late to fix        | Eliminated — replaced by cycle counts |

### Accountability Structure (Proposed)

| Role                 | Responsibility                                | KPI Owned                   |
| -------------------- | --------------------------------------------- | --------------------------- |
| Branch Manager       | Overall inventory accuracy                    | Variance % per branch       |
| Warehouse Supervisor | Daily cycle count + discrepancy escalation    | Discrepancy resolution rate |
| POS Lead             | Correct order entry — no unauthorized changes | Order accuracy rate         |
| System/IT Owner      | ERP uptime + integration health               | System availability %       |
| Procurement Manager  | Purchasing based on live data only            | Stockout frequency          |


<img width="2305" height="6478" alt="image" src="https://github.com/user-attachments/assets/ec322b59-542a-4a48-99f8-4651c5d8888f" />
