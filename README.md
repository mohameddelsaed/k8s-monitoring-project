# 🚀 Kubernetes Monitoring Project

This project demonstrates deploying a full-stack application on Kubernetes with a complete monitoring setup using Prometheus and Grafana.

---

## 📦 Tech Stack

* Kubernetes
* Docker
* Node.js
* PostgreSQL
* Prometheus
* Grafana
* node-exporter
* kube-state-metrics

---

## ⚙️ Features

* Deploy Node.js API using Kubernetes Deployment
* Expose services using Service and Ingress
* Use Persistent Volume for PostgreSQL
* Full monitoring setup:

  * CPU / Memory usage
  * Pods & Deployments status
  * Node metrics
* Custom Grafana dashboards

---

## 📊 Monitoring

This project includes a complete monitoring stack:

* Prometheus for metrics collection
* Grafana for visualization
* node-exporter for node metrics
* kube-state-metrics for Kubernetes objects

---

## 📁 Project Structure

```
k8s/
├── app-deployment.yaml
├── app-service.yaml
├── ingress.yaml
├── config.yaml
├── secret.yaml
├── postgres/
└── monitoring/
```

---

## 🚀 Run Locally

```bash
minikube start
kubectl apply -f k8s/
```

---


---

## 👨‍💻 Author

Mohamed
