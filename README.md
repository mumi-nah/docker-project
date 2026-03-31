# Dockerizing

## Overview
The app folder contains the source code for a Streamlit app with a user interface for uploading a CSV file. Once the CSV file is uploaded, the application loads it into a PostgreSQL database table for persistence, then reads the data from that table. It displays the first 5 rows and the summary statistics of the numerical columns in the table.

I have been tasked with containerizing this application using Docker so it can be easily deployed in a production environment. Additionally, the Docker image is published on Docker Hub to allow other team members to pull and run it on their machines.
This repository houses the Dockerfile and Docker-Compose to 
[Docker Image on Docker Hub](https://hub.docker.com/repository/docker/muminah/docker-project/general
)
