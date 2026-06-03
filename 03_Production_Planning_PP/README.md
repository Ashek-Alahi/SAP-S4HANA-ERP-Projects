## SAP Production Planning (PP) – Production Control System

This project demonstrates a complete end-to-end production control 
workflow implemented in SAP ERP using the Global Bike Inc. (GBI) 
training dataset.

### Product
**Women's Off Road Bike (ORWN1148)** | Plant: DL00 (Dallas) | Type: FERT (Finished Product)

### Process Flow Implemented

| Step | Transaction | Description |
|------|-------------|-------------|
| 1 | MM02 | Material Master configuration (MRP 1–4, Work Scheduling) |
| 2 | CS03 | Multilevel BOM — 6 level-1 components, wheel assembly sub-BOM |
| 3 | CA03 | Routing — 11 operations (ASSY1000 work center) |
| 4 | MD61 | Planned Independent Requirements (Jul 2024 – Mar 2025) |
| 5 | MD02 | MRP Run — Single-item, multi-level (Processing key: NETCH) |
| 6 | MD04 | Stock/Requirements List verification |
| 7 | MIGO | Goods Receipt for raw materials (Off Road Tire: 1,700 EA) |
| 8 | CO01/CO02 | Production Order creation and release |
| 9 | MIGO | Goods Issue against Production Order 1000231 |
| 10 | CO11N | Production Order Confirmation (Yield: 80 EA) |
| 11 | MIGO | Goods Receipt for finished goods (80 EA → FG00) |

### Key Configuration
- **Planning Strategy:** 40 (Make-to-Stock with PIR consumption)
- **MRP Type:** M1 | **Lot Size:** EX (Exact)
- **In-house Production Time:** 4 days
- **Forward Consumption Period:** 30 days

### MRP Run Results
- Materials planned: 11 | Planned orders created: 40
- Dependent requirements created: 60 | Runtime: 1 second

### Final Stock Position
| Stage | Before | After Production |
|-------|--------|-----------------|
| Finished Goods (ORWN1148) | 70 EA | 150 EA |

### Team
| Name | Student ID |
|------|-----------|
| Alahi Ashek | M23W0308 |
| Akter Sarmin | M22W7165 |
| Khanam Tahmina | M22W7349 |
