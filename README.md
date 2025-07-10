<p align="center">
  <img src= "https://github.com/user-attachments/assets/35cc6b0e-31ac-4773-b4f5-75c8ff397b0e" width="90%">
</p>
<h1> 📊 E-commerce User Behaviour and Funnel Analysis (SQL-BigQuery)</h1>
Author: Phuong Dasen<br>
Tool: SQL<br>

## 📌 Table of Contents
- [📌 Background & Overview](#-background--overview)
- [📁 Dataset Description & Data Structure](#-dataset-description--data-structure)
- [🧠 Design Thinking Process](#-design-thinking-process)
- [📊 Key Insights & Visualizations](#-key-insights--visualizations)
- [🔍 Final Conclusion & Recommendations](#-final-conclusion--recommendations) 
  
## 📌 Background & Overview
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
<h3>🔍 Calculate total visit, pageview, transaction for Jan, Feb and March 2017 (order by month)</h3><br>

![Screenshot 2025-07-02 at 10 15 54 AM](https://github.com/user-attachments/assets/d74497fa-f0fc-433a-a710-b54bf0d6d782)<br>
<h4>Purpose:</h4> 
To calculate and summarize total visits, pageviews, and transactions for each of the first three months of 2017.
	
📤 Query Output <br>

![Screenshot 2025-07-02 at 10 15 45 AM](https://github.com/user-attachments/assets/7fe745da-a078-46f6-a39e-ab68d8f57a75)<br>
<h4>Analyse:</h4> 
March 2017 had the highest performance with 69,931 visits, 259,522 pageviews, and 993 transactions, showing consistent growth over the three months

<h3>🔍 Bounce rate per traffic source in July 2017</h3><br>
<img width="700" alt="Screenshot 2025-07-02 at 10 48 27 AM" src="https://github.com/user-attachments/assets/f8b2b4dc-f70d-4d0b-bb69-9c3289301074" /><br>
<h4>Purpose:</h4> 
To evaluate the bounce rate per traffic source based on total visits and bounces in July 2017.

📤 Query Output <br>
<img width="700" alt="Screenshot 2025-07-02 at 10 48 37 AM" src="https://github.com/user-attachments/assets/90f1680e-03d1-45fb-9596-fd8d5aef1d94" /><br>
<h4>Analyse:</h4> 
YouTube.com had the highest bounce rate (66.73%), while reddit.com had the lowest (28.57%), with Google being the top source by visit volume.

<h3>🔍  Revenue by traffic source by week, by month in June 2017</h3><br>

<img width="700" alt="Screenshot 2025-07-02 at 10 49 31 AM" src="https://github.com/user-attachments/assets/325df9d7-17be-47e5-a37a-13a014ac8ef2" /><br>
<h4>Purpose:</h4>
To track product revenue contributions by traffic source, broken down by both weekly and monthly aggregates for June 2017.
	
📤 Query Output <br>
<img width="700" alt="Screenshot 2025-07-02 at 10 49 46 AM" src="https://github.com/user-attachments/assets/2be72812-1e12-439f-8229-c3da1e06ed7f" /><br>
<h4>Analyse:</h4> 
The (direct) source generated the highest monthly revenue (97,333.62), while dfa also showed significant revenue (8,862.23) that month.

<h3>🔍Average number of pageviews by purchaser type (purchasers vs non-purchasers) in June, July 2017</h3><br>

<img width="700" alt="Screenshot 2025-07-02 at 10 50 13 AM" src="https://github.com/user-attachments/assets/025c3b49-1eae-4243-8282-c88b2914ac68" /><br>
<h4>Purpose:</h4>
To compare average pageviews between users who made purchases and those who did not in June and July 2017.

📤 Query Output <br>
<img width="700" alt="Screenshot 2025-07-02 at 10 50 39 AM" src="https://github.com/user-attachments/assets/58efd013-c7c7-4969-92ae-056fa72e5936" /><br>
<h4>Analyse:</h4>
Purchasers had significantly more pageviews per session (7.52 in June, 6.62 in July) than non-purchasers (3.76 in June, 3.29 in July).

<h3>🔍 Average number of transactions per user that made a purchase in July 2017</h3><br>

<img width="700" alt="Screenshot 2025-07-02 at 11 15 23 AM" src="https://github.com/user-attachments/assets/e11d0b9d-ba4d-4a9f-b0f2-0dd5f2d34384" /><br>
<h4>Purpose:</h4>
To calculate how many transactions were made on average by each purchasing user in July 2017.
	
📤 Query Output <br>
<img width="700" alt="Screenshot 2025-07-02 at 10 50 39 AM" src="https://github.com/user-attachments/assets/58efd013-c7c7-4969-92ae-056fa72e5936" /><br>
<h4>Analyse:</h4>
Each purchasing user made approximately 1.19 transactions on average in July 2017. 

<h3>🔍 Average amount of money spent per session. Only include purchaser data in July 2017</h3><br>

<img width="700" alt="Screenshot 2025-07-02 at 11 15 42 AM" src="https://github.com/user-attachments/assets/7282c299-b9c6-4f9d-af98-3be893990af8" /><br>
<h4>Purpose:</h4>
To determine how much revenue was generated per session among users who made purchases in July 2017.
📤 Query Output <br>
<img width="700" alt="Screenshot 2025-07-02 at 11 15 54 AM" src="https://github.com/user-attachments/assets/e6d781cb-5165-4c37-bfc0-ef5d8eb045f6" /><br>
<h4>Analyse:</h4>
The average revenue per session was $8.97, based only on sessions with at least one purchase.

<h3>🔍 Other products purchased by customers who purchased product "YouTube Men's Vintage Henley" in July 2017. Output should show product name and the quantity was ordered</h3><br>

<img width="700" alt="Screenshot 2025-07-02 at 11 16 11 AM" src="https://github.com/user-attachments/assets/33e22dc9-4180-4b18-ac4f-a0f3e4ce6638" /><br>
<h4>Purpose:</h4>
To identify cross-purchased products among users who bought the “YouTube Men’s Vintage Henley” in July 2017.
📤 Query Output <br>
<img width="700" alt="Screenshot 2025-07-02 at 11 16 26 AM" src="https://github.com/user-attachments/assets/3859b8d9-df0d-4cf5-a00e-755e4047f25a" /><br>
<h4>Analyse:</h4>
Customers also frequently bought Google Navy Speckled Pullover Hoodie (9 units) and YouTube Black Cuffed Beanie (8 units) along with the Henley.

<h3>🔍Calculate cohort map from product view to addtocart to purchase in Jan, Feb and March 2017</h3><br>

<img width="1000" alt="Screenshot 2025-07-02 at 11 17 10 AM" src="https://github.com/user-attachments/assets/2cf99014-34d5-47ac-bf88-ba0055109a4a" /><br>
<h4>Purpose:</h4>
To track user behavior through the conversion funnel across three stages: product view, add to cart, and purchase for Q1 2017.
📤 Query Output <br>
<img width="900" alt="Screenshot 2025-07-02 at 11 17 21 AM" src="https://github.com/user-attachments/assets/f1ed82f2-8b1d-47e8-a580-c8209f0d4351" />
<h4>Analyse:</h4>
The funnel shows strong drop-offs at each stage, with March having the highest conversion from view to purchase (~3.91%), indicating improved efficiency over the months.

## 🔎 Final Conclusion & Take Away

* The project explored how users interact with an online store, such as analyzing monthly trends in visits, pageviews, and transactions — for example, March 2017 showed the highest number of purchases.
* It revealed how different sources (like Google or YouTube) influence user behavior — for instance, YouTube brought fewer visitors but had the highest bounce rate, meaning users often left quickly.
* By comparing purchasers and non-purchasers, it became clear that buyers viewed more pages per session — in July, buyers viewed an average of 6.6 pages while non-buyers viewed only 3.3.
* A funnel analysis showed where users drop off before completing a purchase — for example, only a small percentage of users who viewed a product actually completed a transaction.
* The project demonstrated how user data can be turned into clear, actionable insights — such as identifying that most revenue in June came directly from users rather than referrals or ads.
<h3>Recommendation</h3>
Focus on reducing bounce rate from high-volume sources (e.g. YouTube), personalize re-engagement strategies for non-purchasers, and optimize product pages to strengthen the conversion funnel.














