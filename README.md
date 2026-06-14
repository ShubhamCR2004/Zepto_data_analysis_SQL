# Zepto_data_analysis_SQL
# 📊 Zepto SQL Practice  

---

## 📑 Table of Contents  
1. [Overview](#-overview)  
2. [Dataset Structure](#-dataset-structure)  
3. [Key Operations & Queries](#-key-operations--queries)  
4. [Technologies Used](#-technologies-used)  
5. [File Structure](#-file-structure)  
6. [Setup & Usage](#-setup--usage)  
7. [Example Insights](#-example-insights) 

---

## 📌 Overview  
This project contains a series of SQL queries and data analysis steps performed on a **Zepto** product dataset. The goal is to **explore, clean, and analyze** the data to identify valuable business insights such as **top discounts, inventory trends, and revenue projections**.  

The project showcases:  
- **Data exploration** techniques  
- **Data cleaning** best practices  
- **Business-focused analysis** with SQL  

---

## 🗂️ Dataset Structure  

| Column Name              | Description |
|--------------------------|-------------|
| `sku_id`                 | Unique product identifier |
| `category`               | Product category |
| `name`                   | Product name |
| `mrp`                    | Maximum Retail Price |
| `discountPercent`        | Discount percentage |
| `availableQuantity`      | Available stock |
| `discountedSellingPrice` | Price after discount |
| `weightInGms`            | Product weight in grams |
| `outOfStock`             | Stock availability flag |
| `quantity`               | Number of units |

---

## 🔍 Key Operations & Queries  

### **Data Exploration**  
✔ Total rows & sample data  
✔ Null value checks  
✔ Unique product categories  
✔ Stock availability breakdown  
✔ Duplicate product name detection  

### **Data Cleaning**  
✔ Remove invalid prices (₹0)  
✔ Convert **paise → rupees**  
✔ Ensure consistent values  

### **Business Insights**  
📌 **Top 10 Best Discounts** – Highest discount percentage  
📌 **High MRP Out-of-Stock** products  
📌 **Revenue by Category** – Based on available quantity & selling price  
📌 **High MRP, Low Discount** filter  
📌 **Top 5 Categories by Average Discount**  
📌 **Price per Gram** for products above 100g  
📌 Weight classification: **Low, Medium, Bulk**  
📌 **Total Inventory Weight** per category  

---

## 🛠️ Technologies Used  
- **PostgreSQL** – Database  
- **SQL** – Data manipulation & analysis  

---

## 📂 File Structure  
```
📁 Zepto_SQL_Practice
 ├── Zepto_SQL_practice.sql   # SQL script with all queries
 └── README.md                # Project documentation
```

---

## 🚀 Setup & Usage  

1️⃣ Install & start **PostgreSQL**  
2️⃣ Create a database:  
```sql
CREATE DATABASE zepto_analysis;
```
3️⃣ Run the SQL script:  
```sql
\i Zepto_SQL_practice.sql
```
4️⃣ View query outputs in your SQL client.  

---

## 📈 Example Insights  

**Top 5 Categories by Average Discount**  
| Category        | Avg Discount (%) |
|-----------------|------------------|
| Snacks          | 45               |
| Beverages       | 42               |
| Dairy Products  | 40               |
| Household Items | 38               |
| Personal Care   | 37               |

**Inventory Weight Distribution**  
| Category        | Total Weight (kg) |
|-----------------|-------------------|
| Beverages       | 1250              |
| Snacks          | 980               |
| Household Items | 720               |

---
