# AgroMarket – Agriculture and Food Marketplace System

## Project Information

- **Project Name:** AgroMarket
- **Student Name:MUKANEZA Claire
- **Student ID:** 28855
- **Phase:** Phase I – Business Process Modeling
- **Modeling Tool:** diagrams.net (draw.io)

## Project Description

AgroMarket is an Agriculture and Food Marketplace System designed to connect farmers with customers through an online platform. The system aims to make agricultural products easier to find, improve product and stock management, and simplify the ordering process.

The system allows farmers to list their agricultural products, manage prices and quantities, and receive customer orders. Customers can browse products, check availability, and place orders.

## Phase I – Business Process Modeling

### 1. Business Process Definition

**Business Process:** Agricultural Product Ordering and Stock Management.

This process connects farmers with customers through the AgroMarket system. It allows farmers to manage agricultural product listings and stock while customers browse products and place orders.

The process aims to improve agricultural product accessibility, simplify order management, maintain accurate stock records, and improve communication between farmers and customers.

The expected outcome is a successfully recorded order, communicated to the farmer, and properly reflected in the stock records.

### 2. Actors and Responsibilities

| Actor | Responsibility |
|---|---|
| Farmer | Adds products, sets prices and quantities, updates product information, and manages customer orders. |
| Customer | Browses agricultural products, checks availability, selects products, and places orders. |
| AgroMarket System | Stores product and order records, checks stock availability, records orders, and updates stock and order status. |
| Administrator | Manages users, monitors activities, and supervises system information. |

### 3. Business Process Model

The business process is modeled using a UML Activity Diagram with swimlanes to show the responsibilities of the customer, AgroMarket system, and farmer.

The diagram includes:
- Start and end events.
- Activities and tasks.
- Decision points and alternative paths.
- Actors in swimlanes.
- Sequence and information flows.
- Activities that interact with database records.

**Modeling Tool:** diagrams.net (draw.io)

**Published Diagram Link:** [Insert your published diagram link here]

### 4. Data-Generating Activities (CRUD)

| Activity | Operation | Information |
|---|---|---|
| Register customer or farmer | Create | User details and contact information |
| Add agricultural product | Create | Product name, price, quantity and description |
| Browse products | Retrieve | Product information and availability |
| Check stock | Retrieve | Available and requested quantities |
| Place an order | Create | Order ID, customer, product, quantity and date |
| Update product details | Update | Product price, description and quantity |
| Update order status | Update | Order status and processing information |
| Update stock | Update | Remaining product quantity |
| Remove discontinued product | Delete/Archive | Product record or archived product details |

## Documents

The Phase I documentation is organized in the following structure:

```text
AgroMarket/
├── README.md
└── docs/
    └── business_process/
        ├── business_process_diagram.pdf
        └── business_process_explanation.pdf
```

## Tools Used

- diagrams.net (draw.io) – Business process modeling.
- GitHub – Project documentation and version control.

## Conclusion

The Agricultural Product Ordering and Stock Management process provides a structured way to manage agricultural product listings, customer orders, and stock information. The process supports better communication between farmers and customers, improves operational efficiency, and provides a foundation for the future database and system development of AgroMarket.