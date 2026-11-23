# Data Dictionary – AgroMarket Phase II

## 1. COUNTRY Table

| Column | Description | Key | Required | Unique |
|---|---|---|---|---|
| country_id | Unique country identifier | PK | Yes | Yes |
| country_name | Name of the country | | Yes | Yes |

## 2. ITEM Table

| Column | Description | Key | Required | Unique |
|---|---|---|---|---|
| item_id | Unique agricultural item identifier | PK | Yes | Yes |
| item_name | Name of agricultural item | | Yes | Yes |

## 3. ELEMENT Table

| Column | Description | Key | Required | Unique |
|---|---|---|---|---|
| element_id | Unique element identifier | PK | Yes | Yes |
| element_name | Name of measurement element | | Yes | Yes |

## 4. UNIT Table

| Column | Description | Key | Required | Unique |
|---|---|---|---|---|
| unit_id | Unique unit identifier | PK | Yes | Yes |
| unit_name | Measurement unit | | Yes | Yes |

## 5. YEAR Table

| Column | Description | Key | Required | Unique |
|---|---|---|---|---|
| year_id | Unique year identifier | PK | Yes | Yes |
| year_value | Statistical year | | Yes | Yes |

## 6. OBSERVATION Table

| Column | Description | Key | Required | Unique |
|---|---|---|---|---|
| observation_id | Unique observation identifier | PK | Yes | Yes |
| country_id | Country reference | FK | Yes | No |
| item_id | Agricultural item reference | FK | Yes | No |
| element_id | Measurement element reference | FK | Yes | No |
| unit_id | Measurement unit reference | FK | Yes | No |
| year_id | Year reference | FK | Yes | No |
| value | Recorded agricultural value | | Depends on source | No |

## Relationships

- COUNTRY to OBSERVATION: One-to-many.
- ITEM to OBSERVATION: One-to-many.
- ELEMENT to OBSERVATION: One-to-many.
- UNIT to OBSERVATION: One-to-many.
- YEAR to OBSERVATION: One-to-many.

## Notes

- PK means Primary Key.
- FK means Foreign Key.
- Required indicates whether the column must contain a value.
- Unique indicates whether a value must be unique in that column.
- The design is preliminary and must be verified against the actual raw CSV.
- Oracle data types and sizes will be added in Phase IV.

## Conclusion

This data dictionary describes the proposed logical database design for AgroMarket's agriculture dataset. It defines the columns, keys, requirements and relationships between tables.
