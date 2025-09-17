# E-Commerce_Fraud_Dashboard

# This project is built for academic purposes as part of the Loyalist College AI & Data Science Program—Data Analysis Module. Feel free to fork and adapt it for educational use.
<img width="903" height="553" alt="image" src="https://github.com/user-attachments/assets/ec57e685-de12-478d-8593-b7424684d3dc" />

<br>
<br>
A Power BI project that analyzes e-commerce transactions to detect and explain fraud patterns. The dashboard highlights overall trends, country hotspots, and user-behaviour signals across devices, browsers, and acquisition sources.

<br>

# 🔎 Project Overview

This dashboard provides a clear, interactive view of fraud in e-commerce data.
It supports analysts and business stakeholders with:

Overall transaction and fraud trends

Fraud hotspots by country/region

Behavioural patterns by age group, browser, and traffic source

Drill-down interactions and filters (Month, Day, Country, Gender)

# Topic: E-Commerce Fraud Detection & Monitoring

Primary KPIs: Fraud Rate, Total Transactions, Total Fraud Count, Estimated Value Lost

# 🎯 Objectives

- Understand overall transactions and fraud patterns

- Identify fraud hotspots by country

- Uncover patterns across devices, browsers, and user actions

# 🧰 Tools & Tech

Power BI Desktop (DAX, Power Query, Data Model)

Kaggle Dataset: Fraud Ecommerce

DAX measures & calculated columns for dynamic analysis

Power Query for data cleaning, shaping, and transformations

# 📂 Repository Structure
powerbi-ecommerce-fraud-dashboard/
├─ pbix/
│  └─ Ecommerce_Fraud_Dashboard.pbix
├─ README.md

# 📦 Data Source

Link: https://www.kaggle.com/datasets/vbinh002/fraud-ecommerce

Key Fields: signup_time, purchase_time, purchase_value, device_id, user_id, browser, ip_address

Feature Engineering: Added Account Age = time difference between signup and purchase (age of account is often predictive of fraud).

# 🧪 Data Preparation & Modeling

Power Query (ETL):

Standardized gender (M → Male, F → Female)

Joined user metadata to transactions via IP mapping to the country table

Cleaned and typed columns; handled nulls/outliers where appropriate


# 📊 Dashboard Pages
# 1) Overview

KPI Cards: Fraud Rate, Total Users/Transactions

Legit vs Fraud Volume (clustered bar)

Fraud Count by Age Groups (bar)

Fraud vs Non-Fraud Over Time (line)

<img width="903" height="553" alt="image" src="https://github.com/user-attachments/assets/e36255fa-ba40-41de-91fc-c89c82882394" />

# 2) Geographical

Total Fraud Count (All Countries) card

Top 10 Countries by Fraud Occurrence (bar)

Top Countries by Fraud Proportion (treemap with % labels)

Filters: Month, Day, Country, Gender

<p align="center"> <img width="1316" height="549" alt="image" src="https://github.com/user-attachments/assets/ddb8c7c0-d6a6-4991-875d-c6a099264796" />
</p>
# 3) User Behaviour

Total Users card

Users Across Browsers (Fraud vs Legit) (stacked bar)

User Distribution by Browser & Source (matrix)

<img width="905" height="549" alt="image" src="https://github.com/user-attachments/assets/43194fb3-0099-453d-8f3d-b42125cd34ad" />

# 🔍 Exploratory Transformations

Age Group column: derived via DAX 

Gender normalization: M/F → Male/Female

Country mapping: relationship on IP → Country table

# 📈 Key Insights (Preliminary)

Fraud Rate: 9.4% of ~151.11K transactions, peaking early in 2015 and falling later

Hotspots: Highest rates in countries such as Burundi and Bhutan; the United States leads in total fraud occurrences (~10.1K)

Age Patterns: Adult (26–35) and Middle Age (36–50) groups show the highest fraud counts

Sources: SEO and Ads dominate; SEO carries a higher fraud share

# ✅ Deliverables

Fully functional Power BI dashboard with descriptive analytics

Interactive visuals for fraud monitoring & drill-downs

Cleaned & modeled dataset with DAX measures and calculated columns

# 🗓️ Timeline

Week 1 (Mar 12, 2025): Initiation – goals, scope, KPIs (Completed)

Week 2 (Mar 19, 2025): Planning & Wireframes (Completed)

Week 3 (Mar 26, 2025): Data Prep, Build, Test (Completed)

Week 4: (April 3, 2025): Final Dashboard and report presented

# 🚧 Challenges

Creating compact, clear visuals while surfacing multiple fraud patterns and interactions on a limited canvas space.

# 🔮 Next Steps

Deeper analysis of signup-to-purchase time and transaction timestamps

Add Bookmarks to curate interactive story views

# ▶️ How to Run

Download dataset from Kaggle and place CSVs in data/

Open pbix/Ecommerce_Fraud_Dashboard.pbix in Power BI Desktop

If prompted, update Power Query file paths to your local data/ folder

Refresh to load and view the dashboard

# 🙏 Acknowledgements

Dataset: Kaggle – Fraud Ecommerce by vbinh002

Guidance: Prof. Baba (feedback & review)

# 👤 Author

Bikash Ghimirey

LinkedIn: linkedin.com/in/bikash-ghimirey

Email: bikashghimirey@loyalistcollege.com

