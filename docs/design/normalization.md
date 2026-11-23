# Phase II – Database Normalization

## 1. Unnormalized Form (UNF)

The unnormalized form stores agricultural data in one wide table containing country, agricultural item, element, year, unit and value.

### Example of 1NF

| Area | Item | Element | Year | Unit | Value |
|---|---|---|---|---|---:|
| Rwanda | Maize | Production | 2022 | t | 120000 |
| Rwanda | Beans | Production | 2022 | t | 85000 |
| Rwanda | Maize | Yield | 2023 | kg/ha | 2500 |
| Rwanda | Cassava | Production | 2023 | t | 150000 |

These are illustrative examples and must be replaced with real records from the raw dataset.

### Changes from UNF to 1NF
- Each cell contains a single value.
- Each row represents one agricultural observation.
- No repeating groups are stored in a cell.

### Dependency Removed
Repeating groups are avoided by storing one observation per row. If the raw data already satisfies 1NF, no structural change is necessary at this stage.

### Conclusion
The data can satisfy 1NF when each field contains an atomic value and every observation is stored separately.


### Problems with UNF
- Repeated country names.
- Repeated item names.
- Repeated elements and units.
- Data is stored together in a wide table.
## 3. Second Normal Form (2NF)

Second Normal Form requires a table to be in First Normal Form (1NF) and every non-key attribute to depend on the whole primary key, not only part of a composite key.

### Example of 2NF

| Area | Item | Element | Year | Unit | Value |
|---|---|---|---|---|---:|
| Rwanda | Maize | Production | 2022 | t | 120000 |
| Rwanda | Beans | Production | 2022 | t | 85000 |
| Rwanda | Maize | Yield | 2023 | kg/ha | 2500 |

These are illustrative examples and must be replaced with actual records from the raw dataset.

### Changes from 1NF to 2NF
- The table remains in 1NF.
- The candidate key must be identified and verified.
- Non-key attributes must depend on the entire candidate key.

### Dependency Removed
A partial dependency is removed by separating attributes that depend on only part of a composite key. This split must be demonstrated using the actual dataset and its verified dependencies.

### Conclusion
The dataset is evaluated for partial dependencies to ensure that non-key attributes depend on the whole key. Any required decomposition must be justified using the actual data.
UNF is the starting point for normalization. The data will be reorganized into related tables to reduce repetition and improve data organization.
