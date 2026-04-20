# Project Overview — SAP Order-to-Cash Implementation

**Student:** Tanisha Behura | Roll No: 2305663 | B.Tech CSE | KIIT University

---

## 1. About This Project

This capstone project documents the end-to-end implementation of the Order-to-Cash (O2C) process using SAP ERP. The project was undertaken as part of the SAP Order to Cash course at Kalinga Institute of Industrial Technology (KIIT), with the goal of applying classroom learning to a realistic, simulated business environment.

The entire cycle — from a customer's initial product inquiry to the final posting of their payment — has been configured and executed within SAP, with each step documented through transaction screenshots, process notes, and this report.

---

## 2. Business Context — PixelEdge Technologies Pvt. Ltd.

To ground the project in a realistic scenario, a fictional company called **PixelEdge Technologies Pvt. Ltd.** has been used throughout all configurations and demonstrations.

### Company Profile

| Attribute | Details |
|---|---|
| **Company Name** | PixelEdge Technologies Pvt. Ltd. |
| **Industry** | Electronics & Computer Hardware Distribution |
| **Headquarters** | Bhubaneswar, Odisha |
| **Operations** | Pan-India B2B distribution of laptops, peripherals, and networking equipment |
| **SAP Company Code** | PETL |
| **Sales Organization** | PE01 |
| **Distribution Channel** | 10 (Standard Distribution) |
| **Division** | 00 (General) |

### Customer Used for Transactions

| Attribute | Details |
|---|---|
| **Customer Name** | TechNova Enterprises |
| **Customer Code** | CUST-1001 |
| **Location** | Hyderabad, Telangana |
| **Account Group** | Domestic Customer |
| **Payment Terms** | Net 30 Days |

### Material (Product) Used

| Attribute | Details |
|---|---|
| **Material Description** | ProBook Laptop 15 (Core i5, 16GB RAM, 512GB SSD) |
| **Material Code** | MAT-PB15 |
| **Material Type** | Finished Goods (FERT) |
| **Unit of Measure** | Each (EA) |
| **Sales Price** | ₹58,000 per unit |

---

## 3. Problem Statement

Prior to SAP adoption, PixelEdge Technologies managed its sales operations through a mix of spreadsheets, email chains, and verbal approvals. As the company expanded its customer base and product catalog, the following challenges became increasingly disruptive:

**Operational Gaps:**
- Sales representatives had no unified system to track order status from placement to delivery
- Billing was handled manually in Excel, resulting in errors, duplicates, and missed invoices
- No automated credit checks meant that high-risk orders were approved without oversight
- Customer data was maintained in separate files by each team, with no master record

**Financial Gaps:**
- Untracked shipments sometimes went unbilled, creating revenue leakage
- Payment collection was not linked to delivery, making reconciliation difficult
- Management had no real-time view of outstanding receivables or revenue performance

**This project demonstrates how SAP's O2C framework directly resolves each of these problems** by replacing manual steps with structured, system-driven workflows that enforce process discipline and generate an auditable trail across every transaction.

---

## 4. Project Scope

This project covers the following in scope:

- Configuration of master data: customer master, material master, pricing conditions
- Execution of all 7 steps of the O2C cycle using standard SAP T-codes
- Verification of document flow linkage across each step
- Demonstration of SD-MM integration at the delivery and goods issue stages
- Demonstration of SD-FI integration at the billing and payment stages
- Screenshot documentation of each key transaction

The following are **out of scope** for this project:

- SAP CRM or pre-sales campaign management
- Advanced credit management configuration (FD32)
- Returns and complaints processing
- SAP S/4HANA-specific Fiori app usage (standard SAP GUI used throughout)

---

## 5. SAP Environment

| Parameter | Value |
|---|---|
| **SAP System** | SAP ERP (ECC 6.0 / S/4HANA sandbox) |
| **Client** | 100 |
| **Interface** | SAP GUI (standard) |
| **Primary Modules** | SD, MM, FI |
| **Language** | English |

---

## 6. Project Deliverables

| Deliverable | Location |
|---|---|
| README — Project summary and workflow | `/README.md` |
| Project Overview (this document) | `/docs/project_overview.md` |
| O2C Process Walkthrough | `/docs/o2c_process.md` |
| Transaction Screenshots | `/screenshots/` |
| Final Academic Report | `/report/final_report.md` |

---

*Tanisha Behura | 2305663 | KIIT University | 2025–26*
