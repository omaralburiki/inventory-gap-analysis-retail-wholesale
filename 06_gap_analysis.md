## ❗ Identified Issues

| # | Issue Area           | Description                                   | Estimated Impact                 |
| - | -------------------- | --------------------------------------------- | -------------------------------- |
| 1 | Inventory Accuracy   | Gap between physical stock and system records | 10–20% variance                  |
| 2 | Real-Time Visibility | No live inventory tracking during dispatch    | Unknown shortages until picked   |
| 3 | Manual Entry         | 100% manual data entry — no barcode system    | High human error rate            |
| 4 | System Integration   | POS and Warehouse not connected               | Data silos, delayed updates      |
| 5 | Customer Experience  | Customer walks POS → Warehouse → POS          | Slow, unprofessional fulfillment |
| 6 | Purchasing Decisions | No reliable inventory data for buyers         | Overstock & stockout risk        |
| 7 | SKU Complexity       | Same product, multiple SKUs (multi-origin)    | Miscount, wrong picks, confusion |

---

## 📊 Gap Analysis Table

| # | Process Area            | AS-IS                             | Root Cause                       | Gap Type         | TO-BE                               | Owner                | Impact                      |
| - | ----------------------- | --------------------------------- | -------------------------------- | ---------------- | ----------------------------------- | -------------------- | --------------------------- |
| 1 | Inventory Accuracy      | 15% avg variance                  | No real-time deduction           | System + Process | Auto-deduction on dispatch          | Warehouse Supervisor | Reduce to <3%               |
| 2 | Stock Visibility at POS | Zero visibility                   | POS-WH not integrated            | System           | Live stock check before confirm     | IT/ERP Owner         | Eliminate failed orders     |
| 3 | Data Entry              | 100% manual                       | No barcode infrastructure        | Technology       | Barcode scan at dispatch            | Warehouse Staff      | Reduce errors ~80%          |
| 4 | Process Ownership       | Nobody owns accuracy              | No accountability model          | Governance       | Defined owner per touchpoint        | Branch Manager       | Variance accountability     |
| 5 | Customer Journey        | 3-step physical loop              | No digital confirmation          | Process          | Digital order → warehouse → invoice | POS Lead             | Cut time ~60%               |
| 6 | Exception Handling      | No protocol                       | Process not designed for failure | Process          | Documented SOPs per scenario        | Operations Lead      | Reduce daily firefighting   |
| 7 | SKU Management          | Multi-origin duplicates unmanaged | No SKU governance                | Data             | Normalization + origin attribute    | Procurement          | Clean counts, no mismatches |
| 8 | Purchasing Data         | Based on gut/estimates            | No live inventory feed           | Data + System    | Automated purchasing decisions      | Procurement          | Accurate demand planning    |
