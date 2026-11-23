# Phase II – Entity Identification

## 1. Introduction
The purpose of entity identification is to identify the main objects in the FAOSTAT agricultural dataset and organize them into related entities for relational database design.

## 2. Identified Entities

### COUNTRY
- country_id (Primary Key)
- country_name

### ITEM
- item_id (Primary Key)
- item_name

### ELEMENT
- element_id (Primary Key)
- element_name

### UNIT
- unit_id (Primary Key)
- unit_name

### YEAR
- year_id (Primary Key)
- year_value

### OBSERVATION
- observation_id (Primary Key)
- country_id (Foreign Key)
- item_id (Foreign Key)
- element_id (Foreign Key)
- unit_id (Foreign Key)
- year_id (Foreign Key)
- value

## 3. Relationships
- One country can have many observations.
- One item can have many observations.
- One element can have many observations.
- One unit can have many observations.
- One year can have many observations.
- Each observation references one country, one item, one element, one unit and one year.

## 4. Conclusion
The identified entities provide a foundation for normalization from UNF to 3NF and for the logical ERD and data dictionary.
