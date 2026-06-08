# Assignment 3: Kubernetes Orchestration & Full DevOps Pipeline

## Overview
3-tier microservice application: Nginx -> Flask API -> MySQL

## Quick Start
```bash
./start.sh
```

## Architecture
- **Nginx**: Reverse proxy (NodePort 30080)
- **Flask API**: REST API backend (ClusterIP 5000)
- **MySQL**: Database with persistent storage (ClusterIP 3306)

## GitHub Actions
CI/CD pipeline auto-builds and pushes Docker images to DockerHub on push to main.

## DockerHub Images
- zoekhann/flask-api:latest
- zoekhann/nginx-proxy:latest
