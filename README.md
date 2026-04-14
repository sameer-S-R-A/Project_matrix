# Project_matrix
Data science project of Honda Sales Data Analysis.
# ☑️☑️☑️☑️☑️☑️☑️☑️☑️☑️☑️☑️☑️☑️☑️☑️☑️☑️☑️☑️☑️☑️

⸻

# 🧹 1. Data Cleaning (using Pandas + Regex)

✔️ Basic Cleaning
	•	Convert Order_Date → datetime
	•	✅Check missing values (isnull())
	•	✅Remove duplicates
	•	✅Fix data types (int, float)

✔️ Column-wise Cleaning
	•	✅Customer_Age → remove unrealistic values (like <18 or >80)
	•	✅Customer_Gender → standardize (Male/Female only)

✔️ Using Regex (important 🔥)
	•	Extract year/month from date if needed
	•	Clean text columns:
	•	✅Dealer names → remove extra spaces
	•	Standardize city/state names
	•	Example:

import re
df['City'] = df['City'].str.replace(r'\s+', ' ', regex=True)


⸻

# 📊 2. Analysis You Can Do

💰 Sales Analysis
	•	✅Total sales by:
	•	✅Year / Month
	•	✅State / City
	•	✅

👥 Customer Analysis
	•	Age distribution
	•	✅Gender-wise purchases
	•	✅Preferred payment methods

🚀 Business Insights
	•	Which bike gives highest profit
	•	Which city generates max revenue
	•	Online vs Showroom sales comparison

⏱️ Operational Insights
	✅•	Delivery days vs customer rating
	✅•	Does faster delivery = better rating?

⸻

# 📈 3. Visualizations (Matplotlib + Seaborn)

📅 Sales Trends
	•	✅Line chart → Sales over time
	•	✅Payment_Mode → Make a pie-chart (UPI, Cash, Credit Card) to check what percentage of costomer using which payment methord

⸻

🏆 Top Models / Cities
	•	✅Bar chart → Top bike models / cities

⸻

👥 Customer Insights
	•	✅Pie chart → Gender distribution
	•	✅bargram → Age distribution

⸻



⸻


# 🚀•	Create new column:

df['Profit_Percent'] = (df['Gross_Profit'] / df['Cost_Price']) * 100

	•	Predict:
	•	Which factors affect profit most
	•	Which customers are likely to buy expensive bikes

⸻

# ⭐ Final Summary

With this dataset you can:
	•	Clean data using Pandas + Regex
	•	Analyze trends using NumPy + Pandas
	•	Visualize insights using Matplotlib + Seaborn



⸻


# 🌟
![image.png](attachment:image.png)
