# Understanding Liquor Sales in Iowa (Not Production ready)

Data source - https://data.iowa.gov/Sales-Distribution/Iowa-Liquor-Sales/m3tr-qhgy

Data Type - API call and result is a Json File

Time period - The data starts in 2021, January 1st to now. It is upated every month

Size - 23.3M rows and 24 Columns. However using the API you can only get 1000 rows per month.

Objective: 

        - Get State level, vendor level and store level report on the sales of liquor

        - Understand the most demanded liquors and is there a trend

        - Look at who is purchasing the liquor

## Stack
![Alt text](image/iowa_arch.PNG?raw=true "Visualization")

Cloud service - GCP

Infrastructure as code - Terraform

Workflow Orchestrator - Airflow

Data warehouse - Bigquery

Transformation tool - DBT

Dashboard - Google Data studio

## Steps Performed (Scripts available in directories - docker & terraform)
-Create VM and BigQuery table and dataset in GCP using terraform

-Create a docker image of airflow and dbt

-Create extract and load dags

-Create dags to execute dbt for data transformation

-Deploy to VM

-Create Reports using Data Studio

## Visualization
![Alt text](image/iowa.PNG?raw=true "Visualization")


