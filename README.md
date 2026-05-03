#  Kubernetes Monitoring Stack with Node.js API

## 📌 Project Overview

This project demonstrates a complete Kubernetes-based application deployment with a full monitoring and observability stack.

It includes a containerized Node.js REST API, a PostgreSQL database with persistent storage, and a monitoring system powered by Prometheus and Grafana.

The goal is to simulate a production-like DevOps environment locally using Minikube.

---

## 🏗️ Architecture

* Node.js API (Deployment)
* PostgreSQL (Persistent Volume)
* Kubernetes Resources:

  * Deployment
  * Service
  * Ingress
  * ConfigMap
  * Secret
* Monitoring Stack:

  * Prometheus
  * Grafana
  * node-exporter
  * kube-state-metrics

### 🔄 Request Flow

```
User → Ingress → Service → API → PostgreSQL
                         ↓
                   Prometheus → Grafana
```

---

## 🛠️ Tech Stack

* Node.js
* Docker
* Kubernetes (Minikube)
* PostgreSQL
* Prometheus
* Grafana

---

## ⚡ Features

* Containerized application
* Kubernetes-based deployment
* Persistent storage (PV/PVC)
* ConfigMap & Secret usage
* Ingress routing
* Real-time monitoring dashboards

---

## 📊 Monitoring & Observability

The system provides:

* Total / Running Pods
* Node count
* CPU, Memory, Disk usage
* Network traffic
* Top pods by resource usage

---

## 📸 Screenshots

### 📊 Grafana Dashboard

![Grafana](assets/screenshots/grafana-dashboard.png)

---

### 📈 Node Metrics

![Node Metrics](assets/screenshots/node-metrics.png)


---

## 📁 Project Structure

```
project-devops/
├── k8s/
├── monitoring/
├── assets/screenshots/
├── Dockerfile
└── README.md
```

---

## 🚀 How to Run

```bash
minikube start
minikube addons enable ingress
docker build -t project-api:latest .
kubectl apply -f k8s/
kubectl apply -f monitoring/
kubectl port-forward svc/grafana 3000:3000
```



---

## 💡 Key Takeaways

* Hands-on Kubernetes deployment
* Built monitoring system using Prometheus & Grafana
* Simulated production-like DevOps environment

