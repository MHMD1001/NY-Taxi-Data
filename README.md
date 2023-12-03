# NY Taxi Data Ingestion Project

This project demonstrates an end-to-end data pipeline for ingesting New York City taxi data into a PostgreSQL database. The pipeline is containerized using Docker and includes a Python script for data retrieval and insertion. Additionally, pgAdmin is used for database management

## Project Overview

The data pipeline consists of the following components:

1. **Dockerized Python Script:**
   - A Docker container with a Python script (`ingest_data.py`) that retrieves taxi data from a (TLC Trip Record) and inserts it into a PostgreSQL database

2. **PostgreSQL Container:**
   - A Docker container running PostgreSQL to store the ingested taxi data

3. **pgAdmin Container:**
   - A Docker container running pgAdmin for database management and visualization

4. **Docker Compose:**
   - The `docker-compose.yml` file orchestrates the deployment of the PostgreSQL, pgAdmin, and Python script containers

## How to Run

1. **Clone this Repository:**
   ```bash
   git clone https://github.com/MHMD1001/ny-taxi-data-ingestion.git
   cd ny-taxi-data-ingestion

## Build and Run Docker Containers:
```bashdocker-compose up```
This command will start the PostgreSQL, pgAdmin, and Python script containers

## Access pgAdmin:
- Open a web browser and go to http://localhost:8080
- Log in with the following credentials:
- Email: admin@admin.com
- Password: root
- Set up a new server connection to the PostgreSQL database (ny_taxi)

## Additional Note
Customize the Docker Compose environment variables in the docker-compose.yml file according to your preferences
