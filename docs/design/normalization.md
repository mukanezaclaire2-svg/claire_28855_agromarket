# Phase II – Database Normalization

## 1. Unnormalized Form (UNF)

The unnormalized form stores agricultural data in one wide table containing country, agricultural item, element, year, unit and value.

### Example of UNF

| Area | Item | Element | Year | Unit | Value |
|---|---|---|---|---|---:|
| Rwanda | Maize | Production | 2022 | t | 120000 |
| Rwanda | Beans | Production | 2022 | t | 85000 |
| Rwanda | Maize | Yield | 2023 | kg/ha | 2500 |
| Rwanda | Cassava | Production | 2023 | t | 150000 |

These are illustrative examples and must be replaced with actual records from the raw dataset.

### Problems with UNF
- Repeated country names.
- Repeated item names.
- Repeated elements and units.
- Data is stored together in a wide table.

### Conclusion
UNF is the starting point for normalization. The data will be reorganized into related tables to reduce repetition and improve data organization.
