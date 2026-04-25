# 🏍️ Project Matrix — Honda Sales Data Analysis

A data science project focused on cleaning, analyzing, and visualizing Honda sales data using **Python**, **Pandas**, **NumPy**, **Matplotlib**, and **Seaborn**.

---

## 📁 Project Structure

```
project_matrix/
├── data/
│   └── honda_sales.csv
├── notebooks/
│   └── honda_sales_analysis.ipynb
├── visuals/
│   └── (generated charts)
└── README.md
```

---

## ✅ Progress Tracker

| Task | Status |
|------|--------|
| Data Cleaning | ✅ Done |
| Sales Analysis | ✅ Done |
| Customer Analysis | ✅ Done |
| Visualizations | ✅ Done |
| Business Insights | ✅ Done |
| Profit Prediction | ✅ Done |

---

## 🧹 1. Data Cleaning

### Basic Cleaning
- Convert `Order_Date` → `datetime`
- Check missing values using `isnull()`
- Remove duplicate records
- Fix data types (`int`, `float`)

### Column-wise Cleaning
- `Customer_Age` → Remove unrealistic values (age `< 18` or `> 80`)
- `Customer_Gender` → Standardize to `Male` / `Female` only

### Regex Cleaning 🔥
- Extract year/month from date columns
- Clean dealer names (remove extra whitespace)
- Standardize city/state names

```python
import re
df['City'] = df['City'].str.replace(r'\s+', ' ', regex=True)
```

---

## 📊 2. Analysis

### 💰 Sales Analysis
- Total sales by **Year / Month**
- Total sales by **State / City**

### 👥 Customer Analysis
- Age distribution across buyers
- Gender-wise purchase breakdown
- Preferred payment methods

### 🚀 Business Insights
- Which bike model generates the highest profit
- Which city generates maximum revenue
- Online vs Showroom sales comparison

### ⏱️ Operational Insights
- Delivery days vs customer rating
- Does faster delivery correlate with better ratings?

---

## 📈 3. Visualizations

### 📅 Sales Trends
- **Line Chart** → Sales over time
- **Pie Chart** → Payment mode distribution (UPI / Cash / Credit Card)

### 🏆 Top Models / Cities
- **Bar Chart** → Top bike models by sales
- **Bar Chart** → Top cities by revenue

### 👥 Customer Insights
- **Pie Chart** → Gender distribution
- **Bar Chart** → Age distribution

---

## 🚀 4. Feature Engineering

Create a new `Profit_Percent` column:

```python
df['Profit_Percent'] = (df['Gross_Profit'] / df['Cost_Price']) * 100
```

### Prediction Goals
- Identify which factors affect profit the most
- Predict which customers are likely to buy expensive bikes

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| `Pandas` | Data manipulation & cleaning |
| `NumPy` | Numerical analysis |
| `Matplotlib` | Data visualization |
| `Seaborn` | Statistical plots |
| `Regex` | Text cleaning & pattern matching |

---

## ⭐ Summary

With this dataset, this project demonstrates how to:
- **Clean** raw sales data using Pandas + Regex
- **Analyze** trends and patterns using NumPy + Pandas
- **Visualize** actionable insights using Matplotlib + Seaborn
- **Engineer features** to enable profit prediction and customer segmentation

---

> 📌 *Project by: [Team Data-Matrix] | Dataset: Honda Sales Data*------

