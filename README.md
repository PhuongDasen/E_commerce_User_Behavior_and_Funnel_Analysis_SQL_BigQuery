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
   <b>Query 02: Bounce rate per traffic source in July 2017<br>
   - SQL code <br>
   <img width="832" alt="Screenshot 2025-05-08 at 16 19 39" src="https://github.com/user-attachments/assets/677d5382-4cec-4955-a128-7a0f0b1ea6a1" /><br>
   - Query results <br>
   <img width="830" alt="Screenshot 2025-05-08 at 16 19 47" src="https://github.com/user-attachments/assets/85387045-0ff9-4d45-b491-6a7de6f54cd3" /><br>


