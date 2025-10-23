# 📊 Sales Data Analysis

## 🧾 Overview
This project focuses on analyzing sales transactions data.  
The dataset includes product identifiers, sales amounts, cost of goods sold (COGS), quantities, prices, and customer account details.  
It can be used to build dashboards, perform data cleaning, and apply analytical techniques.

---

## 📂 Dataset Structure

| Column Name | Description | Example |
|--------------|-------------|----------|
| **Product_id** | Unique identifier for each product | `2625` |
| **Sales_USD** | Total sales amount in USD | `16156.56` |
| **quantity** | Quantity of items sold | `502` |
| **Price_USD** | Unit selling price in USD | `32.18` |
| **COGS_USD** | Cost of goods sold in USD | `14104.68` |
| **Date_Time** | Date of transaction (DD/MM/YYYY) | `29/03/2024` |
| **Account_id** | Unique customer or account identifier | `1599-E6G-78670` |

---

## 🧮 Data Cleaning Notes
Before performing analysis:
1. Replace commas `,` with dots `.` in numeric columns.
2. Convert numeric columns (`Sales_USD`, `quantity`, `Price_USD`, `COGS_USD`) to float type.
3. Parse `Date_Time` into a proper date format.
4. Standardize separators in `Account_id` (e.g., replace `--` with `-`).
5. Optional: Round quantities to whole numbers if needed.

---

## 🌟 Star Schema Model

**Fact Table:** `FactSales`
- Product_id  
- Account_id  
- Date_Time  
- Sales_USD  
- Quantity  
- Price_USD  
- COGS_USD  

**Dimension Tables:**
- `DimProduct (Product_id, Product_Name, Category, Brand, Supplier, etc.)`
- `DimAccount (Account_id, Customer_Name, Region, Segment, etc.)`
- `DimDate (Date_Time, Year, Month, Quarter, Week, DayName, MonthName)`

---

## 📊 Example Analyses
- Total Sales and Profit over time  
- Profit Margin per Product  
- Monthly or Quarterly Sales Trends  
- Customer or Account performance  
- Price vs. Quantity relationship  

---

## 🧰 Tools Used
- **Excel** → Data cleaning and visualization  
- **Power BI / Tableau** → Dashboard creation  
- **Python / PySpark** → Data processing and analysis  

---

## 🏁 Author
**[Oumayma Abassi]**  
This project was completed as part of a data analysis task involving dataset exploration, cleaning, and schema design.  
