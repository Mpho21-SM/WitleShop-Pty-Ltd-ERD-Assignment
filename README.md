# WitleShop (Pty) Ltd – ERD Assignment

This repository contains my Entity Relationship Diagram (ERD) for the WitleShop (Pty) Ltd online store case study.

## What the System Does

WitleShop is an online store where customers can register, save multiple delivery addresses, browse products (organised by category and linked to suppliers), place orders containing multiple products, make payments, and have their orders delivered.

## Entities

- **Customer** – stores customer account details
- **Address** – a customer's registered delivery addresses (one customer can have many)
- **Category** – groups products (e.g. Electronics, Clothing)
- **Supplier** – companies that supply products to WitleShop
- **Product** – items sold in the store
- **Order** – a customer's order
- **Payment** – payment made for an order
- **Delivery** – delivery details for an order

## Key Relationships

- **Customer → Address (1:M)** – a customer can register many addresses, but each address belongs to one customer.
- **Customer → Order (1:M)** – a customer can place many orders.
- **Order → Payment (1:1)** – each order has exactly one payment.
- **Order → Delivery (1:M)** – an order can have delivery updates/records tied to it.
- **Delivery → Address (1:M)** – a saved address can be used for more than one delivery over time.
- **Category → Product (1:M)** – a category can have many products, but each product belongs to one category.
- **Supplier → Product (1:M)** – a supplier can supply many products, but each product has one supplier.
- **Order ↔ Product (M:N)** – an order can include many products, and a product can appear in many orders. 

## Files in This Repository

- `WitleShop ERD.drawio.png` – the final entity relationship diagram
- `README.md` – this explanation
