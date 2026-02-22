# kubernetes-production-deployment
Production-ready containerized application deployment on Kubernetes using Docker, Helm, and AWS infrastructure, with automated scaling, monitoring using Prometheus and Grafana, and high-availability deployment strategies.

# Kubernetes Production Deployment with Monitoring

## Architecture

This project demonstrates production-grade Kubernetes deployment including:

- Dockerized Flask application
- Kubernetes deployment with probes and resource limits
- Horizontal Pod Autoscaler
- Helm packaging
- Prometheus and Grafana monitoring stack

## Features
- Dockerized application
- Kubernetes deployment
- Helm packaging
- Horizontal Pod Autoscaler
- Prometheus monitoring
- Grafana dashboards

## Run Steps

### Build image
docker build -t <username>/devops-k8s-app:v1 .

### Deploy
kubectl apply -f k8s/

### Install monitoring
helm install prometheus prometheus-community/prometheus
helm install grafana prometheus-community/grafana

