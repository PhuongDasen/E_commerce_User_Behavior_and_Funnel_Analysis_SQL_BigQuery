<p align="center">
  <img src= "https://github.com/user-attachments/assets/35cc6b0e-31ac-4773-b4f5-75c8ff397b0e" width="90%">
</p>
<h1> 📊 E-commerce User Behaviour and Funnel Analysis (SQL-BigQuery)</h1>
Author: Phuong Dasen<br>
Tool: SQL<br>

## 📑 Table of contents

- [📌 Background & Overview](#📌-background--overview)  
- [📁 Dataset Description & Data Structure](#📁-dataset-description--data-structure)  
- [🧠 Design Thinking Process](#🧠-design-thinking-process)  
- [📊 Key Insights & Visualizations](#📊-key-insights--visualizations)  
- [🔍 Final Conclusion & Recommendations](#🔍-final-conclusion--recommendations)  

---
## [📌 Background & Overview](#📌-background--overview) 

### Goal:
- **📖 What is this project?**  
  - Analyze an e-commerce dataset using SQL in BigQuery to uncover patterns in user behavior, product interactions, and traffic source effectiveness.  
  - Supports insights into engagement, purchasing behavior, and conversion metrics to guide business decisions.

- **👤 Who is this project for?**  
  - Designed for marketing analysts, product managers, and business stakeholders who need data-driven insights.  
  - Also supports data teams in building dashboards and tracking KPIs for performance monitoring.

- **❓ What is the business question of the project?**  
  - What user behaviors, traffic sources, and products lead to higher engagement and conversions?  
  - How can the company improve its marketing funnel and product strategy using these insights?

- **🎯 What is the project outcome?**  
  - Provides clear metrics and funnel analysis on top-performing products and effective user paths to conversion.  
  - Enables strategic, data-driven decisions to boost acquisition, retention, and revenue.

## [📁 Dataset Description & Data Structure](#📁-dataset-description--data-structure)  

### 📌 Data Source
## I. Introduction
This project contains an eCommerce dataset that I will explore using SQL on <a href="https://www.example.com">Google BigQuery</a><br>
The Dataset is based on the Google Analytics public dataset and contains data from an eCommerce website.<br>

## II. Requirements
- [Google Cloud Platform account](https://cloud.google.com/)
- [Enable BigQuery Transfer Service API](https://cloud.google.com/bigquery/docs/enable-transfer-service)
- [SQL query editor](https://cloud.google.com/monitoring/mql/query-editor?hl=de) or IDE
  
## III. Dataset Access
The eCommerce dataset is stored in a public Google BigQuery dataset. To access the dataset, follow these steps:
  <ul>
    <li>Log in to your Google Cloud Platform account and create a new project.</li>
    <li>Navigate to the BigQuery console and select your new created project.</li>
    <li>In the navigation panel, select "Add Data" and then "Search a project".</li>
    <li>Enter the project ID "bigquery-public-data.google _analytics_sample.ga_sessions" and click "Enter".</li>
    <li>Click on the "ga_sessions_" table to open it.</li>
  </ul>
  
## ⚒️Main Process 
🔍 Calculate total visit, pageview, transaction for Jan, Feb and March 2017 (order by month)<br>

![Screenshot 2025-07-02 at 10 15 54 AM](https://github.com/user-attachments/assets/d74497fa-f0fc-433a-a710-b54bf0d6d782)<br>
📤 Query Output <br>
![Screenshot 2025-07-02 at 10 15 45 AM](https://github.com/user-attachments/assets/7fe745da-a078-46f6-a39e-ab68d8f57a75)<br>

🔍 Bounce rate per traffic source in July 2017<br>

<img width="700" alt="Screenshot 2025-07-02 at 10 48 27 AM" src="https://github.com/user-attachments/assets/f8b2b4dc-f70d-4d0b-bb69-9c3289301074" /><br>
📤 Query Output <br>
<img width="700" alt="Screenshot 2025-07-02 at 10 48 37 AM" src="https://github.com/user-attachments/assets/90f1680e-03d1-45fb-9596-fd8d5aef1d94" /><br>

🔍  Revenue by traffic source by week, by month in June 2017<br>

<img width="700" alt="Screenshot 2025-07-02 at 10 49 31 AM" src="https://github.com/user-attachments/assets/325df9d7-17be-47e5-a37a-13a014ac8ef2" /><br>
📤 Query Output <br>
<img width="700" alt="Screenshot 2025-07-02 at 10 49 46 AM" src="https://github.com/user-attachments/assets/2be72812-1e12-439f-8229-c3da1e06ed7f" /><br>

🔍Average number of pageviews by purchaser type (purchasers vs non-purchasers) in June, July 2017<br>

<img width="700" alt="Screenshot 2025-07-02 at 10 50 13 AM" src="https://github.com/user-attachments/assets/025c3b49-1eae-4243-8282-c88b2914ac68" /><br>
📤 Query Output <br>
<img width="700" alt="Screenshot 2025-07-02 at 10 50 39 AM" src="https://github.com/user-attachments/assets/58efd013-c7c7-4969-92ae-056fa72e5936" /><br>

🔍 Average number of transactions per user that made a purchase in July 2017<br>

<img width="700" alt="Screenshot 2025-07-02 at 11 15 23 AM" src="https://github.com/user-attachments/assets/e11d0b9d-ba4d-4a9f-b0f2-0dd5f2d34384" /><br>
📤 Query Output <br>
<img width="700" alt="Screenshot 2025-07-02 at 10 50 39 AM" src="https://github.com/user-attachments/assets/58efd013-c7c7-4969-92ae-056fa72e5936" /><br>

🔍 Average amount of money spent per session. Only include purchaser data in July 2017<br>

<img width="700" alt="Screenshot 2025-07-02 at 11 15 42 AM" src="https://github.com/user-attachments/assets/7282c299-b9c6-4f9d-af98-3be893990af8" /><br>
📤 Query Output <br>
<img width="700" alt="Screenshot 2025-07-02 at 11 15 54 AM" src="https://github.com/user-attachments/assets/e6d781cb-5165-4c37-bfc0-ef5d8eb045f6" /><br>

🔍 Other products purchased by customers who purchased product "YouTube Men's Vintage Henley" in July 2017. Output should show product name and the quantity was ordered<br>

<img width="700" alt="Screenshot 2025-07-02 at 11 16 11 AM" src="https://github.com/user-attachments/assets/33e22dc9-4180-4b18-ac4f-a0f3e4ce6638" /><br>
📤 Query Output <br>
<img width="700" alt="Screenshot 2025-07-02 at 11 16 26 AM" src="https://github.com/user-attachments/assets/3859b8d9-df0d-4cf5-a00e-755e4047f25a" /><br>

🔍Calculate cohort map from product view to addtocart to purchase in Jan, Feb and March 2017<br>

<img width="1000" alt="Screenshot 2025-07-02 at 11 17 10 AM" src="https://github.com/user-attachments/assets/2cf99014-34d5-47ac-bf88-ba0055109a4a" /><br>
📤 Query Output <br>
<img width="900" alt="Screenshot 2025-07-02 at 11 17 21 AM" src="https://github.com/user-attachments/assets/f1ed82f2-8b1d-47e8-a580-c8209f0d4351" />

## 🔎 Final Conclusion & Recommendations

### 📊 Insight 1: Traffic is increasing, but conversion rate stays low
- Visits and pageviews increased from January to March 2017, but the number of transactions remains low.
- ✅ **Recommendation:** Optimize product pages and checkout flow. Run A/B tests to identify friction points in the conversion funnel.

### 🌐 Insight 2: High bounce rates from top traffic sources
- Direct and organic traffic have high visit volumes but also high bounce rates.
- 🔧 **Recommendation:** Improve landing page relevance for each source and add engaging CTAs (calls to action) to reduce bounce rates.

### 💰 Insight 3: Most revenue comes from a few top sources
- Revenue is heavily concentrated in sources like Google and YouTube in June 2017.
- 📈 **Recommendation:** Allocate more marketing budget to high-performing channels and build targeted campaigns around them.

### 🛒 Insight 4: A small set of products generate most of the revenue
- Top-selling products contribute disproportionately to total revenue.
- 🧲 **Recommendation:** Promote these top products via cross-selling, bundling, and featured listings on the homepage.

### 📱 Insight 5: Mobile devices have high traffic but lower conversion
- Mobile generates a large share of visits but underperforms in conversions compared to desktop.
- 📱 **Recommendation:** Optimize the mobile user experience, especially load time, layout, and mobile-friendly checkout.















