# End-to-End CI/CD Pipeline with Monitoring on AWS

This project demonstrates a complete DevOps CI/CD pipeline using:

- Jenkins
- Docker
- Node.js
- Prometheus
- Grafana
- AWS EC2

## Features

- Automated CI/CD pipeline using Jenkins
- Docker container deployment
- Node.js sample application
- Prometheus monitoring
- Grafana dashboards
- Node Exporter metrics

## Tech Stack

- AWS EC2
- Ubuntu
- Jenkins
- Docker
- GitHub
- Prometheus
- Grafana

## Ports Used

- 8080 → Jenkins
- 3000 → Node.js App
- 9090 → Prometheus
- 3001 → Grafana
- 9100 → Node Exporter

## Pipeline Flow

GitHub → Jenkins → Docker Build → Container Deployment

## Monitoring

Prometheus collects metrics from:
- Node Exporter
- Docker containers

Grafana visualizes:
- CPU Usage
- Memory Usage
- Disk Usage
- Network Usage

## Author

Anjali Somwanshi# nodejs-cicd-app
