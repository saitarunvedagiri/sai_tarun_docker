# Hands-On L3: Installing Docker & Building a Multi-Container Microservice  

**Course:** Cloud Computing for Data Analysis – ITCS 6190/8190, Fall 2025  
**Instructor:** Marco Vieira  

This project demonstrates the setup and deployment of a Python Flask web application with a Redis cache and PostgreSQL database using Docker Desktop and Docker Compose.  

---



## Student Info
- **Name:** Sai Tarun Vedagiri  
- **Student ID:** 801421332  
- **Email:** svedagi1@charlotte.edu  

---

## Project Description
This project demonstrates setting up and orchestrating a multi-container microservice using Docker.  
It includes:
- A **PostgreSQL** database container.
- A **Flask web application** container.
- A **Redis cache** container.

All services are managed using **Docker Compose**.

---

## Execution Steps



#### 1. Verify Docker Installation
#### 2. PostgreSQL Setup
#### 3. Run PostgreSQL container:
#### 4.Access the container:
#### 5.Open PostgreSQL prompt:
```bash
docker -v
docker pull postgres
docker run -d -p 5432:5432 --name postgres1 -e POSTGRES_PASSWORD=pass12345 postgres
docker exec -it postgres1 bash
psql -d postgres -U postgres

