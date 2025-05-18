# Daraz-Database-Management-System

This repository contains SQL scripts for managing the **Daraz E-commerce Platform Database**, covering everything from database schema creation to applying constraints and inserting sample data. It ensures structured, validated, and clean data handling for operations typically required in an online retail system.

---

## Repository Structure

### 1. **Create daraz.sql**
- **Purpose**: Initializes the database schema.
- **Contents**:
  - Creates the `daraz` database.
  - Defines all tables with their respective attributes (e.g., Customers, Users, Products, Orders, Cart, Payments, etc.).
  - Sets up primary keys and foreign key relationships.

---

### 2. **Adding Constraints Daraz.sql**
- **Purpose**: Enforces data integrity rules on the previously created tables.
- **Constraints Applied**:
  - **UNIQUE Constraints**: Ensures no duplicate values for fields like `Email`, `Phone`, and `BrandName`.
  - **DEFAULT Values**: Sets default value of `0` for `Points` in the `Customers` table.
  - **CHECK Constraints**: Ensures valid ranges and non-negative/positive values for:
    - Prices, quantities, points, total amounts, stock, and product ratings.
    - Example: `Rating` must be between `1` and `5`, `TotalAmount > 0`, etc.

---

### 3. **Insert data Daraz.sql**
- **Purpose**: Populates the tables with initial data.
- **Details**:
  - Inserts sample and test data into all key tables.
  - Ensures that all inserted values respect the constraints defined earlier (e.g., no duplicate emails, valid rating ranges, non-zero quantities).

---

## How to Use

1. **Step 1:** Run `Create daraz.sql` to create the database and tables.
2. **Step 2:** Run `Adding Constraints Daraz.sql` to apply constraints for data validation.
3. **Step 3:** Run `Insert data Daraz.sql` to insert valid sample data into the database.

> Make sure to execute these scripts **in order** to avoid constraint violations and ensure database consistency.

---

## Purpose

This project is designed for:
- Learning relational database design.
- Practicing SQL constraint handling.
- Simulating an e-commerce data management system.
- Preparing databases for backend integration.

---

## 🛠 Technologies Used

- **MySQL**
- **SQL DDL & DML**
- **Manual Constraint Management**

---

