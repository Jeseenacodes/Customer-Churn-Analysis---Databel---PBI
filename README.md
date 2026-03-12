

# 📊 Databel Customer Churn Analysis — Power BI Dashboard

## Project Overview

Customer churn is one of the most critical challenges for subscription-based businesses, particularly in the telecommunications industry. Identifying why customers leave and which segments are most at risk allows organizations to design more effective retention strategies.

This project analyzes customer churn for **Databel**, a fictional telecom company, using **Power BI**. The objective was to uncover key drivers of churn, identify high-risk customer segments, and present insights through an interactive business intelligence dashboard.

The project demonstrates how data analytics and visualization can transform raw operational data into actionable business insights.

---

# Business Problem

Customer churn directly impacts revenue and growth. Businesses must understand:

* Why customers are leaving
* Which customer segments are most likely to churn
* How pricing, contracts, and usage patterns influence churn behavior

This analysis aims to support **data-driven retention strategies** by identifying churn patterns across multiple dimensions.

---

# Project Objectives

The key objectives of this analysis were:

* Measure overall churn rate and customer retention trends
* Identify the primary reasons customers leave
* Analyze churn behavior across demographics, contracts, and service usage
* Detect high-risk customer segments
* Build an interactive Power BI dashboard for business stakeholders

---

# Dataset

The dataset used in this project was provided by **DataCamp** and simulates customer data for a telecommunications company.

### Data Categories

**Customer Information**

* Customer ID
* Churn Label
* Churn Reason

**Demographics**

* Gender
* Age
* Under 30 Indicator
* Senior Indicator
* State

**Contract & Billing**

* Contract Type
* Payment Method
* Account Length
* Number of Customers in Group

**Service Usage**

* Local Calls
* International Calls
* International Plan
* Average Monthly Data Usage
* Monthly Charges

---

# Tools & Technologies

* **Power BI** — Data visualization and dashboard creation
* **DAX** — Calculated columns and measures
* **Power Query** — Data preparation and transformation
* **Data Modeling** — Relationship building and dataset optimization

---

# Dashboard Structure

The Power BI dashboard is divided into four analytical sections:

### 1️⃣ Churn Overview

Provides a high-level snapshot of overall churn performance.

Key visuals include:

* KPI Cards (Churn Rate, Total Customers, Churned Customers)
* Churn Reason Analysis
* Churn Category Distribution
* Churn by Payment Method
* Tenure (Account Length) Slicer

Key Insight:
Competitor offers are the leading cause of customer churn.

---

### 2️⃣ Demographic Analysis

Examines churn patterns across demographic segments and geographic regions.

Visuals include:

* Churn by State Table
* Geographic Churn Map
* Churn Rate by Gender
* Churn Rate by Age Group
* Customers vs Churn Rate by Age (Binned)

Key Insight:
Younger customers show higher churn volatility, while senior customers demonstrate more stable retention.

---

### 3️⃣ Contract & Billing Insights

Analyzes how contract types and pricing influence customer retention.

Visuals include:

* Churn Rate by Contract Type
* Group Contract Size vs Churn Rate
* Contract Type vs Gender
* Churn by Account Length and Contract Type

Key Insight:
Month-to-month contracts show significantly higher churn rates compared to long-term contracts.

---

### 4️⃣ Service Usage & Subscription Behavior

Investigates how customer usage patterns impact churn.

Visuals include:

* Customer Service Call Metrics
* Data Consumption Groups
* Unlimited Data Plan vs Churn Rate
* International Plan Activity

Key Insight:
Customers subscribed to unlimited data plans but with low data usage exhibit higher churn rates.

---

# Key Insights

Major churn drivers identified through the analysis include:

* Competitor offers are the most common churn reason
* Customers on **month-to-month contracts** churn significantly more
* High churn occurs during the **early lifecycle of customers**
* Higher **monthly charges correlate with higher churn**
* Customers paying for services they do not fully use (e.g., unlimited data) show higher churn rates
* Churn rates vary significantly by geographic region

---

# Business Recommendations

Based on the analysis, the following strategies could help reduce churn:

* Introduce incentives for **long-term contracts**
* Improve **pricing competitiveness**
* Offer **flexible or usage-based data plans**
* Implement **early customer engagement programs**
* Improve billing experiences for customers using paper checks
* Identify and proactively support **high-risk customer segments**

---

# Example DAX Calculations

### Demographic Segmentation

```DAX
Demographics =
IF('Databel — Data'[Senior] = "Yes", "Senior",
IF('Databel — Data'[Under 30] = "Yes", "Under 30", "Other"))
```

### Data Consumption Grouping

```DAX
Grouped Consumption =
IF('Databel — Data'[Avg Monthly GB Download] < 5, "Less than 5 GB",
IF('Databel — Data'[Avg Monthly GB Download] < 10, "Between 5 and 10 GB",
"10 or more GB"))
```

---

# Project Outcome

This project demonstrates how Power BI can be used to:

* Perform exploratory churn analysis
* Identify key business drivers
* Transform complex data into actionable insights
* Communicate findings through interactive dashboards

The final dashboard enables stakeholders to quickly understand churn patterns and make informed decisions to improve customer retention.


---

# Screenshots

*( screenshots )*

Example:

```
![Dashboard Overview](images/dashboard-overview.png)
```

---

# Learning Outcomes

Through this project, I strengthened skills in:

* Data modeling in Power BI
* DAX calculations
* Business-focused dashboard design
* Data storytelling
* Customer churn analysis

---

⭐ If you found this project useful, feel free to explore the dashboard and share feedback.

