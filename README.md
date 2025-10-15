# Retail-Data-Modeling-and-Visualization

## Project Overview
This Power BI project aims to analyze product and store performance across a retail network using two structured datasets — **Product Hierarchy** and **Store Cities**.  
Although the datasets are not shared in this repository, the following documentation explains the data model, Power Query transformations, DAX measures, and visualization concepts implemented.

The goal is to create an insightful **Retail Analytics Dashboard** showing trends by product categories, store locations, and sales performance.

---

## Data Model

The project follows a **Star Schema** data structure with two dimension tables and one fact table.

| Table | Role | Key | Description |
|--------|------|-----|-------------|
| `producthierarchy` | Dimension | `product_id` | Contains product details such as brand, size, and category. |
| `store_cities` | Dimension | `store_id` | Contains store information including size, city, and coordinates. |
| `sales_fact` *(simulated)* | Fact | `product_id`, `store_id` | Stores sales transactions with date, quantity, and revenue data. |

