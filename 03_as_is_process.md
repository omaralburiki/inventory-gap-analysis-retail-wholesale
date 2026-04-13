## 3. AS-IS Process — Current State
 
### Sales Fulfillment Workflow (Wholesale Branch)
 
```
AS-IS: WHOLESALE SALES FLOW (Current — Broken State)
 
[CUSTOMER ARRIVES]
       |
       v
[POS STAFF] ---> Creates draft order based on system stock
       |          WARNING: System stock may not reflect physical reality
       |
       v
[PAPER DRAFT] ---> Customer receives paper order list
       |
       v
[CUSTOMER WALKS TO WAREHOUSE]   <--- Physical journey: time wasted
       |
       v
[WAREHOUSE STAFF] ---> Manually picks items from shelves
       |          WARNING: No system confirmation
       |          WARNING: No barcode scan
       |
       v
[ITEM SHORTAGE FOUND?]
       |
    Yes --> Warehouse staff CROSSES OUT items on paper
    |       WARNING: No system notification to POS
    |       WARNING: No stock discrepancy flag
    |
    No --> All items available
       |
       v
[CUSTOMER RETURNS TO POS]   <--- Second physical trip
       |
       v
[POS STAFF] ---> Adjusts invoice based on paper from warehouse
       |          WARNING: Manual adjustment -- error-prone
       |
       v
[INVOICE ISSUED]
       |          WARNING: System inventory NOT updated in real-time
       v
[ORDER COMPLETE]
```
 
### AS-IS Process Diagram


[<img width="1543" height="5845" alt="image" src="https://github.com/user-attachments/assets/a7aa55c3-60d4-4ed8-a94b-d85f086453d1" />](https://mermaid.ai/d/86cd628e-cdaa-4c9c-a241-98ddcc9407d9)
