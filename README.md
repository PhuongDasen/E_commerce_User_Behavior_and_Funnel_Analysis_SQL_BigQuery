# [SQL]Explore-Ecommerce-Dataset
<h1>I. Introduction</h1>
This project contains an eCommerce dataset that I will explore using SQL on <a href="https://www.example.com">Google BigQuery</a><br>
The Dataset is based on the Google Analytics public dataset and contains data from an eCommerce website.<br>

<h1>II. Requirements</h1>
<ul>
  <li><a href=https://cloud.google.com/>Google Cloud Platform account</a></li>
  <li><a href=https://cloud.google.com](https://cloud.google.com/bigquery/docs/enable-transfer-service?hl=de#:~:text=Enable%20the%20BigQuery%20Data%20Transfer%20Service,-Before%20you%20can&text=Open%20the%20BigQuery%20Data%20Transfer,Click%20the%20ENABLE%20button.)/>Google BigQuery API</a> enable</li>
  <li><a href=https://cloud.google.com/monitoring/mql/query-editor?hl=de/>SQL query editor</a> or IDE</li>

<h1>III. Dataset Access</h1>
The eCommerce dataset is stored in a public Google BigQuery dataset. To access the dataset, follow these steps:
  <ul>
    <li>Log in to your Google Cloud Platform account and create a new project.</li>
    <li>Navigate to the BigQuery console and select your new created project.</li>
    <li>In the navigation panel, select "Add Data" and then "Search a project".</li>
    <li>Enter the project ID "bigquery-public-data.google _analytics_sample.ga_sessions" and click "Enter".</li>
    <li>Click on the "ga_sessions_" table to open it.</li>
  </ul>

<h1>IV. Exploring the dataset</h1>
  In this project, I will write 08 queries in Bigquery base on Google Analytics dataset.<br>
  <br>
  <b>Query 01: Calculate total visit, pageview, transaction and revenue for January, February and march 2017 order by month</b><br>
    - SQL code <br>
    <img width="829" alt="Screenshot 2025-05-08 at 16 16 05" src="https://github.com/user-attachments/assets/32142a54-d929-4973-b5c1-3f698437a28d" /><br>
    - Query results<br>
    <img width="830" alt="Screenshot 2025-05-08 at 16 16 11" src="https://github.com/user-attachments/assets/dbe64527-72ea-42d8-80e5-edec0bd920b7" /><br>
    <br>
   <b>Query 02: Bounce rate per traffic source in July 2017<br>
   - SQL code<br>
   <img width="832" alt="Screenshot 2025-05-08 at 16 19 39" src="https://github.com/user-attachments/assets/677d5382-4cec-4955-a128-7a0f0b1ea6a1" /><br>
   - Query results<br>
   <img width="830" alt="Screenshot 2025-05-08 at 16 19 47" src="https://github.com/user-attachments/assets/85387045-0ff9-4d45-b491-6a7de6f54cd3" /><br>
    <br>
    <b>Query 03: Revenue by traffic source by week, by month in June 2017<br>
   - SQL code<br>
   <img width="830" alt="Screenshot 2025-05-08 at 16 25 12" src="https://github.com/user-attachments/assets/3b5be772-fb56-44e2-9002-de735f098fe3" /><br>  
   - Query results<br>
   <img width="827" alt="Screenshot 2025-05-08 at 16 24 17" src="https://github.com/user-attachments/assets/7f9564a7-01ca-4460-aba3-5a3f59b41d28" /><br>
    <br>
  <b>Query 04: Average number of product pageviews by purchaser type ( purchasers vs non-purchasers) in June, July 2017<br>
   - SQL code<br>
  <img width="828" alt="Screenshot 2025-05-08 at 16 31 03" src="https://github.com/user-attachments/assets/d960b5ad-c9f4-4155-a4c3-8186bd631c79" /><br>
   - Query results<br>
  <img width="744" alt="Screenshot 2025-05-08 at 16 31 09" src="https://github.com/user-attachments/assets/bf8330ae-d148-40a0-a091-13a49ae3b329" /><br>
 <br>
 <b>Query 05: Average number of transactions per user that made a purchase in July 2017 <br>
   - SQL code<br>
  <img width="824" alt="Screenshot 2025-05-08 at 16 34 00" src="https://github.com/user-attachments/assets/e6c458ba-710a-4194-8190-d6dc2e7c47a4" /><br>
   - Query results<br>
  <img width="744" alt="Screenshot 2025-05-08 at 16 34 07" src="https://github.com/user-attachments/assets/0247dd63-ab36-4dcc-97be-6539d78f45ca" /><br>
<br>
<b>Query 06: Average amount of money spent per session. Only include purchaser data in July 2017 <br>
   - SQL code<br>
 <img width="820" alt="Screenshot 2025-05-08 at 16 39 06" src="https://github.com/user-attachments/assets/910a8720-f0bd-4250-a62e-7eb27e0c80de" /><br>
   - Query results<br>
  <img width="738" alt="Screenshot 2025-05-08 at 16 39 12" src="https://github.com/user-attachments/assets/a746fe20-6824-434c-9652-dc1ca57274d9" /><br>
  <br>
  <b>Query 07: Other products purchased by customers who purchased product "Youtube Men's Vinatge Henley" in July 2017. Output should show product name and the quantity was ordered. <br>
   - SQL code<br>
<img width="823" alt="Screenshot 2025-05-08 at 16 42 11" src="https://github.com/user-attachments/assets/79edb714-f9b6-4b02-a6b2-09f818892133" /><br>
   - Query results<br>
<img width="571" alt="Screenshot 2025-05-08 at 16 42 28" src="https://github.com/user-attachments/assets/dd745781-dfb3-49fb-898c-6f8095eb4350" /><br>
<br>
<b>Query 08: Calculate cohort map from pageview to add to cart to purchase in last 3 months. <br>
 - SQL code<br>
<img width="819" alt="Screenshot 2025-05-08 at 16 50 23" src="https://github.com/user-attachments/assets/abe7f49e-964d-4e88-94df-306774d1983c" /><br>
- Query results<br>
<img width="826" alt="Screenshot 2025-05-08 at 16 52 02" src="https://github.com/user-attachments/assets/7d44b8a0-76e1-41c7-9c49-e4109ca37255" /><br>
<br>
<h1>V. Conclusion</h1>
<ul>
  <li>In conclusion, my exploration of the eCommerce dataset using SQL on Google BigQuery based on the Google Analytics dataset has revealed several intersting insights.</li>
  <li>By exploring eCommerce dataset, I have gained valuable information about total visits, pageview, transactions, bounce rate, and revenue per traffic source,... which could inform future business decisions.</li>
  <li>To ddep dive into the insights and key trends, the next step will visualize the data with some software like Power BI, Tableau,...</li>
  <li>Overall, this project has demonstrated the power of using SQL and big data tools like Google BigQuery to gain insights into large datasets.</li>
</ul>

 

