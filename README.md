# 🚀 DevSecOps CI/CD Pipeline with Kubernetes Monitoring

A complete end-to-end DevSecOps project demonstrating Continuous Integration, Continuous Delivery, Security Scanning, Containerization, Kubernetes Deployment and Monitoring using industry tools.

This project builds a Java Spring Boot application (BoardGame App), scans it for vulnerabilities, containerizes it, pushes it to DockerHub, deploys into Kubernetes and monitors using Prometheus + Grafana + Blackbox Exporter.

---

## 🧠 Project Architecture

Developer → GitHub → Jenkins Pipeline → SonarQube → Trivy → Nexus → DockerHub → Kubernetes → Prometheus → Grafana

---

## 🛠️ Tools & Technologies Used

| Category | Tools |
|--------|------|
| CI/CD | Jenkins |
| Build Tool | Maven |
| Code Quality | SonarQube |
| Security Scan | Trivy |
| Artifact Repo | Nexus |
| Containerization | Docker |
| Orchestration | Kubernetes (kubeadm cluster) |
| Monitoring | Prometheus + Grafana |
| Probing | Blackbox Exporter |
| Metrics | Node Exporter |
| Cloud | AWS EC2 |
| Language | Java (Spring Boot) |

---

## ⚙️ Pipeline Stages

1. Git Checkout
2. Maven Compile & Test
3. File System Vulnerability Scan (Trivy)
4. SonarQube Code Analysis
5. Quality Gate Validation
6. Package Build
7. Publish Artifact to Nexus
8. Build Docker Image
9. Docker Image Vulnerability Scan
10. Push Image to DockerHub
11. Deploy to Kubernetes
12. Verify Deployment
13. Email Notification

---

## 🔐 Security Implementations

- Static Code Analysis using SonarQube
- Dependency Vulnerability Scan using Trivy
- Container Image Scan using Trivy
- Kubernetes RBAC Authentication (Jenkins ServiceAccount)
- Quality Gate enforcement before deployment

---

## ☸️ Kubernetes Deployment

Application deployed as:
- Deployment (2 replicas)
- Service (LoadBalancer / NodePort)

kubectl get pods -n webapps
kubectl get svc -n webapps

---

## 📊 Monitoring Setup

| Component | Purpose |
|--------|------|
| Node Exporter | Server metrics (CPU, RAM, Disk) |
| Prometheus | Metrics collection |
| Grafana | Visualization dashboards |
| Blackbox Exporter | Endpoint uptime monitoring |
| Jenkins Metrics | CI/CD monitoring |

---

## 📈 Grafana Dashboards

- Node Exporter Full Dashboard
- Blackbox HTTP Probe Dashboard
- Jenkins Metrics Dashboard

---

## 📁 Project Structure

.
├── app/ # Spring Boot Application
├── docker/ # Dockerfile
├── kubernetes/ # Deployment & Service YAML
├── jenkins/ # Jenkins pipeline config
├── sonar/ # Sonar properties
├── screenshots/ # Project output screenshots
├── Jenkinsfile
└── README.md
---

## 🧪 How to Run (High Level)

1. Create 4 AWS EC2 Instances
2. Setup Kubernetes cluster using kubeadm
3. Install Jenkins, SonarQube, Nexus, Docker
4. Configure Jenkins credentials
5. Run Jenkins pipeline
6. Access application via LoadBalancer
7. Monitor using Grafana

---

## 📸 Screenshots

Screenshots available inside `/screenshots` folder showing:

- Jenkins Pipeline Success
- SonarQube Quality Gate
- Trivy Scan Report
- DockerHub Image
- Kubernetes Pods
- Prometheus Targets
- Grafana Dashboards

---

## 👨‍💻 Author

**Darshan S P**
DevSecOps & Cloud Enthusiast

---
## ⭐ Project Goal

To demonstrate real-time industry level DevSecOps workflow from code commit to monitored production deployment.

---

## 📌 Conclusion

This project simulates a production-grade DevSecOps pipeline implementing automation, security and observability across the software delivery lifecycle.
