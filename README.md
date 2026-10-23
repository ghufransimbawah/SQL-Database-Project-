# SQL-Database-Project-
A database project developed using SQL
# Café Management System ☕[cite: 2]

A database project developed as part of the Database course requirements at Umm Al-Qura University[cite: 2].

## 📌 Project Info
* **University:** Umm Al-Qura University[cite: 2]
* **Instructor:** Dr. Najwa Samarkandi[cite: 2]
* **Team Members:**
  * Ghufran Talal Simbawah (446001992)[cite: 2]
  * Lujain Mohammed Alabdali (446000790)[cite: 2]
  * Fatmah Obaid Alruweys (446000941)[cite: 2]
* **Date:** May 2026[cite: 2]

---

## 📖 Project Description
The Café Management System is designed to manage customers, menu items, and orders in a cafe[cite: 4]. The system stores customer information, menu details, and order records, allowing the cafe to track which customers made orders and which items were ordered[cite: 4].

---

## 🗄️ Database Design
The database `CafeManagementDB` was created to provide a structured environment for managing the cafe's data using MySQL Workbench[cite: 6]. It consists of three main tables[cite: 6]:

1. **`CUSTOMER` Table:**
   * Stores client data[cite: 6].
   * **Attributes:** `Customer_ID` (Primary Key), `Customer_Name`, `Phone_Number` (Unique constraint prevents duplicate phone numbers)[cite: 4, 6].
2. **`ITEM` Table:**
   * Manages menu items[cite: 6].
   * **Attributes:** `Item_ID` (Primary Key), `Item_Name`, `Price` (DECIMAL data type with a `CHECK (Price > 0)` constraint to ensure positive prices)[cite: 4, 6].
3. **`ORDERS` Table:**
   * Records transactions by linking customers to items[cite: 6].
   * **Attributes:** `Order_ID` (Primary Key), `Order_Date` (DATE data type), `Item_ID` (Foreign Key), `Customer_ID` (Foreign Key)[cite: 4, 6].

---

## 🛠️ Constraints & Implementation
* **Primary Keys (PK):** Defined for Customer_ID, Item_ID, and Order_ID to uniquely identify each record[cite: 6].
* **Foreign Keys (FK):** Implemented in the ORDERS table to maintain relationships between customers and items[cite: 6].
* **Data Integrity:** Check and Unique constraints are applied to maintain data accuracy[cite: 6].
* **Sample Data:** Five sample records were inserted into each table for testing and demonstration[cite: 6].

---

## 🔍 SQL Queries & Reports
The project includes advanced SQL queries and reporting mechanisms[cite: 7, 8]:
* **Basic SELECT Queries:** Retrieves specific customer records and menu items based on conditions[cite: 7].
* **Aggregate Functions:** Uses `COUNT` to calculate total orders per customer and `AVG` to find the average menu price[cite: 7].
* **JOIN Operations:** Performs multiple joins between `ORDERS`, `CUSTOMER`, and `ITEM` tables to generate comprehensive reports[cite: 7].
* **Subqueries:** Filters data using nested statements to identify customers who ordered items priced above the overall average menu price[cite: 8].
* **Views:** Creates a virtual table named `Order_Report` to simplify the generation of future sales reports[cite: 8].
