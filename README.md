# Data-Engineering-Olympics-Data
🚀 Building a Scalable ETL Pipeline with Microsoft Azure
🧱 Architecture Overview



📥 Data Ingestion

 I sourced a CSV dataset from a GitHub repository using an HTTP connection. This data was ingested directly into Azure Data Lake Storage Gen2, into a container labeled Bronze, representing raw unprocessed data.



⚙️ Data Transformation with Azure Databricks

 The Bronze container was connected to Azure Databricks, where I used PySpark notebooks to clean and transform the dataset.

Handled missing values

Standardized column names

Performed necessary joins and filtering

The cleaned dataset was then saved back into the Data Lake as:

✅ transformed_data.csv (processed output)

📝 raw_data.csv (original input for reference)



📊 Analysis with Azure Synapse Analytics

 I connected Synapse Analytics to the transformed dataset in the Data Lake and ran SQL queries to perform data analysis.

 Instead of using external BI tools, I utilized the Synapse built-in studio for analytics



📈 Optional Dashboarding

 While I didn’t use Tableau or Power BI in this build, the architecture supports easy integration for visual dashboards in the future.

✅ Highlights

End-to-end data flow: GitHub ➡ Data Lake ➡ Databricks ➡ Synapse Analytics

Organized raw and transformed data layers for modularity and traceability

Used native Synapse features for quick data exploration and reporting

Built entirely on cloud-native, scalable, and secure architecture
