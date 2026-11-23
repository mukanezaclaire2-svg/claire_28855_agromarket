# AgroMarket – Phase II: Data Sourcing, Normalization and Logical Design

## Project Information

- **Project Name:** AgroMarket – Agriculture and Food Marketplace System
- **Student Name:**MUKANEZA Claire
- **Student ID:** 28855
- **Course:** INSY 8311 – Database Development with PL/SQL
- **Phase:** Phase II – Data Sourcing, Normalization and Logical Design
- **Academic Year:** 2026–2027

## Phase Overview

Phase II focuses on sourcing real agricultural data, assessing its quality, identifying entities, normalizing data from Unnormalized Form (UNF) to Third Normal Form (3NF), mapping raw fields to relational tables, and developing the logical Entity Relationship Diagram (ERD) and data dictionary.

This phase provides the logical database design foundation for the future Oracle database implementation of AgroMarket.

## 1. Data Source

The dataset used in this phase was obtained from FAOSTAT, the agricultural statistics database of the Food and Agriculture Organization of the United Nations (FAO).

- **Source:** FAOSTAT
- **Website:** https://www.fao.org/faostat/en/
- **Country:** Rwanda
- **Dataset:** Rwanda Agricultural Statistics
- **Format:** CSV
- **Records:** 597
- **Columns:** 15

The dataset contains agricultural observations for different agricultural items, measurement elements, years and units.

## 2. Dataset Storage

The original dataset is stored in `data/raw/` and preserved unchanged.

The dataset card documenting the source, dataset characteristics, record meaning, and data quality is available at:

`data/dataset_card.md`

## 3. Data Quality Assessment

The dataset was inspected to identify missing values and duplicate records.

| Quality Check | Result |
|---|---:|
| Total records | 597 |
| Total columns | 15 |
| Duplicate rows | 0 |
| Missing values in Value | 12 |
| Missing values in Note | 593 |
| Missing values in other columns | 0 |

The original data has not been cleaned or modified. Data cleaning will be performed during Phase IV.

## 4. Normalization

The dataset will be normalized step by step:

- **UNF:** Identify repeating groups and the original data structure.
- **1NF:** Ensure each field contains a single value and remove repeating groups.
- **2NF:** Remove partial dependencies.
- **3NF:** Remove transitive dependencies.

Each normalization stage will be demonstrated using real dataset records and explanations of the dependencies removed.

The normalization documentation is located in:

`docs/design/normalization.md`

## 5. Field Mapping

Every field from the original dataset will be mapped to its target table and column, or its removal will be justified. Necessary type conversions will also be documented.

Field mapping will be included in the normalization and logical design documentation.

## 6. Logical ERD

The logical Entity Relationship Diagram will illustrate the entities, primary keys, foreign keys, relationships, cardinalities, and optionality using crow's-foot notation.

The ERD will be stored at:

`docs/design/erd.png`

## 7. Data Dictionary

The data dictionary will document each entity and its attributes, meanings, required fields and unique fields, including primary keys and foreign keys.

The data dictionary will be stored at:

`docs/design/data_dictionary.md`

## 8. Project Structure

```text
claire_28855_agroMarket/
│
├── README.md
│
├── data/
│   ├── raw/
│   │   └── FAOSTAT_Rwanda_Agriculture_2022_2024.csv
│   │
│   └── dataset_card.md
│
└── docs/
    └── design/
        ├── normalization.md
        ├── erd.png
        └── data_dictionary.md
```

## 9. Tools Used

- FAOSTAT – Data source.
- GitHub – Version control and project documentation.
- Microsoft Excel – Data inspection and analysis.
- diagrams.net (draw.io) – ERD modeling.

## 10. Conclusion

Phase II provides the foundation for designing a properly structured relational database for AgroMarket. Through data sourcing, data quality assessment, normalization, field mapping, ERD development and data dictionary preparation, the project establishes a logical database design that will be implemented in Oracle Database during the subsequent phase.

## Reference

Food and Agriculture Organization of the United Nations (FAO). FAOSTAT. https://www.fao.org/faostat/en/
