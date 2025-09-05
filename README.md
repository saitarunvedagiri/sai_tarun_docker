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



### 1. Verify Docker Installation
1. Install Docker Desktop on Windows
2. Download Docker Desktop for Windows from Docker Hub
3. Run the installer with default settings.
4. Start Docker Desktop from the Start Menu.
5. If prompted, enable WSL 2 and restart.
Verify installation:
```bash
docker -v
```

### 2. PostgreSQL Setup with Docker
1. Pull the PostgreSQL image:
```bash
docker pull postgres
```
2. Create and start a PostgreSQL container:
```bash
docker run -d -p 5432:5432 --name postgres1 -e POSTGRES_PASSWORD=pass12345 postgres
```
3. Open a terminal inside the container:
```bash
docker exec -it postgres1 bash
```
4. Connect to PostgreSQL with psql:
```bash
psql -d postgres -U postgres
```

