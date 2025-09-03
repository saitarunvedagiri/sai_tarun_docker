# Hands-On 3: Docker Microservice (ITCS 6190/8190)

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




```bash
docker -v
docker-compose -v
git clone <your-github-repo-link>
cd <your-project-directory>
docker-compose up --build
docker ps
wsrfgsrtjytyukjm
http://localhost:5000
docker-compose logs -f
docker-compose down
