# Business Requirements

## Overview

The Fashion Store Management System was designed to support the daily operations of a fashion retail business. The system integrates the workflows of multiple departments, including Store Management, Sales, Warehouse, Delivery, and Customer Service, to improve operational efficiency and data consistency.

---

## Stakeholders

| Stakeholder | Responsibilities |
|-------------|------------------|
| Store Manager | Manage products, inventory, promotions, and business performance |
| Sales Staff | Create orders, process payments, generate invoices |
| Warehouse Staff | Manage inventory, goods receipt, stock issuance |
| Delivery Staff | Create delivery orders and monitor shipment status |
| Customer Service Staff | Handle customer inquiries, complaints |
| Customers | Purchase products and receive after-sales services |

---

## Key Business Requirements

### Sales Management

- Create customer orders.
- Process payments using multiple payment methods.
- Generate sales invoices.
- Maintain customer information.
- Support promotional campaigns.

### Inventory Management

- Monitor inventory availability.
- Record stock receipts and stock issues.
- Perform periodic inventory audits.
- Generate inventory reports.

### Delivery Management

- Create delivery orders.
- Coordinate with shipping providers.
- Track delivery status.
- Record delivery performance.

### Customer Service

- Receive customer feedback.
- Process complaints.
- Support product returns and exchanges.
- Maintain customer satisfaction records.

### Store Management

- Manage product information.
- Monitor sales performance.
- Manage promotional programs.
- Review operational reports.

---

## Business Rules

- Product availability must be verified before an order is confirmed.
- Payment must be completed before generating a sales invoice.
- Inventory quantities are updated automatically after stock transactions.
- Returns and exchanges must comply with company policies.
- Promotional campaigns are managed by Store Managers.

---

## Sample Business Processes

### Create Sales Order

**Actor:** Sales Staff

1. Select products.
2. Verify inventory availability.
3. Enter customer information.
4. Confirm order details.
5. Save the order.
6. Forward the order for further processing.

---

### Process Payment

**Actor:** Cashier

1. Retrieve order information.
2. Verify product details and promotions.
3. Select payment method.
4. Confirm payment.
5. Generate invoice.
6. Update payment status.

---

### Handle Customer Complaints

**Actor:** Customer Service Staff

1. Receive customer feedback.
2. Verify order information.
3. Investigate the issue.
4. Coordinate with related departments.
5. Update complaint status.
6. Record the final resolution.