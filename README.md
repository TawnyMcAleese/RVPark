# RV Park Management System

A full-stack reservation and customer management platform for RV park administration. Built as a Capstone project for CS 4760, this ASP.NET Core web application allows customers to reserve RV lots, and manage their stays, while administrators handle lot availability, guest records, and billing.

## Overview

**Key Features**
- Customer dashboard with order history, order tracking
- Admin interface for managing reservations, lots, guests, and fees, employees
- Real-time balance tracking
- Integration with Stripe for secure payments
- Intelligent filtering (e.g., by lot type, availability, guest name)
- Reservation editing and cancellation with financial impact handling

## Technologies Used

- **Frontend**: Razor Pages · Bootstrap · JavaScript (jQuery, DataTables)
- **Backend**: ASP.NET Core · C# · Entity Framework Core
- **Database**: SQL Server with stored procedures and calculated fields
- **Payments**: Stripe API (balance updates, discount handling)
- **Tools**: Visual Studio · GitHub · Stripe CLI

## Screenshots

| Customer Dashboard | Admin Reservation Panel | Lot Management |
|--------------------|--------------------------|----------------|
| ![Customer](screenshots/customer-dashboard.png) | ![Admin](screenshots/admin-reservations.png) | ![Lots](screenshots/lot-management.png) |

## Architecture

- Modular Razor Pages for both Admin and Customer interfaces
- Repository pattern for data abstraction
- Custom service layer for business logic (fees, balances)
- Stripe integration layered via StripeSettings and PaymentModel
- Datatables integration for dynamic record display and filtering

## My Contributions

- **Designed and built the complete admin interface** for managing reservations, RV lots, guest records, and associated fees
- **Implemented the reservation upsert workflow**, allowing for dynamic creation and editing of reservations with real-time financial impact
- **Developed logic for fee calculation and balance tracking**, handling nightly rates, service fees, and automated total computation
- **Built advanced filtering and sorting tools** for admin use, using jQuery and DataTables to manage large datasets efficiently
- **Created reusable Razor components and backend services** to separate logic from presentation and improve maintainability
- **Wrote SQL logic and stored procedures** to support backend operations, including updates to reservation totals and guest data
- - **Created admin reports** for both reservations and financial data, including:
  - Filterable reporting interfaces
  - **PDF and Excel export functionality** for offline tracking and archival

## Lessons Learned

- Learned advanced usage of **Entity Framework** and query optimization
- Integrated **Stripe** into a full-stack .NET environment
- Refined UI/UX through iterative design and admin feedback
- Improved backend layering
- Developed production-level debugging and error handling skills

