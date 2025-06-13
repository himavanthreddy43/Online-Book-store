# 📚 Online Book Store - Database Project

This project is a relational database schema designed for an **Online Book Publishing and Sales Platform**. It captures essential entities such as books, editions, authors, publishers, genres, customers, and orders, while supporting features like multiple editions, co-authored books, customer wishlists, and detailed order tracking.

---

## 📘 Project Overview

The **Online Book Store** system aims to model a comprehensive backend database that can:

- Store detailed information about books and their editions
- Track authorship and genres
- Manage customer profiles, shipping addresses, and wishlists
- Record and process customer orders with payment and shipment statuses

---

## 🧱 Entity-Relationship Model (ERD)

The ER schema includes the following major entities and relationships:

- **Books** have multiple **Editions**, associated with one **Publisher**
- **Books** can belong to multiple **Genres**
- **Books** can be co-authored by multiple **Authors**
- **Customers** can have multiple **Shipping Addresses** and maintain a **Wishlist**
- **Orders** are placed by **Customers**, contain multiple **Book Editions**, and include **Order Items** with quantity and discount details

---

## 🛠️ SQL Table Creation

The schema is implemented in SQL using the following tables:

1. `Author` - Stores author info
2. `Publisher` - Stores publisher info
3. `Genre` - Stores genres
4. `Book` - Stores general book data
5. `BookEdition` - Stores edition-specific data like ISBN, price, etc.
6. `BookAuthor` - Maps many-to-many relation between books and authors
7. `BookGenre` - Maps many-to-many relation between books and genres
8. `Customer` - Stores customer data
9. `ShippingAddress` - Stores multiple addresses for customers
10. `Wishlist` - Stores customer's wishlist items
11. `Orders` - Stores customer orders with shipment info
12. `OrderItems` - Stores detailed order contents per edition

---

## 📦 Sample Data Inserts

Sample records have been inserted into each table to demonstrate:

- Books authored by **J.K. Rowling** and **George R.R. Martin**
- Two publishers: **Bloomsbury Publishing** and **Bantam Books**
- Genres like **Fantasy**, **Adventure**, and **Drama**
- Customers with sample orders and wishlist entries

---

## 🧾 Example Order Workflow

A typical order scenario includes:

- A customer selects a book edition (from wishlist or directly)
- Adds it to an order with quantity and optional discount
- Chooses a shipping address
- Completes payment and tracks shipping status

---

## ✅ Features Demonstrated

- Many-to-many relationships (Books ↔ Authors, Books ↔ Genres)
- One-to-many relationships (Customer ↔ Addresses, Book ↔ Editions)
- Detailed order tracking with payment and shipping status
- Support for co-authored books, pre-orders, and multiple editions

---

## 📂 Files Included

- `create_tables.sql` – SQL scripts to create all tables
- `insert_data.sql` – SQL scripts to insert sample data
- `README.md` – Project overview and description (this file)

---
![image](https://github.com/user-attachments/assets/54b13c9c-5bad-488b-ba2a-2cffc4721e9f)



