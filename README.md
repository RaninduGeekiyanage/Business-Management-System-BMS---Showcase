🏢 Business Management System (Mini ERP) with POS

🚀 A modern, scalable Mini ERP + POS platform built with the TALL Stack for seamless retail & wholesale operations.

<p align="center"> <img src="https://img.shields.io/badge/Laravel-12-red?style=for-the-badge&logo=laravel" /> <img src="https://img.shields.io/badge/Livewire-3-purple?style=for-the-badge&logo=livewire" /> <img src="https://img.shields.io/badge/TailwindCSS-4-38BDF8?style=for-the-badge&logo=tailwindcss" /> <img src="https://img.shields.io/badge/Filament-Admin-orange?style=for-the-badge" /> <img src="https://img.shields.io/badge/MySQL-Database-blue?style=for-the-badge&logo=mysql" /> <img src="https://img.shields.io/badge/Status-Production_Ready-success?style=for-the-badge" /> </p>

✨ Overview

This Business Management System (BMS) is a powerful Semi ERP solution designed for:

🏪 Retail Stores
📦 Wholesale Businesses
🧾 Accounting Operations
🛒 POS-Based Companies
📊 Inventory-Centric Businesses

Built using Laravel 12 + Livewire 3, the system delivers a real-time SPA-like experience without heavy frontend complexity.

It combines:

⚡ Fast POS Transactions
📦 Inventory Management
🧾 Procurement Workflows
💰 Financial Accounting
📊 Reporting & Analytics
🔐 Enterprise-grade RBAC

🧩 Core Modules
┌───────────────────────────────────────────────┐
│              BUSINESS MANAGEMENT SYSTEM       │
├───────────────────────────────────────────────┤
│                                               │
│  🛒 POS & SALES                               │
│  📦 INVENTORY MANAGEMENT                      │
│  🧾 PROCUREMENT                               │
│  💰 ACCOUNTING & GL                           │
│  📊 REPORTING & ANALYTICS                     │
│  👥 USER & ROLE MANAGEMENT                    │
│  🖨️ PRINTING & EXPORTS                        │
│                                               │
└───────────────────────────────────────────────┘

🚀 Features
🛒 POS Operations
✅ Real-time retail sales & refund processing
✅ Multi-payment support
💵 Cash
💳 Cards
📱 Mobile Payments
🧾 Credit Sales
✅ Outstanding collection tracking
✅ Customer advance management
✅ Multiple POS accounts & cash drawers
✅ Thermal receipt printing
✅ PDF invoice generation
✅ Credit note handling

📦 Inventory Management
✅ Live stock movement tracking
✅ Reorder level alerts
✅ Barcode generation & scanning
✅ Serial / batch tracking
✅ Transfer & return tracking
✅ Inventory visibility across:
- Sales
- Purchases
- Returns
- Transfers

🧾 Procurement & Supplier Management
✅ Purchase Requests (PR)
✅ Purchase Orders (PO)
✅ Goods Received Notes (GRN)
✅ Return-to-supplier workflows
✅ Vendor billing management
✅ Supplier invoice tracking
✅ Purchase-related expense management

💰 Financial Accounting
✅ Automatic General Ledger posting
✅ Trial Balance reports
✅ Journal Entries
✅ Audit Trails
✅ Reconciliation workflows
✅ Dual-run accounting architecture
✅ Financial statement generation
✅ Credit note adjustments

💵 Petty Cash & Expenses
✅ Petty cash handling
✅ Expense categorization
✅ Cash drawer movement logs
✅ Audit-ready expense history

📊 Reporting & Analytics
✅ Operational dashboards
✅ Financial summaries
✅ Inventory reports
✅ Sales analytics
✅ Procurement insights
✅ P&L reports
✅ Accountant & manager dashboards

👥 User & Access Control
✅ Role-Based Access Control (RBAC)
✅ Permission-driven modules
✅ Secure finance access
✅ Multi-role system:

| Role          | Access                    |
| ------------- | ------------------------- |
| 🛒 Cashier    | POS Operations            |
| 👨‍💼 Manager | Reports & Monitoring      |
| 👨‍💻 Admin   | Full System Access        |
| 📊 Accountant | GL & Financial Operations |

🖨️ Printing & Exports
✅ Thermal receipt printing
✅ PDF document generation
✅ Excel exports
✅ Barcode printing

🧠 System Workflow

 Customer Purchase
         │
         ▼
 ┌─────────────────┐
 │ POS Transaction │
 └─────────────────┘
         │
         ▼
 ┌─────────────────┐
 │ Inventory Update│
 └─────────────────┘
         │
         ▼
 ┌─────────────────┐
 │ GL Posting      │
 └─────────────────┘
         │
         ▼
 ┌─────────────────┐
 │ Financial Reports│
 └─────────────────┘

 🏗️ Architecture
🔷 High-Level Architecture

┌──────────────────────────────────────────────┐
│               PRESENTATION LAYER             │
│  Livewire Components + Blade Templates       │
└──────────────────────────────────────────────┘
                       │
                       ▼
┌──────────────────────────────────────────────┐
│               APPLICATION LAYER              │
│ Controllers • Services • Business Logic      │
│ Invoice Engine • GL Posting • Printing       │
└──────────────────────────────────────────────┘
                       │
                       ▼
┌──────────────────────────────────────────────┐
│                DOMAIN / DATA LAYER           │
│ Eloquent Models • MySQL • Migrations         │
└──────────────────────────────────────────────┘
                       │
                       ▼
┌──────────────────────────────────────────────┐
│              CROSS CUTTING LAYER             │
│ Sanctum • RBAC • Audit Trail • Security      │
└──────────────────────────────────────────────┘

🧰 Tech Stack
⚙️ Backend
PHP 8.2+
Laravel 12
Laravel Sanctum

🎨 Frontend
Livewire 3
Alpine.js 3
Tailwind CSS 4
Blade Templates

🗄️ Database
MySQL

🛠️ Admin & UI
Filament Admin Panel

📚 Libraries & Packages
| Package                   | Purpose            |
| ------------------------- | ------------------ |
| DomPDF / MPDF             | PDF Generation     |
| ESCPOS                    | Thermal Printing   |
| Maatwebsite Excel         | Excel Exports      |
| Picqer Barcode Generator  | Barcode Printing   |
| Spatie Laravel Permission | RBAC               |
| Laravel Sanctum           | API Authentication |


🔐 Security & Compliance
🔒 Role-Based Access Control (RBAC)
🔒 Secure API authentication via Sanctum
🔒 Financial audit trails
🔒 Transaction reconciliation
🔒 Idempotent GL posting
🔒 Operational-first transaction model

⚡ Key Highlights

| Feature                   | Benefit                         |
| ------------------------- | ------------------------------- |
| ⚡ Livewire SPA Experience | Fast & reactive UI              |
| 🧾 Integrated Accounting  | Automatic GL posting            |
| 📦 Inventory Tracking     | Real-time stock control         |
| 🛒 POS Optimization       | Faster checkout experience      |
| 🔐 RBAC Security          | Enterprise-grade access control |
| 📊 Business Analytics     | Better decision making          |

📈 Project Status

+ Production Ready
+ Live Retail Deployment
+ Multi-Role Operations
+ Financial Reconciliation Enabled
+ POS + Accounting Integrated

🚀 Future Roadmap
🏭 Production Module
🏢 Asset Accounting
📱 Mobile Companion App
☁️ Cloud Multi-Tenant Support
📡 API Integrations

👨‍💻 Development Philosophy

This project follows:

✅ Clean Architecture Principles
✅ Service-Based Business Logic
✅ Transaction-safe workflows
✅ Scalable modular design
✅ Operational-first accounting model

⭐ Summary

A complete Mini ERP + POS ecosystem tailored for growing businesses requiring:

Fast retail operations
Accurate inventory control
Integrated accounting
Procurement workflows
Real-time reporting
Enterprise-grade security

Built for scalability, reliability, and real-world business operations.

