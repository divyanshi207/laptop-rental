# Salesforce CRM Laptop Rental Management System

## Project Overview
The Salesforce CRM Laptop Rental Management System is designed to streamline the rental operations of laptops by integrating key business processes such as managing inventory, rental transactions, customers, and payments using Salesforce CRM. This project leverages custom objects, automations, and reporting capabilities to provide a complete solution for laptop rental management.

## Features
- **Laptop Inventory Management**: Track available laptops and manage stock.
- **Customer Management**: Maintain records of customers and rental history.
- **Rental Transactions**: Handle laptop rental transactions with start/end dates and total prices.
- **Payment Tracking**: Manage payments and track due or completed transactions.
- **Maintenance Tracking**: Monitor laptops under maintenance.
- **Custom Reports & Dashboards**: Get insights on inventory, revenue, and rental statistics.

## Custom Objects Used
1. **Laptops**
2. **Customers**
3. **Rental Transactions**
4. **Payments**

## Prerequisites
- A Salesforce Developer Account.
- Basic understanding of Salesforce CRM.

## Setup Guide

### Step 1: Setting Up the Salesforce Environment
1. **Create a Salesforce Developer Account**: Sign up at [Salesforce Developer Signup](https://developer.salesforce.com/signup).
2. **Log in and Access Salesforce Setup**: Click the gear icon in the top-right corner to access the Setup menu.

### Step 2: Creating Custom Objects
1. **Laptops Object**:
   - **Label**: Laptop
   - **Plural Label**: Laptops
   - **Fields**: Model Name, Brand, Specifications, Status, Price per Day

2. **Customers Object**:
   - **Label**: Customer
   - **Fields**: Full Name, Email, Phone Number

3. **Rental Transactions Object**:
   - **Label**: Rental Transaction
   - **Fields**: Customer, Laptop, Rental Start Date, Rental End Date, Total Price

4. **Payments Object**:
   - **Label**: Payment
   - **Fields**: Rental Transaction, Payment Date, Amount Paid, Payment Method

### Step 3: Setting Up Relationships
Create **Lookup Relationships** between the following:
- **Customers ↔ Rental Transactions**
- **Laptops ↔ Rental Transactions**
- **Rental Transactions ↔ Payments**

### Step 4: Creating Automations
1. **Rental Status Automation**: Update the status of laptops based on rental start/end dates.
2. **Payment Reminder Workflow**: Send an email reminder for upcoming due payments.

### Step 5: Setting Up Profiles & Permission Sets
1. Assign object permissions for **Laptops, Customers, Rentals, and Payments**.
2. Use **Profiles** or **Permission Sets** to control CRUD permissions.

### Step 6: Creating Reports and Dashboards
Create custom reports for:
1. Rental History
2. Payments and Revenue
3. Laptops in Maintenance
4. Overdue Rentals

## Deployment
1. **Test the system** thoroughly in a Sandbox environment.
2. **Deploy to Production** using Change Sets or other migration tools.
3. **Train users** on how to use the system.

## Future Enhancements
- Implement a **Mobile App** for on-the-go management.
- Add **Automated Invoice Generation**.
- Build **Custom UI** components using Lightning Web Components (LWC).


