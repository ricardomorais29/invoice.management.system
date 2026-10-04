# invoice.management.system
A full-stack Flask web application for managing clients, tracking financial metrics, and dynamically generating (and emailing) highly formatted PDF invoices with embedded QR codes.

# Velo: Full-Stack Invoice Management Web App

A complete, full-stack web application built in Python and Flask to manage clients, track financial dashboards, and automate the generation of professional PDF invoices.

Initially conceived as a simple script to stop manual billing errors, this project evolved into a fully featured web platform. It handles everything from secure user authentication and relational data management (supporting both SQLite and PostgreSQL) to dynamic PDF rendering and direct email dispatch via SMTP.

## 🚀 Key Features
* **Full-Stack Architecture:** Built on Flask with a flexible database layer that seamlessly switches between local SQLite for development and PostgreSQL for production deployment.
* **Dynamic PDF Rendering:** Uses the `fpdf2` library to programmatically draw highly structured, professional invoices. It automatically calculates line items, VAT (IVA), and total amounts.
* **QR Code Integration:** Automatically generates and embeds a scannable QR code on every invoice containing the core billing data using the `qrcode` library.
* **Direct Email Dispatch:** Integrated `smtplib` allows users to email the generated PDF directly to the client from within the web dashboard using secure SMTP/App Passwords.
* **Financial Dashboard:** Tracks total revenue, outstanding balances, and overall collection rates to provide immediate business insights.

## 🛠️️ Tech Stack
* **Backend:** Python 3.x, Flask
* **Database:** SQLite (Development) / PostgreSQL (Production)
* **Document Generation:** FPDF2
* **Utilities:** `qrcode` (image generation), `hashlib` (password hashing), `smtplib` (email routing)

## ⚙️️ Getting Started

### Prerequisites
Make sure you have Python installed. You will need to install the following dependencies:
```bash
pip install Flask fpdf2 qrcode
