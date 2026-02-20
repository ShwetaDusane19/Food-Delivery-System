## **Food-Delivery-System**
Food Delivery Database System
​A comprehensive MySQL-based backend project that simulates a three-tier marketplace involving Customers, Restaurants, and Delivery Drivers. This project manages the entire order lifecycle—from browsing menus to final delivery tracking.

### **Tech Stack**
​Database: MySQL (Relational Database Management System)

​Environment: MySQL Workbench & MySQL Shell

​Architecture: Relational Schema (5 Core Tables)

### ​**Database Schema**

​The system is built on five highly normalized tables:
​**​Users​**: Stores profiles for Customers, Drivers, and Admins (including Pune-based sample data).
​​**Restaurants​**: Contains restaurant names, cuisine types (Asian, Italian, Mexican), and ratings.
​​**Menu​**: An itemized catalog linked to restaurants with price and availability status.
​​**Orders​**: The transaction header tracking order status (Placed, Preparing, Out for Delivery, Delivered).
​​**Order_Details​**: The "line items" table that captures quantity and a price snapshot at the time of purchase.
​
### **Key Features**
​​**1. Order Lifecycle Management​**

​The project tracks the movement of an order through various states using UPDATE statements:
​Preparation: Restaurant accepts and prepares the food.
​Assignment: A specific driver (e.g., Rahul Verma) is assigned to a specific order.
​Logistics: The status moves to Out for Delivery and eventually Delivered. 

​​**2. Business Analytics​**

​Using JOIN and GROUP BY operations, the system can generate:
​Total revenue reports by restaurant or cuisine type.
​Top-selling menu item analysis.
​Customer loyalty and spending habits.

### ​**Future Enhancements​**
​Implementing Payment Gateway tracking tables.
​Adding Triggers for automatic stock reduction when an order is placed.
​Creating a Python Wrapper to automate status transitions.
