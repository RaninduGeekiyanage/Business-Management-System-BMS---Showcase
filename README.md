# Business Management System (Mini ERP) with POS
A modern, scalable Semi ERP with POS system leveraging the TALL stack for seamless retail  &amp; wholesale operations

## Description

This Business Management System (BMS) is designed for retail and wholesale businesses, offering a complete suite of tools for transaction processing, inventory control, procurement, and financial management. Built on Laravel 12 with Livewire components, it ensures a responsive, real-time user experience without page reloads. The system supports multi-role access (Cashier, Manager, Accountant, Admin) and integrates dual-run accounting for operational efficiency and compliance. Key workflows include POS sales/refunds, purchase orders, inventory tracking, and GL posting, making it ideal for growing businesses needing robust, audit-ready operations.

## Features

- POS Operations: Complete sales, refunds, outstanding collections, and customer advances with thermal/PDF printing.
- Procurement Management: Purchase requests, orders, goods received notes (GRN), returns, and expense tracking.
- Inventory Control: Stock movement, reorder alerts, and barcode generation.
- Financial Integration: General Ledger posting with trial balance, journals, and audit trails.
- Reporting & Analytics: Operational reports, GL financial statements, and dashboard widgets.
- User Management: Role-based access control (RBAC) with permissions for secure multi-user environments.
- Printing & Exports: Support for thermal receipts, PDF invoices, and Excel exports.
- Quotations & Proforma: Customer-facing document management.

## Core Functionality
The core revolves around transactional workflows: operational transactions (sales, purchases) are processed first, followed by automatic GL posting for accounting. This ensures business continuity even if accounting steps encounter issues. Modules include POS for front-end sales, back-office procurement for supply chain, inventory for stock oversight, and GL for financial reconciliation.

## Features Showcase
1. POS Sales Interface
Real-time sales processing with item scanning, discount application, and multi-payment methods.

2. Inventory Dashboard
Monitor stock levels, reorder points, and movement history with live updates.

3. Procurement Workflow
End-to-end purchase request to GRN process with approval modes and serial tracking.

4. GL Trial Balance Report
View debit/credit balances across accounts with period-based filtering.

5. Multi-Role Dashboard
Role-specific widgets for stats, latest sales, and reorder alerts.

## Tech Stack

- Backend: PHP 8.2+, Laravel 12 Framework
- Frontend: Livewire 3 (with Flux/Volt), Alpine.js 3, Tailwind CSS 4
- Database: MySQL (via Laravel migrations)
- Admin Panel: Filament (forms, tables, widgets, actions)
- Additional Libraries:
-- DomPDF/MPDF for PDF generation
-- ESCPOS for thermal printing
-- Maatwebsite Excel for exports
-- Picqer PHP Barcode Generator
-- Spatie Laravel Permission for RBAC
-- Laravel Sanctum for API authentication
- Build Tools: Vite, Composer, NPM

## Architecture Diagram

[Presentation Layer]
    Livewire Components (UI/UX)
    Blade Templates

[Application Layer]
    Controllers (API/Export)
    Services (Business Logic: Invoice, Print, GL Posting)

[Domain/Data Layer]
    Eloquent Models
    Database Migrations

[Cross-Cutting]
    Authentication (Sanctum)
    Permissions (Spatie RBAC)
    GL Reconciliation & Idempotency

## Architecture Layers

1. Presentation Layer: Handles user interfaces with Livewire components and Blade views for dynamic, reactive interactions.
2. Application Layer: Manages business logic through controllers and services, including transaction processing and GL hooks.
3. Domain/Data Layer: Core data models and migrations for entities like sales, inventory, and GL accounts.
4. Cross-Cutting Concerns: Security (auth/permissions), reconciliation for accounting integrity, and idempotent posting to prevent duplicates.

## Tech Stack Highlights

- Laravel 12: Latest framework with enhanced performance and security features.
- TALL Stack: Tailwind for styling, Alpine.js for reactivity, Laravel for backend, Livewire for seamless SPA-like experience without JavaScript complexity.
- Filament: Modern admin panel for rapid UI development of forms, tables, and reports.
- Integrated Printing: Supports thermal and PDF outputs for receipts/invoices, crucial for retail environments.
- Scalable Permissions: Fine-grained RBAC ensures secure access across roles.
- Real-Time GL: Post-commit accounting integration allows operational-first workflows with automatic financial tracking.

## Privacy & Security Note
The system employs role-based access control (RBAC) via Spatie Laravel Permission, ensuring users only access authorized features. API endpoints are secured with Laravel Sanctum. GL operations include audit trails and reconciliation snapshots for financial integrity and compliance. All transactions are logged for traceability, and sensitive data is handled per Laravel's security best practices.

## Project Status
Production Ready - Currently in use for live retail operations with comprehensive testing guides and user manuals. Supports POS-first transactions with parallel GL posting, suitable for small to medium businesses expanding to semi-ERP capabilities. Future roadmap includes enhanced production and asset accounting.

