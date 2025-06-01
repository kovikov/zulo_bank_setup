# zulo_bank_setup
# 🏦 Zulo Bank Data Warehouse Project

This project is a comprehensive end-to-end data engineering pipeline designed for a fictional financial institution, **Zulo Bank**. It demonstrates how to clean and normalize raw banking data, design a dimensional model, and load structured tables into a relational database management system for analytical and reporting purposes.

---

## 📌 Objectives

- Transform raw transactional and account data to adhere to database normalization rules (1NF → 2NF → 3NF)
- Construct a robust **date dimension table**
- Design a scalable **Data Warehouse schema**
- Load the final fact and dimension tables into a **PostgreSQL** database using `psycopg2`

---

## 📁 Key Components

| Component | Description |
|----------|-------------|
| `Customer` Table | Extracted from full names and contact info |
| `Account` Table | Normalized with `OpeningDate_ID` foreign key |
| `Transaction` Table | Split by type and linked with `date_dim` |
| `Loan` Table | Cleaned and mapped with interest & time dimensions |
| `Date Dimension` | Fully normalized time-based dimension |
| `Data Warehouse Schema` | Prepared using SQL DDL via psycopg2 |

---

## 🛠 Technologies Used

- **Python** (Pandas, NumPy, psycopg2)
- **PostgreSQL** (Relational Database)
- **Jupyter Notebook**
- **Database Normalization (1NF, 2NF, 3NF)**
- **ETL Principles**

---

## 🚀 How to Use

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/zulo_bank_dw.git
cd zulo_bank_dw
```

### 2. Install Dependencies
```bash
pip install pandas psycopg2-binary
```

### 3. Run the Notebook
Open `zulo_bank_notebook.ipynb` in Jupyter and follow through the cells.

### 4. Load Data into PostgreSQL
Ensure PostgreSQL is running, then configure the credentials in the notebook to load the cleaned data into your database.

---

## 📊 Results

- ✅ Redundant fields eliminated via 3NF normalization
- ✅ Date dimension created for advanced time-based reporting
- ✅ PostgreSQL schema populated with production-ready tables
- ✅ Scalable data model ready for BI tools like Power BI or Tableau

---

## 📌 Author

**Rene Fondufe**  
Data Analyst | System Operations | Data Engineering Enthusiast

---

## 📫 Contact

For questions, collaborations, or consulting:  
📧 [rfondufe@gmail.com](mailto:rfondufe@gmail.com)  
📍 United Kingdom

---

## ✅ License

This project is licensed under the MIT License.

