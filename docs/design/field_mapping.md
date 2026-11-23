# Field Mapping – FAOSTAT Agriculture Dataset

## Purpose

This document maps the original FAOSTAT dataset fields to the proposed normalized tables in the AgroMarket database design.

## Proposed Field Mapping

| Original Field / Information | Target Table | Target Column |
|---|---|---|
| Country / Area | COUNTRY | country_name |
| Item | ITEM | item_name |
| Element | ELEMENT | element_name |
| Unit | UNIT | unit_name |
| Year | YEAR | year_value |
| Value | OBSERVATION | value |

## Fields Requiring Verification

The original CSV may contain additional fields such as codes, flags, flag descriptions, notes or other metadata.

These fields must be checked against the actual CSV header and mapped appropriately before the final design is completed.

| Field | Action |
|---|---|
| Country code | Verify and decide whether to retain |
| Item code | Verify and decide whether to retain |
| Element code | Verify and decide whether to retain |
| Flag | Verify and decide whether to retain |
| Flag description | Verify and decide whether to retain |
| Note | Verify and decide whether to retain |
| Other original fields | Map to a table or explain why they are dropped |

## Data Type Conversion Plan

| Field | Planned Data Type Category |
|---|---|
| IDs and codes | Numeric or text, depending on source |
| Country name | Text |
| Item name | Text |
| Element name | Text |
| Unit | Text |
| Year | Integer |
| Value | Numeric |
| Notes and descriptions | Text |

Oracle data types and sizes will be decided in Phase IV.

## Conclusion

This field mapping provides a preliminary guide for organizing the FAOSTAT dataset into related tables. The mapping must be verified against every column in the original raw CSV before the logical design is finalized.
