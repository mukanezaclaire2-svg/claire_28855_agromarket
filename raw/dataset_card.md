# Dataset Card – AgroMarket Phase II

## 1. Dataset Information

- **Dataset Name:** FAOSTAT Rwanda Agriculture Dataset
- **Source:** Food and Agriculture Organization of the United Nations (FAO)
- **Source Website:** https://www.fao.org/faostat/en/
- **Country:** Rwanda
- **Domain:** Crops and livestock products
- **File Format:** CSV (Comma-Separated Values)
- **Original File Name:** FAOSTAT_data_en_11-22-2026 (1).csv
- **Project File Name:** FAOSTAT_Rwanda_Agriculture_2022_2024.csv
- **Collection Date:** 22 November 2026
- **File Size:** 98,815 bytes
- **Number of Records:** 597
- **Number of Columns:** 15

## 2. Source and License

The dataset was obtained from FAOSTAT, the statistical database of the Food and Agriculture Organization of the United Nations (FAO).

Source: https://www.fao.org/faostat/en/

The dataset is used for academic purposes in the AgroMarket database development project. The applicable terms of use and licensing conditions should be checked on the official FAO website.

## 3. What One Record Represents

Each record represents an agricultural statistical observation for a particular agricultural item, element, year, country, and measurement unit.

For example, a record may represent the production of avocados in Rwanda during a particular year, measured in tonnes.

## 4. Dataset Content

The dataset contains agricultural statistics for Rwanda from 2022 to 2024.

It includes:

- 84 agricultural items.
- 8 agricultural measurement elements.
- 3 years: 2022, 2023 and 2024.
- 10 different measurement units.

Examples of agricultural items include avocados, bananas, barley, beans, cabbages, carrots and turnips, cassava and cattle.

The agricultural elements include:

- Area harvested
- Yield
- Production
- Stocks
- Producing Animals/Slaughtered
- Yield/Carcass Weight
- Laying
- Milk Animals

## 5. Data Quality Assessment

The dataset was inspected to identify missing values and duplicate records.

| Quality Check | Result |
|---|---:|
| Total records | 597 |
| Total columns | 15 |
| Duplicate rows | 0 |
| Missing values in Value | 12 |
| Missing values in Note | 593 |
| Missing values in other columns | 0 |

### Observed Data Quality Issues

1. **Missing Value entries:** 12 records have missing values in the Value column.
2. **Missing Note entries:** 593 records have empty Note fields.
3. **Duplicate records:** No duplicate rows were identified during the inspection.
4. **Measurement units:** Different agricultural observations use different units, including ha, kg/ha, t, No, An, 1000 An, No/An, g/An, 1000 No and kg/An.

The dataset has not been cleaned or modified. These issues will be addressed during Phase IV.

## 6. Original Data Preservation

The original CSV file is stored in the `data/raw/` directory and is preserved unchanged.

The raw dataset will serve as the source for data quality analysis, normalization, logical database design and subsequent database implementation.

## 7. Intended Use

The dataset is used for academic purposes in the AgroMarket capstone project to:

- Analyze agricultural data.
- Identify database entities.
- Develop relational tables.
- Demonstrate normalization from UNF to 3NF.
- Develop the logical Entity Relationship Diagram (ERD).
- Prepare the data dictionary and field mapping.

## 8. Reference

Food and Agriculture Organization of the United Nations (FAO). FAOSTAT. https://www.fao.org/faostat/en/
