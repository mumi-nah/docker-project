# Dockerizing a Streamlit Data App

---
## Overview
This project contains a Streamlit application that allows users to upload a CSV file. Once uploaded, the application processes the data and stores it in a PostgreSQL database. It then retrieves the data to display the first 5 rows and summary statistics for numerical columns.

The goal of this project was to containerize the application using Docker so it can be easily set up and run in any environment.

Since the application depends on PostgreSQL for data storage, Docker Compose was used to run both the app and the database as separate services, with the app depending on PostgreSQL.

---

## Project Structure

```
├── app/
│ ├── Dockerfile
│ ├── data_process.py
│ ├── data_process_db.py
│ ├── requirements.txt
│ └── student.csv
├── docker-compose.yaml
└── README.md
```
---

## How to Run the Project

1. Clone the repository:
```bash
git clone https://github.com/mumi-nah/docker-project
cd docker-project
```
2. Build and run the containers
```
docker-compose up
```
3. Open your browser and access the app at:
```http://localhost:8501```

## Docker Setup

### Dockerfile
Defines the environment for the Streamlit app
Installs dependencies from requirements.txt
Copies application files into the container
Runs the Streamlit app

### Docker Compose
Sets up two services:
app → runs the Streamlit application
db → runs PostgreSQL
Handles communication between the app and the database
Ensures both services start together

The Docker image can also be accessed on Docker Hub.
[Docker Image on Docker Hub](https://hub.docker.com/repository/docker/muminah/docker-project/general
)

## What I learned
- Writing Dockerfiles
- Working with containers
- Debugging build errors

##### credit ->
Original project by Najeeb Sulaiman. [Link to the repo](https://github.com/Najeeb-Sulaiman/dec_docker_training/blob/master/task.md) 
