# 🧾 SAP Order-to-Cash (O2C) — Complete Sales Cycle Implementation

> A SAP SD capstone project showcasing the end-to-end Order-to-Cash business process implemented using SAP ERP.

---

## 👤 Student Details

| Field | Details |
|---|---|
| **Name** | Tanisha Behura |
| **Roll Number** | 2305663 |
| **Programme** | B.Tech |
| **Specialization** | Computer Science and Engineering (CSE) |
| **Course** | SAP Order to Cash |
| **University** | Kalinga Institute of Industrial Technology (KIIT) |

---

## 📌 Introduction

The Order-to-Cash (O2C) process sits at the heart of every customer-facing business operation. It governs the journey from the moment a buyer expresses interest in a product or service, through order confirmation, fulfillment, and invoicing, all the way to the final settlement of payment. This project implements the complete O2C cycle using SAP's Sales & Distribution (SD) and Financial Accounting (FI) modules within a live SAP ERP environment.

Throughout this project, a fictional company called **PixelEdge Technologies Pvt. Ltd.** — an electronics and computer hardware distribution firm — serves as the business entity for all configurations, master data, and transaction demonstrations.

---

## 🧩 Business Problem

Before adopting SAP, PixelEdge Technologies managed its sales operations through a combination of spreadsheets, email threads, and manual approvals. While workable at a small scale, this approach became increasingly unreliable as order volumes grew:

- Sales teams had no real-time view into order status or delivery timelines
- Invoice generation was done manually, leading to frequent billing mismatches
- There was no standardized workflow for approvals, causing processing delays
- Customer master data was scattered across files with no central system of record
- Shipments sometimes went unrecorded, causing gaps in revenue recognition

This project demonstrates how implementing SAP SD's O2C framework resolves each of these pain points through automation, integration, and structured process controls.

---

## 🎯 Objectives

- Understand and configure the complete O2C lifecycle within SAP SD
- Execute each process step using the appropriate SAP transaction codes
- Trace the document flow end-to-end, from Sales Inquiry to Payment Posting
- Demonstrate how SAP SD, MM, and FI modules interact throughout the cycle
- Produce documentation useful for both academic evaluation and real-world reference

---

## 🔧 SAP Modules Involved

| Module | Full Name | Role in O2C |
|---|---|---|
| **SD** | Sales & Distribution | Core module — handles inquiries, orders, delivery, and billing |
| **MM** | Materials Management | Manages inventory levels and confirms goods issue |
| **FI** | Financial Accounting | Posts customer invoices and records incoming payments |

---

## 🔄 End-to-End Workflow

```
[Customer Inquiry Received]
         │
         ▼
 ┌───────────────────┐
 │  Sales Inquiry    │  T-Code: VA11
 │                   │  Customer requests product availability or pricing
 └────────┬──────────┘
          │
          ▼
 ┌───────────────────┐
 │  Sales Quotation  │  T-Code: VA21
 │                   │  Formal quote issued with price, terms, and validity
 └────────┬──────────┘
          │
          ▼
 ┌───────────────────┐
 │  Sales Order (SO) │  T-Code: VA01
 │                   │  Customer confirms; binding order entered in system
 └────────┬──────────┘
          │
          ▼
 ┌───────────────────┐
 │  Delivery         │  T-Code: VL01N
 │  Processing       │  Outbound delivery document created; goods picked
 └────────┬──────────┘
          │
          ▼
 ┌───────────────────┐
 │  Post Goods Issue │  T-Code: VL02N
 │  (PGI)            │  Inventory reduced; legal ownership shifts to buyer
 └────────┬──────────┘
          │
          ▼
 ┌───────────────────┐
 │  Customer Invoice │  T-Code: VF01
 │  (Billing)        │  Billing document raised against delivery
 └────────┬──────────┘
          │
          ▼
 ┌───────────────────┐
 │  Payment Receipt  │  T-Code: F-28
 │                   │  Payment posted; accounts receivable cleared
 └───────────────────┘
```

---

## ✅ Key Highlights

- Full 7-step O2C cycle executed with a realistic business scenario
- All transactions performed against PixelEdge Technologies as the test company
- Document linkage verified across each transaction in the chain
- SD → MM → FI integration clearly demonstrated at relevant steps
- Screenshot evidence captured for every major transaction
- Content written in clear, academic-friendly language

---

## 📋 Transaction Summary

| Step | Activity | T-Code | Module |
|---|---|---|---|
| 1 | Sales Inquiry | VA11 | SD |
| 2 | Sales Quotation | VA21 | SD |
| 3 | Sales Order | VA01 | SD |
| 4 | Delivery Processing | VL01N | SD / MM |
| 5 | Post Goods Issue | VL02N | SD / MM |
| 6 | Customer Billing | VF01 | SD / FI |
| 7 | Payment Receipt | F-28 | FI |

---

## 🖼️ Screenshots Index

All screenshots are saved in `/screenshots/` following the naming convention below:

| File | What It Shows |
|---|---|
| `01_VA11_inquiry_creation.png` | Inquiry created for customer product request |
| `02_VA21_quotation_creation.png` | Quotation with valid pricing and timeline |
| `03_VA01_sales_order.png` | Sales order with line items and schedule lines |
| `04_VL01N_delivery.png` | Outbound delivery document |
| `05_VL02N_pgi.png` | Post Goods Issue confirmation |
| `06_VF01_billing.png` | Customer invoice/billing document |
| `07_F28_payment_receipt.png` | Payment posted against open invoice |
| `08_document_flow.png` | Full document flow chain in SAP |

---

## 📚 What I Learned

- How sales transactions flow through an ERP system from first contact to cash collection
- How to navigate and execute SAP SD transactions using T-codes
- The integration logic between SD, MM, and FI and why it matters operationally
- How document flow in SAP creates an auditable trail from inquiry to payment
- How structured processes in SAP prevent common issues like duplicate invoicing and stock discrepancies

---

## 🚀 Scope for Further Development

- Connect **SAP CRM / S/4HANA Sales** for richer pre-sales and customer lifecycle management
- Enable **Credit Management (FD32)** for automated credit exposure checks during order creation
- Explore **SAP Fiori** for a modern, app-based interface for order and delivery processing
- Build dashboards with **SAP Analytics Cloud** to track O2C KPIs like DSO and order-to-ship time
- Extend the project with **Returns Management** — including return orders and credit memo processing

---

## 📁 Repository Structure

```
SAP-o2c-project/
├── README.md                        ← Project overview (this file)
├── docs/
│   ├── project_overview.md          ← Business context, scope, and company background
│   └── o2c_process.md               ← Step-by-step process walkthrough with T-codes
├── screenshots/                     ← SAP transaction screenshots
│   └── SCREENSHOT_GUIDE.md          ← Naming conventions and capture instructions
└── report/
    └── final_report.md              ← Full academic submission report
```

---

## 🏫 Disclaimer

This project was developed for academic purposes as part of the SAP Order to Cash course at KIIT University. All company names, customer records, and business data used are entirely fictional and bear no resemblance to any real organization.

---

*Submitted by **Tanisha Behura** | Roll No: 2305663 | B.Tech CSE | KIIT University | 2025–26*
