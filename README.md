# INVOICES-SYSTEM
### Basic web-based invoice management program

## 🧾 Invoice Management System - Invoice System

### A simple and efficient web-based system for managing invoices and customers, designed to be lightweight and easy to use.

## 🎯 Key Features :

  ✅ Secure Login – Simple and secure session-based authentication

  ✅ Customer Management – Add, edit, and delete customers

  ✅ Invoice Creation – Easy interface with instant total calculation

  ✅ View & Export PDF – View invoices and download them as PDF

  ✅ Dashboard – Quick sales statistics overview

  ✅ Validation – Data validation and integrity checks

  ✅ Arabic Interface – Fully Arabic user interface

## 🛠️ Technologies Used

```
BACK-END

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
```


## 📋 Project Structure

```
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
```

## 🚀 Quick Start
### 1. Installation

```
BASH

# Clone or copy the project
cd INVOICES_SYS

# Install dependencies
pip install -r requirements.txt
```

### 2. Run the Application

```
BASH

python app.py
```


### Then open your browser at:

```
http://localhost:5000
```

### 3. Login
### Default Password: admin123


## 📊 Database
### Tables
### 1. Customers

```
- id: Unique identifier
- name: Customer name (required)
- phone: Phone number
- email: Email address
- address: Address
- created_at: Creation date
```

### 2. Invoices

```
- id: Unique identifier
- invoice_number: Unique invoice number
- customer_id: Customer ID (relationship)
- date: Invoice date
- currency: Currency
- subtotal: Subtotal amount
- total: Final total amount
- created_at: Creation date
```

### 3. InvoiceItems

```
- id: Unique identifier
- invoice_id: Invoice ID (relationship)
- item_name: Item name
- quantity: Quantity
- price: Price
- total: Total (quantity × price)
```

## 🔄 Workflow
### 1. Login

```
login_required → session → protected routes
```

### 2. Dashboard

### Displays quick statistics:

### - Total invoices

### - Total sales

### - Today’s invoices

### - Today’s sales

### 3. Customer Management

```
View → Add → Edit → Delete
```

### 4. Create Invoice

```
Select customer → Add items → Calculate total → Save
```

### 5. View Invoice

```
Read-only view → Download PDF → Print
```


## 🔐 Security

### - Secure session management

### - Authentication required for protected routes

### - XSS data sanitization

### - SQL Injection protection via SQLAlchemy ORM


## 📝 Validation
## Customers

### - Name is required (2–255 characters)

### - Valid email format

### - Valid phone format


## Invoices

### - Customer is required

### - At least one item required

### - Quantity > 0

### - Price ≥ 0


## 🎨 Interface

### - Responsive Design – Works on mobile and desktop

### - Dark Sidebar – Modern design

### - Arabic Support – Full RTL support

### - Bootstrap 5 – Professional styling


## 📦 Main Dependencies

```
Flask==2.3.2
Flask-SQLAlchemy==3.0.5
WeasyPrint==68.0
Werkzeug==2.3.6
```


## ⚙️ Configuration

In config.py:

```
DEBUG = True              # Development mode
SECRET_KEY = '...'        # Session security key
DATABASE = 'database.db'  # Database file
```


## 🔮 Future Improvements

 ### - Multi-currency support
 
 ### - Advanced reports
 
 ### - Multi-user support
 
 ### - Roles & permissions system
 
 ### - Automatic backups
 
 ### - API for external applications
 
 ### - SaaS conversion


## 🐛 Troubleshooting
###No Customers Found

```
Solution: Add a customer first before creating an invoice.
```

## PDF Error

```
Make sure WeasyPrint and all required dependencies are installed.
```

## Missing Database

```
It will be created automatically when running the application for the first time.
```


## 📞 Support

### For help and inquiries, review the following files:

### - config.py – Configuration

### - models/ – Data structure

### - routes/ – Business logic


## 📄 License

### This project is available for free use.








































