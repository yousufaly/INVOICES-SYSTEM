# INVOICES-SYSTEM
Basic web-based invoice management program

🧾 Invoice Management System - Invoice System

A simple and efficient web-based system for managing invoices and customers, designed to be lightweight and easy to use.

🎯 Key Features

✅ Secure Login – Simple and secure session-based authentication

✅ Customer Management – Add, edit, and delete customers

✅ Invoice Creation – Easy interface with instant total calculation

✅ View & Export PDF – View invoices and download them as PDF

✅ Dashboard – Quick sales statistics overview

✅ Validation – Data validation and integrity checks

✅ Arabic Interface – Fully Arabic user interface

🛠️ Technologies Used
Backend

_ Python 3.x

_ Flask – Web framework

_ SQLAlchemy – ORM for database management

_ SQLite – Local database

_ Frontend

_ HTML5

_ CSS3

_ JavaScript

_ Bootstrap 5 – For styling and responsiveness

PDF
_ WeasyPrint – Convert HTML to PDF

📋 Project Structure

invoice_system/
├── app.py                 # Main entry point
├── config.py              # Configuration settings
├── models/
│   ├── customer.py        # Customer model
│   ├── invoice.py         # Invoice model
│   └── invoice_item.py    # Invoice item model
├── routes/
│   ├── auth.py            # Authentication
│   ├── dashboard.py       # Dashboard
│   ├── customers.py       # Customer management
│   └── invoices.py        # Invoice management
├── templates/             # HTML templates
├── static/                # CSS & JavaScript
├── pdf/                   # PDF generation
└── database.db            # Database file
