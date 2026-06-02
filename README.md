

# <p align="center" style="font-size: 55px;"> <b> </b>**Company-Sales-Revenue-Analysis-Using-MongoDB**</p>

<p align="center">
  <b>Insights about Company Sales with Visualizations</b><br>
   <i> 🚀🚀🚀 </i>     
</p>

---

---


## Project Overview

This project focuses on analyzing company sales and revenue data using **MongoDB**, a NoSQL document-oriented database. The system is designed to store, process, and analyze large volumes of business transaction data efficiently. By using MongoDB aggregation pipelines, the project generates valuable business insights such as revenue trends, product performance, customer behavior, and regional sales analysis with the use of visualization tool as Microsoft Power BI.

The primary goal of this project is to demonstrate how MongoDB can be used for real-world business analytics and decision-making processes. The project combines database management, data preprocessing, analytical querying, and visualization techniques to create a complete sales analytics solution.

---

# Objectives

The major objectives of this project are:

- Store company sales data in MongoDB collections.
- Perform data cleaning and preprocessing.
- Analyze revenue, profit, and sales performance.
- Generate business insights using MongoDB aggregation.
- Visualize trends and key performance indicators (KPIs).
- Integrate MongoDB for advanced analysis.

---

# Technologies Used

| Technology | Purpose |
|---|---|
| MongoDB | NoSQL database storage |
| PyMongo | MongoDB-Python connectivity |
| Microsoft Power BI | Visualization |
| Jupyter Notebook | Development environment |

---



# Dataset Description

The dataset used in this project contains company sales transaction records. Each record represents an individual sales order and includes detailed information related to customers, products, pricing, and revenue generation.

## Dataset Fields

| Field Name | Description |
|---|---|
| Order ID | Unique identifier for each order |
| Order Date | Date of transaction |
| Customer Age | Age of customer |
| Customer Gender | Gender of customer |
| Product Category | Category of product |
| Product Name | Product purchased |
| Quantity Sold | Number of units sold |
| Unit Price | Price per unit |
| Unit Cost | Cost per unit |
| Revenue | Total revenue generated |
| Cost | Product cost |
| Product Sub Category | Sub Category of product |
| Region / State | Sales region/location |


---


# System Workflow

The project follows the below workflow:

```text
Dataset Collection
        ↓
Data Cleaning & Preprocessing
        ↓
Import Data into MongoDB
        ↓
MongoDB Aggregation Queries
        ↓
Data Visualization
        ↓
Business Insights & Reporting
```

---

# MongoDB Database Structure

The project uses a MongoDB database named:

```bash
companyDB
```

Main collection:

```bash
sales
```

Example MongoDB document:

```json
{
  "order_id": 101,
  "date": "2025-01-15",
  "customer": "ABC Pvt Ltd",
  "region": "South",
  "product": "Laptop",
  "quantity": 5,
  "unit_price": 50000,
  "revenue": 250000,
  "profit": 40000
}
```

---

# Project Workflow

```text
+----------------------+
|   Sales Dataset      |
| (CSV / Excel / JSON) |
+----------+-----------+
           |
           v
+----------------------+
| Data Cleaning &      |
| Preprocessing        |
+----------+-----------+
           |
           v
+----------------------+
| MongoDB Database     |
|  companyDB           |
|  sales collection    |
+----------+-----------+
           |
           v
+----------------------+
| MongoDB Aggregation  |
| Queries & Analysis   |
+----------+-----------+
           |
           v
+----------------------+
| Data Visualization   |
| (Microsoft Power BI) |
+----------+-----------+
           |
           v
+----------------------+
| Business Insights &  |
| Final Reports        |
+----------------------+
```

---

# Project Architecture

```text
                     +----------------------+
                     |   User / Analyst     |
                     +----------+-----------+
                                |
                                v
                     +----------------------+
                     |MongoDB Compass App.  |
                     |  (Analysis Scripts)  |
                     +----------+-----------+
                                |
                +---------------+---------------+
                |                               |
                v                               v
     +----------------------+       +----------------------+
     |      MongoDB         |       |  Visualization Tools |
     |      companyDB       |       |   Microsoft Power BI |
     |  sales collection    |       +----------------------+
     +----------+-----------+
                |
                v
     +----------------------+
     |   Sales Dataset      |
     | CSV / Excel / JSON   |
     +----------------------+
```

---


# Simple Workflow Explanation

1. The sales dataset is collected in CSV, Excel, or JSON format.
2. Data cleaning and preprocessing are performed to remove errors and missing values.
3. Cleaned data is imported into MongoDB collections.
4. MongoDB aggregation pipelines are used for querying and analysis.
5. Pandas processes and analyzes the retrieved data.
6. Visualization libraries generate charts and reports.
7. Final business insights are obtained from the analysis.


---


# Features of the Project

## Revenue Analysis
- Calculate total revenue generated by the company.
- Analyze monthly and yearly sales growth.
- Identify peak sales periods.

## Product Performance Analysis
- Determine best-selling products.
- Compare product category performance.
- Identify low-performing products.

## Regional Sales Analysis
- Compare revenue across regions.
- Analyze geographical sales distribution.
- Detect high-demand markets.

## Customer Analytics
- Identify top customers.
- Analyze customer purchase patterns.
- Study repeat customer behavior.

## Profitability Analysis
- Compare revenue and profit margins.
- Identify products generating maximum profit.
- Analyze cost efficiency.

---

# MongoDB Aggregation Example

Example query to calculate total revenue by region:

```javascript
db.sales.aggregate([
  {
    $group: {
      _id: "$region",
      totalRevenue: { $sum: "$revenue" }
    }
  }
])
```

---


---

# Data Visualization

Tool: Microsoft Power BI

The project generates graphical reports for easier business interpretation.

Visualizations include:

- Revenue trend charts
- Product performance bar graphs
- Regional sales pie charts
- Profit comparison graphs
- Monthly sales analysis

These visualizations help management understand sales patterns and make strategic business decisions.

---

# Key Performance Indicators (KPIs)

The following KPIs are analyzed:

| KPI | Description |
|---|---|
| Total Revenue | Total company earnings |
| Total Profit | Net business profit |
| Profit Margin | Profit percentage |
| Best-Selling Product | Highest sales product |
| Top Region | Highest revenue region |
| Average Order Value | Average customer spending |

---

# Advantages of Using MongoDB

- Flexible schema structure
- Efficient handling of large datasets
- Fast aggregation operations
- Scalable database architecture
- Easy integration with Python tools

---

# Expected Outcomes

After successful implementation, the project provides:

- Better understanding of company sales trends
- Business decision support through analytics
- Improved revenue tracking
- Product performance insights
- Customer behavior analysis
- Interactive visual reports

---



# Future Enhancements

The project can be further enhanced by adding:

- Real-time analytics dashboard
- Machine learning-based sales prediction
- Customer recommendation system
- Cloud database deployment
- Interactive web application

---

# Conclusion

The **Sales & Revenue Data Analysis Using MongoDB** project demonstrates how NoSQL databases can be effectively used for business intelligence and analytics. By combining MongoDB aggregation capabilities with data analysis and visualization tools, the project delivers meaningful insights from raw sales data.

This project helps organizations improve strategic planning, monitor revenue performance, and optimize sales operations through data-driven decision-making.

---


# Final Note

This project demonstrates the power of combining **MongoDB** with **data analytics techniques** to transform raw business data into meaningful insights. 
By analyzing sales, revenue, customer behavior, and product performance, organizations can make smarter and more strategic business decisions.


✨ Thank you for exploring this project!  
📊 Turning data into valuable business insights.   
💻 Coding with MongoDB & Data Analytics!  
