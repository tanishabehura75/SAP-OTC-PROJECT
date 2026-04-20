# Screenshot Guide — SAP O2C Project

**Student:** Tanisha Behura | Roll No: 2305663 | KIIT University

---

## Purpose

This guide defines the naming conventions, capture requirements, and quality standards for all SAP transaction screenshots included in this project. Consistent, well-labeled screenshots are essential for demonstrating that each step of the O2C cycle was actually executed in SAP.

---

## Naming Convention

All screenshots follow this format:

```
[step-number]_[tcode]_[description].png
```

**Examples:**
- `01_VA11_inquiry_creation.png`
- `05_VL02N_pgi.png`
- `08_document_flow.png`

---

## Required Screenshots

| # | File Name | T-Code | What to Capture |
|---|---|---|---|
| 01 | `01_VA11_inquiry_creation.png` | VA11 | Inquiry creation screen with customer, material, quantity, and validity date filled in. Include the system-generated Inquiry Number visible on screen. |
| 02 | `02_VA21_quotation_creation.png` | VA21 | Quotation screen showing pricing conditions, validity period, and the net value. Reference to the source inquiry should be visible. |
| 03 | `03_VA01_sales_order.png` | VA01 | Sales order overview screen with customer, material, quantity, confirmed delivery date, and total order value. Schedule line confirmation preferred. |
| 04 | `04_VL01N_delivery.png` | VL01N | Outbound delivery document with picking quantity confirmed. Delivery document number visible. |
| 05 | `05_VL02N_pgi.png` | VL02N | Delivery document after Post Goods Issue execution. Status should show "Goods Issue Posted" and the GI date should be visible. |
| 06 | `06_VF01_billing.png` | VF01 | Billing document (invoice) with line items, base price, tax amount, and total invoice value. Billing document number visible. |
| 07 | `07_F28_payment_receipt.png` | F-28 | Incoming payment posting screen showing the amount received, customer account, and cleared invoice reference. Payment document number visible on confirmation. |
| 08 | `08_document_flow.png` | VA03 | Full document flow chain accessed via `Environment → Document Flow` from the Sales Order. All documents in the chain should show "Completed" status. |

---

## Capture Standards

- **Resolution:** Minimum 1280×720. Full HD (1920×1080) preferred.
- **Format:** PNG (not JPG — avoids compression artifacts on text)
- **Content:** Always capture the full SAP window including the title bar and transaction code visible in the command field
- **Sensitive Data:** No real personal or financial data should appear. All data used is fictional (PixelEdge Technologies scenario)
- **Annotations:** Optional — you may add red boxes or arrows to highlight key fields, but this is not required

---

## Tips for Good Screenshots

1. Before capturing, verify that the document number is visible on screen — this confirms the transaction was saved successfully
2. For the document flow screenshot, expand all nodes so the complete chain is visible
3. If a screen has scrollable content, consider taking two screenshots (top and bottom) rather than missing key fields
4. Rename screenshots immediately after capture to match the naming convention above

---

*Tanisha Behura | 2305663 | KIIT University | 2025–26*
