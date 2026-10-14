# Rotoflux India CRM

A dedicated Single-Page CRM and inventory management application designed for **Rotoflux India** to manage Italian imports (Rotoflux SRL), customs clearance, landed cost apportionment, customer purchase orders, sales invoicing, payment tracking, and real-time Profit & Loss (P&L) reporting.

---

## 🚀 Key Features

- **Dashboard**: High-level KPI cards for inventory value, sales revenue, net profit, outstanding & overdue receivables, out-of-stock items, and recent activity.
- **Inventory Master**: Track Rotoflux rotary union codes, thread/flange sizes, mediums (water, hydraulic oil, steam, thermal oil, etc.), passages, HSN codes, unit selling prices, and real-time average landed costs.
- **GRN (Goods Receipt Note — Italy Imports)**: 
  - Manage incoming shipments from Rotoflux SRL, Italy.
  - Automatically calculates foreign exchange conversion (EUR → INR).
  - Net customs duty apportionment (deducts recoverable IGST).
  - Inbound freight, CHA clearance, bank transfer charges, and overhead allocation across line items.
  - Updates physical inventory stock and weighted-average landed cost upon posting.
- **Purchase Orders (POs)**: Record customer orders, track delivery schedules, and convert directly into sales invoices with a single click.
- **Rotoflux India Invoices**:
  - Issue INR sales invoices with customer-specific payment terms and automatic due date calculation.
  - Automatically deducts physical inventory and locks in cost of goods sold (COGS).
  - Outbound customer door delivery/transportation cost accounting.
  - Generates a **Printable GST Tax Invoice** layout (`@media print`) for client billing and PDF generation.
- **Customers & Receivables**: Track customer GSTINs, credit terms, total invoiced/received amounts, aging breakdown (1–30, 31–60, 61–90, 90+ days), and advance balances.
- **Payment Collection**: Record payments against specific invoices, as PO advances, or as unassigned customer advances. Supports partial payments and advance-to-invoice allocations.
- **Profit & Loss (P&L)**: Real-time analytics for gross revenue, landed COGS, delivery expenses, net operating margin, full landed cost breakdown, and monthly trends.
- **CSV Import & Export**: One-click CSV exports for inventory, invoices, receivables, POs, and GRNs. Built-in zero-dependency CSV parser for importing parts and invoice lines.
- **Data Backup & Restore**: Full JSON backup export and restore mechanism with local storage persistence.

---

## 🛠️ Tech Stack

- **Frontend**: Vanilla HTML5, CSS3, Modern JavaScript (ES6+)
- **Design System**: Space Grotesk & Inter typography, Rotoflux industrial color palette, responsive layout
- **Libraries**:
  - [SheetJS (xlsx.full.min.js)](https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js) for Excel reading
  - [PDF.js](https://cdnjs.cloudflare.com/ajax/libs/pdf.js/3.11.174/pdf.min.js) for document parsing
  - Built-in standalone CSV parser fallback (100% offline capable)

---

## 💻 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/abhi08verma-web/CRM.git
   ```
2. Open `index.html` directly in any web browser (Google Chrome, Microsoft Edge, Mozilla Firefox, Safari). No backend server or Node.js environment is required.
