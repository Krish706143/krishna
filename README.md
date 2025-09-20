 Designed andi mplemented a complete data pipeline to automate fault ticket analysis:
 
 •Ingested weekly CSV dumps(~5,000 tickets)from on-premisesSQL Serverto Azure DataLakeStorage (ADLS)
 using Azure Data Factory with Self-hosted Integration Runtime.
 
 • Fetched and secured data from Azure Data Lake Storage (ADLS) to Azure Databricks using SAS tokens, and processed data by
 accessing the ADLS Bronze layer with controlled access permissions.
 
 • Removeddelimiters, corrected mismatched values, handled nulls, eliminated duplicates, and stored the cleaned data in the Silver
 layer of Azure Databricks.
 
 • Applied aggregation transformations to meet KPI requirements by retrieving ticket details exceeding the SLA threshold of 20
 minutes, in line with client specifications, and stored the results in the Gold layer of Azure Databricks.
