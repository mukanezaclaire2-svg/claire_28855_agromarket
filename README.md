# AgroMarket – Agriculture and Food Marketplace System

## 1. Project Information

- **Project Title:** AgroMarket – Agriculture and Food Marketplace System
- **Student Name:** Claire
- **Student ID:** 28855
- **Project Category:** Agriculture and Food Technology
- **Project Phase:** Phase 0 – Project Planning

## 2. Problem Statement

Many farmers face difficulties accessing markets and finding customers for their agricultural products. This can lead to food waste and reduced income. Customers also experience difficulties finding fresh agricultural products at affordable prices.

## 3. Project Objectives

### General Objective
To develop an agricultural marketplace system that connects farmers with customers and improves the buying and selling of agricultural products.

### Specific Objectives
- To register and manage farmers and customers.
- To allow farmers to add and manage agricultural products.
- To display available agricultural products and their prices.
- To allow customers to place orders.
- To manage customer orders and sales.
- To improve market access and reduce food waste.

## 4. Data Sources

**FAOSTAT – Food and Agriculture Organization**

Website: https://www.fao.org/faostat/en/

FAOSTAT provides agricultural statistics and information about crop production, food supply, livestock, and food availability. These data will support the agricultural information used in the project.

## 5. Planned Innovation

AgroMarket introduces a digital marketplace that connects farmers directly with customers. Farmers will advertise their products, update prices and availability, and receive customer orders. Customers will easily find and order fresh agricultural products online.

## 6. Planned Database Tables

The system will use Oracle Database to store and manage information.

| Table Name | Description |
|---|---|
| FARMERS | Stores farmer information. |
| CUSTOMERS | Stores customer information. |
| CATEGORIES | Stores agricultural product categories. |
| PRODUCTS | Stores product names, prices, quantities and descriptions. |
| ORDERS | Stores customer order information. |
| ORDER_DETAILS | Stores products included in each order. |
| PAYMENTS | Stores payment records and status. |

## 7. Planned PL/SQL Features

The project will use Oracle PL/SQL to manage database operations.

- **Procedures:** Register farmers, register customers, add products, and manage orders.
- **Functions:** Calculate order totals and check product availability.
- **Triggers:** Automatically update product quantities after confirmed orders.
- **Cursors:** Retrieve and display product and order information.
- **Records:** Organize and process farmer, customer, and product information.
- **Collections:** Manage multiple products and order details.
- **Exception Handling:** Handle errors such as insufficient stock and invalid customer orders.
- **Sequences:** Automatically generate unique IDs.
- **Packages:** Organize related procedures and functions.

## 8. Technologies to Be Used

- **Frontend:** HTML, CSS, JavaScript.
- **Backend:** PHP.
- **Database:** Oracle Database 21c Express Edition (XE).
- **Database Programming:** Oracle PL/SQL.
- **Database Development Tool:** Oracle SQL Developer.
- **Code Editor:** Visual Studio Code.
- **Version Control:** Git and GitHub.

## 9. Expected Outcomes

- Improved market access for farmers.
- Easier access to fresh food products.
- Reduced agricultural food waste.
- Better management of agricultural products and orders.
- Improved communication between farmers and customers.

## 10. References

1. Food and Agriculture Organization (FAO). FAOSTAT. https://www.fao.org/faostat/en/
2. Oracle. Oracle Database Documentation. https://docs.oracle.com/en/database/
3. Oracle. PL/SQL Language Reference. https://docs.oracle.com/en/database/oracle/oracle-database/21/lnpls/

## 11. Conclusion

AgroMarket aims to improve agricultural marketing through technology. By connecting farmers directly with customers, the system will support farmers, improve access to food products, and contribute to reducing food waste.

---

**Project Name:** AgroMarket  
**Student:** Claire  
**Student ID:** 28855  
**Repository:** claire_28855_agroMarket  
**Visibility:** Public
