# Related Tables

## 1. Area Table
Stores country or geographical area information.

- Area_ID (Primary Key)
- Area_Code
- Area_Name

## 2. Domain Table
Stores agricultural domain information.

- Domain_ID (Primary Key)
- Domain_Code
- Domain_Name

## 3. Item Table
Stores agricultural product information.

- Item_ID (Primary Key)
- Item_Code
- Item_Name

## 4. Element Table
Stores measurement types.

- Element_ID (Primary Key)
- Element_Code
- Element_Name

## 5. Year Table
Stores reporting years.

- Year_ID (Primary Key)
- Year_Value

## 6. Unit Table
Stores measurement units.

- Unit_ID (Primary Key)
- Unit_Name

## 7. Flag Table
Stores data quality indicators.

- Flag_ID (Primary Key)
- Flag_Code
- Flag_Description

## 8. Observation Table
Stores agricultural statistical records.

- Observation_ID (Primary Key)
- Area_ID (Foreign Key)
- Domain_ID (Foreign Key)
- Item_ID (Foreign Key)
- Element_ID (Foreign Key)
- Year_ID (Foreign Key)
- Unit_ID (Foreign Key)
- Flag_ID (Foreign Key)
- Value

## Relationships

One area, domain, item, element, year, unit, or flag can be associated with many observations.
