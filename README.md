# 📚 SQL Database Project – Customer Orders System

This project is a comprehensive SQL-based relational database modeling a customer order system. It includes table creation, referential integrity enforcement, data insertion, and several example queries using explicit joins.

---

## 🏗️ Project Structure

The SQL script is organized into several key phases:

### 1. **Initialization**
- Switches to the target database: `dbSQL1`
- Suppresses row count messages with `SET NOCOUNT ON`

### 2. **Cleanup**
- Drops any existing versions of the tables to ensure the script runs from a clean state.

### 3. **Table Creation**
Creates 12 interrelated tables:
- `TCustomers`, `TOrders`, `TOrderProducts`
- `TProducts`, `TProductCategories`, `TStatuses`
- `TVendors`, `TGenders`, `TRaces`
- `TCities`, `TStates`

Each table includes appropriate primary keys and necessary columns.

### 4. **Referential Integrity**
Establishes 12 foreign key relationships to ensure data consistency across the database (e.g., `TOrders` → `TCustomers`, `TProducts` → `TVendors`, etc.).

### 5. **Data Insertion**
Populates all tables with sample data, simulating real-world entries for:
- States, Cities, Genders, Races
- Customers, Vendors, Products
- Orders and Product Orders

### 6. **Explicit Join Queries**
Performs meaningful SQL joins for data analysis, including:
- 🔍 Customer orders and products
- 📦 Products by category and vendor
- 📉 Low inventory products
- 👨 Male customers over 21
- 🗺️ Vendors by customer state

---

## 📊 Sample Output Goals

The example queries are intended to:
- Show how data from multiple tables relate
- Demonstrate mastery of joins, ordering, and filtering
- Highlight data relationships such as customers-to-orders, products-to-vendors, etc.

---

## ⚙️ How to Run

To execute the script:
1. Open SQL Server Management Studio (SSMS) or any SQL client connected to a server with `dbSQL1`.
2. Paste and run the full script.
3. Review the results of each `SELECT` query for verification.

---

## 📝 Notes

- All table and column names use clear, descriptive naming conventions.
- Foreign keys include `ON DELETE CASCADE` where applicable for automated clean-up.
- Dates and sample values are selected for meaningful query outputs.

---

## 🎓 Educational Purpose

This assignment demonstrates proficiency in:
- Relational database design
- SQL DDL (Data Definition Language)
- SQL DML (Data Manipulation Language)
- Writing complex join queries
- Understanding data normalization and integrity

---

## 📄 License

This project is part of a school assignment and is intended for academic use only.
