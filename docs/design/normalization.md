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

## 4. Third Normal Form (3NF)

Third Normal Form requires a table to be in 2NF and to have no transitive dependencies between non-key attributes.

### Proposed Tables

**COUNTRY**
- country_id (PK)
- country_name

**ITEM**
- item_id (PK)
- item_name

**ELEMENT**
- element_id (PK)
- element_name

**UNIT**
- unit_id (PK)
- unit_name

**YEAR**
- year_id (PK)
- year_value

**OBSERVATION**
- observation_id (PK)
- country_id (FK)
- item_id (FK)
- element_id (FK)
- unit_id (FK)
- year_id (FK)
- value

### Changes from 2NF to 3NF
Repeated descriptive information is separated into related tables. The OBSERVATION table stores foreign keys to the related entities rather than repeatedly storing their descriptive names.

### Dependency Removed
Descriptive information is stored in its own tables, so observation records reference those entities using foreign keys.

### Conclusion
The proposed design separates countries, items, elements, units and years from observations. This design aims to reduce duplication and improve data consistency. The dependencies and fields must be verified against the actual dataset before finalizing the logical design.
