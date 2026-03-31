# Dockerizing

## Overview
The app folder contains the source code for a Streamlit app with a user interface for uploading a CSV file. Once the CSV file is uploaded, the application loads it into a PostgreSQL database table for persistence, then reads the data from that table. It displays the first 5 rows and the summary statistics of the numerical columns in the table.

I have been tasked with containerizing this application using Docker so it can be easily deployed in a production environment. Additionally, the Docker image is published on Docker Hub to allow other team members to pull and run it on their machines.
Since the data needs to be persisted to PostgreSQL, the app needs to be connected to a PostgreSQL container. This means multiple images need to be created and run using Docker Compose. The resulting files can be accessed in the appropriate folders.

The Docker image can also be accessed on Docker Hub.
[Docker Image on Docker Hub](https://hub.docker.com/repository/docker/muminah/docker-project/general
)

###### credit ->
Najeeb Sulaiman. [Link to the repo](https://github.com/Najeeb-Sulaiman/dec_docker_training/blob/master/task.md) 
