# End-to-End ETL Process (Data Engineering Project)

## Introduction
This project is an end-to-end data engineering pipeline designed to extract and process hourly gasoline prices for any country and weather data for any city. The data extraction is performed using **BeautifulSoup**, while **FastAPI** serves as the interface for data ingestion and interaction. The extracted data is then stored in a **PostgreSQL** database, and the entire workflow is orchestrated using **Apache Airflow** to ensure automation and scheduling.

