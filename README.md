# Prometheus + Grafana Monitoring for a Containerized Flask Application

A minimal, production-style monitoring setup using **Prometheus** and **Grafana** to monitor a containerized **Python Flask application**.  
This project demonstrates core observability concepts such as metrics exposure, scraping, visualization, and containerized service communication.

---

## 🚀 Project Overview

This project implements end-to-end monitoring for a sample Flask application using:
- **Prometheus** for metrics collection
- **Grafana** for visualization
- **Docker & Docker Compose** for container orchestration

The application exposes custom metrics which are scraped by Prometheus and visualized through Grafana dashboards.

---

## 🏗️ Architecture

Flask App (/metrics) → Prometheus → Grafana


---

## Tech Stack

- Python (Flask)
- Prometheus
- Grafana
- Docker & Docker Compose

---

## Metrics

- **app_requests_total**  
  Counter metric tracking total HTTP requests served by the application

---

## Project Structure

.
├── app/
│ ├── app.py
│ └── Dockerfile
├── prometheus.yml
├── docker-compose.yml
└── README.md


---

## Run Locally

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
docker compose up --build
