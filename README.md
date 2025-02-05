# End-to-End ETL Process (Data Engineering Project)

## Introduction
This project is an end-to-end data engineering pipeline designed to extract and process hourly gasoline prices for any country and weather data for any city. The data extraction is performed using **BeautifulSoup**, while **FastAPI** serves as the interface for data ingestion and interaction. The extracted data is then stored in a **PostgreSQL** database, and the entire workflow is orchestrated using **Apache Airflow** to ensure automation and scheduling.

![ETL Process](images/ETL.gif)

## Data Extraction & Transformation

Gasoline price and weather data are scraped from the internet as **HTML content** and temporarily stored in a designated folder. Using **BeautifulSoup**, the relevant price and weather data are extracted from the HTML. Once extracted, the data is transformed into **JSON format** for further processing and storage.

## Data Loading & Storage

After the data has been extracted and transformed into **JSON format**, it is loaded into a **PostgreSQL database** for structured storage and efficient querying. The database schema is designed to store both gasoline price and weather data, ensuring data integrity and consistency.

Once stored in PostgreSQL, the data can be used for **exploratory data analysis (EDA)**, **report generation**, and **visualization**. Additionally, the stored data serves as a foundation for **training predictive models**, enabling insights such as fuel price forecasting and weather trend analysis.

To maintain data accuracy and prevent redundancy, **data validation checks** are performed before loading, ensuring only clean and structured data is stored in the database.

