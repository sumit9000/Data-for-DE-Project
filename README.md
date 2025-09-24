# Azure End-to-End Data Engineering Project 

This project demonstrates how to build a complete **data engineering pipeline** on Microsoft Azure.  
The pipeline covers **data ingestion, transformation, storage, and reporting** using key Azure services.

---

## Architecture Overview


<img width="1919" height="842" alt="image" src="https://github.com/user-attachments/assets/06cbd59a-07a6-4a64-ae67-b49bd528f12f" />



### Components Used:
1. **Azure Data Factory (ADF)**  
   - Handles data ingestion from source systems (HTTP, APIs, files, etc.).
   - Orchestrates movement of raw data into Data Lake.

2. **Azure Data Lake Storage Gen2**  
   - Stores data in two layers:
     - **Raw Zone** → Unprocessed ingested data.  
     - **Transformed Zone** → Cleaned, structured, and transformed data.

3. **Azure Databricks**  
   - Performs data transformation, cleansing, and enrichment.  
   - Converts raw data into analytics-ready format.  
   - Uses Spark notebooks for scalable processing.

4. **Azure Synapse Analytics**  
   - Serves as the data warehouse.  
   - Stores transformed and aggregated data for analytics.  

5. **Power BI**  
   - Connects with Synapse for data visualization and reporting.  
   - Creates dashboards for business insights.

---

## ⚙️ Workflow Steps

1. **Data Ingestion**  
   - ADF copies data from external sources (e.g., HTTP APIs) into Data Lake (raw zone).

2. **Data Transformation**  
   - Databricks cleans and processes data.  
   - Writes transformed data back to Data Lake (transformed zone).

3. **Data Serving**  
   - Transformed data loaded into Azure Synapse Analytics.  

4. **Data Reporting**  
   - Power BI connects to Synapse for visualization.  

---

##  How to Reproduce

1. Create a **Resource Group** in Azure (example: `kaggleRG`).  
2. Deploy the following resources:
   - Azure Data Factory (V2)  
   - Azure Data Lake Storage Gen2  
   - Azure Databricks Workspace  
   - Azure Synapse Workspace  
   - Power BI (external connection)  

3. Configure **Linked Services** in ADF.  
4. Import and run the ADF pipeline.  
5. Use Databricks notebooks to transform data.  
6. Load final data into Synapse.  
7. Connect Power BI and build dashboards.  

---

##  Sample Use Case
- Ingest Kaggle datasets via HTTP.
- Store in Data Lake raw zone.  
- Transform using Databricks (clean missing values, aggregate features).  
- Serve to Synapse.  
- Build Power BI dashboards for reporting.  

---

##  Technologies Used
- **Azure Data Factory**  
- **Azure Data Lake Gen2**  
- **Azure Databricks**  
- **Azure Synapse Analytics**  
- **Power BI**  

---

##  Outcome
This project demonstrates how to implement a **modern data engineering pipeline** on Azure, ensuring scalability, automation, and business-ready reporting.

--- 
