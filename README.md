## ETL NBA Player Dataset Using Talend and Storing it into BigQuery
Extract Transform Load NBA dataset using Talend Open Studio and Storing it into Big Query Databases.

The purpose of this project is to extract dataset from csv online using Talend Open Studio, transform with several basic technique using tmap component on Talend. The next one is storing to big query data lake. From data lake table, filter exclude null or No Data, filter just all teams from Pacific Division. Finnaly, Storing into Big Query Data Warehouse for Pacific Division Teams.

Download Dataset file : https://media.geeksforgeeks.org/wp-content/uploads/nba.csv

# Goals of the Project:
1.  Ingest Data csv using Talend Component
2.  Storing data csv to Big Query Data Lake
3.  Filter and Clean the Data using tBiqQueryInput Talend Component.
4.  Storing the final Data into Big Query Data Warehause.

# prerequisite
1. Using Talend Open Studio for Big Data
2. Using Java 11
3. Have a Big Query (Google Cloud) Account

# Lesson Result
![image](https://github.com/user-attachments/assets/e45b7f42-3a48-48af-b018-4b2845b25f79)

1.  After download csv dataset to my local computer, create tFileInputDelimited and open nba dataset file. Field separator "," and Header 1.
2.  Adding tMap component for cleansing, formating, and validating the Data.
3.  Adding tBigQueryOutput. Config the credentials needed such as security key, project id, dataset, bucket, file storage google cloud.
4.  Adding tBigQueryInput. Create SQL Query with where clause inside.
5.  Adding tBigQueryOutput. This one is different from previous one. This is Big Query Data Warehouse for specific teams.
6.  
