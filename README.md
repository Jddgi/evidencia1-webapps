# evidencia1-webapps
Evidéncia 1

Halcón - Order Tracking and Internal Management Web Application

Overview

Halcón is a web-based management platform built to automate and streamline internal processes for a construction materials distributor. The application features a public tracking interface for customers and an administrative dashboard for staff members across various operational departments.

Key Features

1. Public Customer Portal

Order Status Lookup: Customers can check their order status on the landing page by entering their Customer Number and Invoice Number.

Order Statuses:

Ordered: Order has been registered by a Sales Executive.

In process: Order is being prepared in the warehouse or materials are being acquired via Purchasing.

In route: Materials are loaded and out for delivery.

Delivered: Materials have been successfully delivered to the customer site.

2. Administrative Dashboard & Role Management

Default Admin User: Includes a default Super Admin account with permissions to create new staff accounts and assign roles.

Role-Based Access Control:

Sales: Creates orders and registers customer billing details.

Purchasing: Handles external material purchases when stock is insufficient.

Warehouse: Manages stock levels, prepares order packages, and updates order status to "In process" and "In route".

Route: Oversees distribution, uploads proof of loading/unloading photos, and marks orders as "Delivered".

3. Order Lifecycle & Evidence Management

Order Creation: Registers consecutive invoice number, customer name/company name, unique customer number, fiscal details, date/time, delivery address, notes, and assigns initial status Ordered.

Order Processing: Warehouse picks materials or coordinates with Purchasing. Updates status to In process.

Dispatch & Routing: Materials loaded. Status updated to In route. Route personnel must take and upload a photo of the loaded transport vehicle.

Delivery Evidence (Route): Operator uploads a photo of the unloaded material upon delivery and updates status to Delivered.

4. Advanced Order Management

Search & Filters: Search orders by Invoice Number, Customer Number, Date, or Status.

Soft Deletes: Orders are soft-deleted rather than permanently removed from the database.

Recycle Bin / Soft Delete Management: Dedicated view to list, edit, or restore logically deleted orders.

System Architecture & Technologies

Framework: Laravel (PHP)

Template Engine: Blade Engine

Database: MySQL / PostgreSQL 

Authentication: Laravel Auth / Role Middleware
