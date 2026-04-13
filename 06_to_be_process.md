## 7. TO-BE Process — Future State
 
### Redesigned Workflow
 
```
TO-BE: WHOLESALE SALES FLOW (Future — System-Driven State)
 
[CUSTOMER ARRIVES / CONTACTS POS]
       |
       v
[POS STAFF] ---> Enters order in ERP
       |          OK: ERP checks live warehouse stock in real-time
       |
       v
[ERP: LIVE STOCK VALIDATION]
       |
    Sufficient ---> Order confirmed in system
    |               OK: Warehouse receives digital pick request
    |
    Insufficient ---> ERP alerts POS: shortage flag
                      OK: Customer informed immediately
                      OK: Alternative offered (partial / backorder SOP)
       |
       v
[WAREHOUSE RECEIVES DIGITAL PICK LIST]
       |          OK: No paper
       |          OK: System-generated per item, per SKU
       |
       v
[WAREHOUSE STAFF] ---> Scans barcode at pick
       |          OK: Real-time stock deduction on scan
       |          OK: System confirms each item picked
       |
       v
[DISPATCH CONFIRMATION]
       |          OK: ERP closes pick order
       |          OK: Invoice auto-generated
       |          OK: Stock updated in real-time
       |
       v
[CUSTOMER RECEIVES INVOICE — DIGITAL OR POS]
       |          OK: One step — no return trip
       v
[ORDER COMPLETE — SYSTEM FULLY UPDATED]
```

### AS-IS vs. TO-BE Comparison
 
| Dimension | AS-IS | TO-BE |
|-----------|-------|-------|
| Stock check at POS | None — outdated system data | Real-time ERP query |
| Order confirmation | Paper draft | Digital in-system confirmation |
| Warehouse pick instruction | Paper handed by customer | Digital pick list from ERP |
| Barcode scanning | None | Required at every pick |
| Stock deduction timing | End of day (or never) | At point of scan/dispatch |
| Exception handling | Cross out on paper | ERP flag + SOP + supervisor notification |
| Invoice generation | Manual after return trip | Auto-generated on dispatch |
| Customer journey steps | 3 (POS → WH → POS) | 1 (POS only) |
| Inventory accuracy | ~85% | Target >97% |
 
---


 
### TO-BE Process Diagram
 

<img width="2305" height="6478" alt="image" src="https://github.com/user-attachments/assets/ec322b59-542a-4a48-99f8-4651c5d8888f" />
