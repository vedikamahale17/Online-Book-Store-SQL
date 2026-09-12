# 📚 Online Book Store SQL Analysis

> **PostgreSQL | SQL | Data Analysis | Relational Database | Business Insights**

A practical **SQL data analysis project** built using **PostgreSQL** to manage an Online Book Store database and generate business insights from book, customer, and order data.

The project demonstrates **relational database design, SQL querying, data aggregation, joins, filtering, customer analysis, sales analysis, revenue analysis, and inventory analysis**.

---

## 📌 Project Overview

The **Online Book Store SQL Analysis** project simulates a real-world bookstore database containing three related tables:

* 📖 **Books**
* 👥 **Customers**
* 🛒 **Orders**

The database connects book, customer, and transaction data using **Primary Keys and Foreign Keys**. SQL queries are used to analyze sales performance, customer purchasing behavior, revenue, book pricing, and inventory levels.

---

## 🎯 Project Objectives

* Designed a **relational database structure** for an online bookstore.
* Organized book, customer, and order information into related tables.
* Applied **Primary Key and Foreign Key relationships**.
* Analyzed transactional data using SQL.
* Calculated sales, revenue, and inventory metrics.
* Evaluated customer purchasing behavior.
* Identified frequently ordered and high-value books.
* Applied SQL aggregation, joins, filtering, grouping, and sorting for business analysis.

---

## 🛠️ Tools & Technologies

| Tool / Technology | Purpose                                   |
| ----------------- | ----------------------------------------- |
| **PostgreSQL**    | Relational Database Management System     |
| **SQL**           | Data querying and analysis                |
| **pgAdmin**       | Database development and query execution  |
| **GitHub**        | Project documentation and version control |

---

## 🗄️ Database Schema

### 📖 Books

Stores book and inventory information.

| Column           | Description                     |
| ---------------- | ------------------------------- |
| `Book_ID`        | Unique identifier for each book |
| `Title`          | Book title                      |
| `Author`         | Book author                     |
| `Genre`          | Book genre                      |
| `Published_Year` | Publication year                |
| `Price`          | Book price                      |
| `Stock`          | Available stock                 |

### 👥 Customers

Stores customer information.

| Column        | Description                         |
| ------------- | ----------------------------------- |
| `Customer_ID` | Unique identifier for each customer |
| `Name`        | Customer name                       |
| `Email`       | Customer email                      |
| `Phone`       | Customer phone number               |
| `City`        | Customer city                       |
| `Country`     | Customer country                    |

### 🛒 Orders

Stores customer transaction information.

| Column         | Description                      |
| -------------- | -------------------------------- |
| `Order_ID`     | Unique identifier for each order |
| `Customer_ID`  | Reference to the customer        |
| `Book_ID`      | Reference to the purchased book  |
| `Order_Date`   | Date of the order                |
| `Quantity`     | Number of books ordered          |
| `Total_Amount` | Total order value                |

---

## 🔗 Database Relationships

```text
Customers
    │
    │ Customer_ID
    ▼
 Orders
    │
    │ Book_ID
    ▼
 Books
```

**Relationships:**

* `Customers.Customer_ID` → `Orders.Customer_ID`
* `Books.Book_ID` → `Orders.Book_ID`

---

## 🧠 SQL Skills Demonstrated

### Data Retrieval & Filtering

* `SELECT`
* `WHERE`
* `DISTINCT`
* `BETWEEN`

### Sorting & Limiting

* `ORDER BY`
* `LIMIT`

### Aggregation

* `SUM()`
* `AVG()`
* `COUNT()`

### Relational Analysis

* `INNER JOIN`
* `LEFT JOIN`
* Primary Keys
* Foreign Keys

### Grouped Analysis

* `GROUP BY`
* `HAVING`

### Business Analysis

* Sales Analysis
* Revenue Analysis
* Customer Analysis
* Inventory Analysis
* Product Analysis
* Transaction Analysis

### Other SQL Concepts

* `SERIAL`
* `NUMERIC`
* `COALESCE()`

---

# 📊 Analysis & Business Questions

The project uses SQL to answer practical business questions across **sales, customers, products, revenue, and inventory**.

### 📚 Book Analysis

* **Identified** books within specific genres.
* **Filtered** books based on publication year.
* **Ranked** books by price to identify the most expensive books.
* **Identified** low-stock books.
* **Analyzed** available book genres.
* **Evaluated** average pricing for Fantasy books.

### 🛒 Sales & Order Analysis

* **Calculated** total books sold by genre.
* **Calculated** total books sold by author.
* **Identified** the most frequently ordered book.
* **Analyzed** orders based on quantity and order value.
* **Filtered** transactions within a specific date range.

### 👥 Customer Analysis

* **Identified** customers with at least two orders.
* **Calculated** total customer spending.
* **Determined** the highest-spending customer.
* **Analyzed** customer locations associated with higher-value orders.

### 💰 Revenue Analysis

* **Calculated** total revenue generated from orders.
* **Evaluated** customer spending using aggregated order values.
* **Analyzed** orders exceeding a specified transaction value.

### 📦 Inventory Analysis

* **Calculated** total available stock.
* **Identified** books with the lowest stock levels.
* **Calculated** ordered quantity for each book.
* **Determined** remaining inventory after recorded orders using `LEFT JOIN` and `COALESCE()`.

---

# 🚀 Key Project Results

| Area                     | Result                                                            |
| ------------------------ | ----------------------------------------------------------------- |
| **Sales Performance**    | Calculated books sold by genre and author.                        |
| **Revenue Performance**  | Calculated total order revenue and customer spending.             |
| **Customer Behavior**    | Identified repeat customers and the highest-spending customer.    |
| **Product Performance**  | Identified frequently ordered and high-priced books.              |
| **Inventory Management** | Calculated remaining stock after recorded orders.                 |
| **Pricing Analysis**     | Calculated average Fantasy book price and ranked expensive books. |
| **Order Analysis**       | Evaluated order quantity, order value, and order dates.           |

---

# 💼 Business Value

The analysis demonstrates how SQL can transform transactional database records into **actionable business information**.

The project supports analysis of:

* **Sales performance**
* **Revenue generation**
* **Customer purchasing behavior**
* **Product performance**
* **Inventory levels**
* **Pricing patterns**
* **Order trends**

---

# 📁 Project Structure

```text
Online-Book-Store-SQL/
│
├── OnlineBookStore.sql
└── README.md
```

---

# ▶️ How to Run

### 1️⃣ Create Database

Open **PostgreSQL / pgAdmin** and create a new database.

### 2️⃣ Create Tables

Open:

```text
Online-Book-Store-SQL
```

Execute the table creation queries.

### 3️⃣ Load Data

Load the corresponding book, customer, and order data into their respective tables.

### 4️⃣ Run Analysis

Execute the SQL queries to perform:

```text
Sales Analysis
Customer Analysis
Revenue Analysis
Inventory Analysis
Product Analysis
```

> **Note:** CSV file paths may need to be updated according to your local PostgreSQL/pgAdmin environment.

---

# 📈 Key Skills

**SQL • PostgreSQL • Relational Database Design • Data Analysis • Data Aggregation • SQL Joins • Data Filtering • Data Sorting • GROUP BY • HAVING • Business Analysis • Sales Analysis • Revenue Analysis • Customer Analysis • Inventory Analysis**

---

# 🎓 Learning Outcome

This project strengthened my practical understanding of **SQL, PostgreSQL, relational database concepts, and business-oriented data analysis**.

It provided hands-on experience in:

* Writing SQL queries for business problems
* Working with relational tables
* Applying Primary and Foreign Keys
* Combining data using SQL joins
* Performing aggregate analysis
* Grouping and filtering transactional data
* Analyzing sales and revenue
* Evaluating customer behavior
* Calculating inventory metrics

---

# 👩‍💻 Author

## Vedika Mahale

**Aspiring Data Analyst | Excel | SQL | Power BI**

Interested in:

**Data Analytics • Business Intelligence • Data Visualization • Reporting • Dashboard Development**

---

