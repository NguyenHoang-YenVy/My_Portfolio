# Business Requirements

## Overview
This document defines the business requirements for the Management Information System of **Co MayCa**, a fashion retail store. It describes stakeholders, user roles, functional requirements, and business rules to support Sales, Inventory, Delivery, Customer Service, and Store Management.

---

## Stakeholders

| Stakeholder | Responsibilities |
|---|---|
| Store Manager | Manage overall store operations, coordinate departments, and monitor sales, inventory, and staff |
| Sales Department | Advise customers, introduce products, support the purchasing process, and handle sales activities |
| Delivery Management Department | Manage the delivery of products to customers |
| Warehouse Department | Manage warehouse operations, including receiving, issuing, classifying, counting, and storing products |
| Customer Service Department | Handle customer feedback, inquiries, complaints, and after-sales support |
| Customers | Purchase products, receive delivery, and after-sales services |

## User Roles

| User Role | Department |
|---|---|
| Store Manager | Store Management |
| Sales Staff | Sales Department |
| Cashier | Sales Department |
| Delivery Staff | Delivery Management Department |
| Storekeeper | Warehouse Department |
| Warehouse Staff | Warehouse Department |
| Customer Service Staff | Customer Service Department |
---
## Functional Requirements

### Sales Management
- Create customer orders.
- Process payments using multiple payment methods.
- Generate sales invoices.

### Delivery Management
- Create delivery orders.
- Track delivery status.
- Record delivery performance.

### Inventory Management
- Product management.
- Record stock receipts, and stock issues.
- Perform periodic inventory audits.

### Promotion Management
- Create, and manage promotional campaigns.

### Customer Management 
- Manage customer information.
- Handle customer inquiries and complaints.
- Support customer returns and after-sales services.

### Reporting
- Create reports on Sales, Inventory, Promotion effectiveness, and Customer Service quality.
---

## Business Rules
- **QD01:** An invoice can only be generated after order confirmation, and successful payment (if applicable).
- **QD02:** Delivery staff must update the delivery status after completing the shipment.
- **QD03:** Customer complaints, and return requests are accepted within 7 days of product delivery according to the company's return policy.

---
