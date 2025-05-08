# 🚀 fastapi-prod-app

A production-ready, containerized Python web application built with **FastAPI**, **PostgreSQL**, **Redis caching**, and **Nginx reverse proxy** — all orchestrated using **Docker Compose**.

This setup is optimized for performance and security, using **multi-stage builds**, **Alpine-based images**, and includes a **Trivy security scan report**.

---

## 🧰 Tech Stack

- **FastAPI** – High-performance Python web framework
- **PostgreSQL** – Relational database
- **Redis** – In-memory data store for caching
- **Nginx** – Reverse proxy server
- **Docker Compose** – Multi-container orchestration
- **Trivy** – Container vulnerability scanner

---

## 📦 Features

- ✅ FastAPI RESTful backend
- ✅ PostgreSQL database with persistent volume
- ✅ Redis cache integration
- ✅ Nginx reverse proxy with production config
- ✅ Multi-stage Docker build for optimized image size
- ✅ Alpine-based images for minimal footprint
- ✅ Security scan with Trivy or Docker Scout
- ✅ Easily extensible for real-world production apps

---

## 📁 Project Structure
fastapi-prod-app/
├── app/ # FastAPI application code
│ ├── main.py
├── nginx/
│ └── nginx.conf # Nginx config
├── docker-compose.yml
├── Dockerfile # Multi-stage FastAPI build
├── requirements.txt
└── README.md
----

Create .env file

```bash
POSTGRES_USER=admin
POSTGRES_PASSWORD=admin123
POSTGRES_DB=app_db
REDIS_HOST=redis
REDIS_PORT=6379
```
---

Build and run the stack

```bash
docker-compose up --build
```
---

## Security Scan

```bash
trivy image fastapi-prod-app > trivy-report.txt
```
---
 ## Architecture Diagram

 ![image](https://github.com/user-attachments/assets/87123f40-5bdd-446a-87aa-59e15ae616a1)![image](https://github.com/user-attachments/assets/e2d56fed-9cab-4335-8004-26d3008c51c7)


