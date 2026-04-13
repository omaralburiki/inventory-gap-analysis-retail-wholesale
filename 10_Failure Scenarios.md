## 10. Failure Scenarios
 
| Scenario | Trigger | System Response | Manual Fallback |
|----------|---------|----------------|----------------|
| ERP system down | Network / server failure | POS notified — fallback to paper | Paper order → supervisor approval → system entry when restored |
| Scanner failure | Device malfunction | Alert raised via ERP | Manual entry by supervisor only — not staff |
| Stock mismatch at pick | Physical ≠ system count | ERP flags discrepancy → supervisor review | Physical count recorded → variance report → stock adjustment with approval |
| SKU not found in ERP | Item received without matching SKU | Hold order — notify procurement | Procurement creates temp SKU → normalize within 24 hrs |
| POS ↔ WH integration failure | API timeout or sync error | Alert sent to IT and supervisor | Revert to paper for session → IT resolves → backfill system |
| Customer refuses partial order | Shortage at system check | System flags partial unavailability | Offer backorder or substitute via SOP |
 
---
