# Simplified E-commerce System

## Overview
This project implements a simplified e-commerce system that supports user management, product ordering, and payment processing. It also includes inventory management for business logic and SQL queries for a bookstore database.

## System Design
- The system comprises several classes, including `User`, `Product`, `Order`, and `Payment`.
- `AdminUser` extends the `User` class to allow for administrative functions.
- A `ShoppingCart` class helps users manage products before placing an order.
- Orders contain products, and each order is associated with a payment.
  
## Business Logic
- The `InventoryManager` class handles stock levels and restocking.
  - The `processOrders()` function checks if products are in stock, reduces stock levels, and triggers restocking alerts if necessary.
  - The `restockItems()` function updates the stock levels based on restocking operations.

## Database Queries
- The SQL queries retrieve insights from a bookstore's database:
  - Top 5 customers by book quantity purchased.
  - Total revenue generated by each author.
  - Books ordered more than 10 times.

## How to Run
1. **Java Code**: 
   - Compile and run the Java code using any Java IDE (e.g., IntelliJ IDEA, Eclipse).
   - Ensure you have a valid list of `Products` and `Orders` for testing.
   
2. **SQL Queries**:
   - Execute the SQL queries on a MySQL database with the specified schema.

## Assumptions
- Products are restocked if their stock level falls below 10 units.
- Users can register and log in, with admins having additional privileges.
- SQL queries are optimized for performance with proper indexing.