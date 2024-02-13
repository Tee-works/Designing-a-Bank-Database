# Bank Marketing Campaign Data Engineering Project

## Overview
In the competitive realm of personal banking, effective marketing strategies can significantly boost profitability. With interest rates generating substantial revenue streams, it's imperative for banks to optimize their marketing campaigns. This project aims to fortify the marketing efforts of a prominent bank by engineering a robust data pipeline that cleans, processes, and stores data collected from their personal loan campaign.

### Project Goals
The primary objective of this project was to assist the bank in setting up a PostgreSQL database to store and manage data from their recent and future marketing campaigns. To achieve this, I was tasked with the following:

1. Clean and preprocess the provided bank_marketing.csv data.
2. Design a database schema to accommodate the current and future campaign data.
3. Implement an ETL pipeline using pandas for data manipulation and SQL for database operations.
4. Ensure the security of the database design by providing SQL code as multiline string variables.

### Database Schema Design
The designed PostgreSQL database consists of three interconnected tables:

* Client Table: Stores detailed client information, facilitating personalized marketing strategies.
* Campaign Table: Captures campaign-specific data points, enabling the bank to analyze the effectiveness of each campaign.
* Economics Table: Holds economic indicators that impact consumer behavior, aiding in macroeconomic analysis.

### Methodology
The ETL process involved several steps, each designed to enhance the integrity and usability of the data:

* Extraction: Data was read from the CSV file into pandas DataFrames, divided into three segments based on the future table structures.
* Transformation: Data was cleaned and reformatted. This included handling missing values, standardizing text entries, converting binary outcomes, and creating new columns for better analysis.
* Loading: The transformed data was then saved into separate CSV files, ready to be loaded into the PostgreSQL database.
  
### SQL Database Creation
The database creation was facilitated by SQL code that:

* Defines the table structures and relationships.
* Populates the tables with data from the CSV files using the PostgreSQL \copy command.
* Ensures the security of data operations by avoiding direct interaction with the database server.
  
### Tools Used
* pandas: For data manipulation and splitting the data into separate tables.
* NumPy: To handle missing values and perform other numerical operations.
* PostgreSQL: As the database management system to store and manage the campaign data.

### Conclusion
The successful completion of this project not only streamlines the data storage process for the bank's marketing campaign but also sets the stage for more efficient and data-driven marketing efforts in the future. With a scalable and secure database in place, the bank is now well-equipped to harness their data for insightful decision-making and to adapt to the ever-evolving financial landscape.
