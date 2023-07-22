# Azure Data pipeline for flight delay prediction due to weather

The project entails 3 different types of sources namely web API, SQL and noSQL database. Weather data fetched from the API is processed using pyspark in azure databricks due to complexity of the json response and stored back in a data lake. The SQL and noSQL database is ingested using azure data factory’s dataflow and joined with the processed weather dataset focussing on departure airport. The dataflow transformation involves cleansing, date processing etc and the adf pipeline pushes the transformed data into the data lake in parquet format. Azure ML studio is then used to build a decision tree regressor model along with an endpoint.

Detailed presentation and report with screenshots are attached for reference.
