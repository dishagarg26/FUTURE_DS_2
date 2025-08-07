
# 🛍️ Marketing Campaign Dataset Dashboard

This project presents an interactive **Looker Studio Dashboard** built using a cleaned marketing campaign dataset. The dashboard helps analyze customer demographics, spending behavior, campaign effectiveness, and purchasing channels.

---

## 📁 Dataset Overview

The dataset consists of **2240 customer records** and **31 fields** collected from a direct marketing campaign. It includes demographic details, purchasing history, campaign responses, and engagement metrics.

### 🔑 Key Columns

| Column Name         | Description |
|---------------------|-------------|
| `ID`                | Unique customer identifier |
| `Year_Birth`        | Year of birth |
| `Age`               | Customer's age (pre-calculated) |
| `Education`         | Education level (e.g., Graduation, PhD) |
| `Marital_Status`    | Marital status |
| `Income`            | Annual household income |
| `Kidhome` / `Teenhome` | Number of children and teenagers at home |
| `Dt_Customer`       | Date of becoming a customer |
| `Recency`           | Days since last purchase |
| `MntWines` - `MntGoldProds` | Money spent on various product categories |
| `NumDealsPurchases` | Number of purchases using a discount |
| `NumWebPurchases`, `NumCatalogPurchases`, `NumStorePurchases` | Channel-based purchases |
| `NumWebVisitsMonth` | Monthly website visits |
| `AcceptedCmp1` - `AcceptedCmp5` | Response to each campaign |
| `Response`          | Overall campaign response |
| `Complain`          | Whether the customer complained |
| `Total_Spend`       | Total monetary spend (sum of all categories) |
| `Total_Purchases`   | Total number of purchases across all channels |
| `Country`           | Country of residence |

---

## 📊 Dashboard Insights
This dashboard was created in **Looker Studio** and includes the following key visualizations:

- **Scorecards**: 
  - Total Spend: `1.4M`
  - Total Purchases: `33.3K`

- **Pie Charts**:
  - Total Spend by Education
  - Record Count by Marital Status
  - Total Purchases by Country

- **Bar Chart**:
  - Spend by Product Category

- **Column Chart**:
  - Complaint Impact on Total Spend

- **Time Series**:
  - Purchases Over Time

- **Table View**:
  - Top customer records with Age, Education, Income, Country, and Total Spend

---

## 📌 Calculated Fields

- `Total_Spend = Sum(MntWines to MntGoldProds)`
- `Total_Purchases = Sum(NumWebPurchases, NumCatalogPurchases, NumStorePurchases, NumDealsPurchases)`


## 🚀 Getting Started

### 1. Import the CSV to Google Sheets
- Upload the `marketing_data_cleaned.csv` to your Google Drive
- Open Looker Studio and connect it as a data source

### 2. Create Dashboard Components
- Follow the widget breakdown in the `/docs/dashboard_structure.md` (optional)

---

## 🤖 Tools Used
- Python (Pandas) for preprocessing
- Looker Studio for dashboarding
- Google Sheets for cloud integration




