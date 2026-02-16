# 🚀 Production-Grade DevSecOps CI/CD Pipeline on Kubernetes

This project demonstrates a complete **end-to-end DevSecOps pipeline** used in real companies.

Whenever a developer pushes code, the system automatically:

✔ Builds application
✔ Runs tests
✔ Performs code quality analysis
✔ Runs security scans
✔ Publishes artifact
✔ Builds Docker image
✔ Pushes image to DockerHub
✔ Deploys to Kubernetes cluster
✔ Monitors using Prometheus & Grafana
✔ Sends email notification

No manual intervention required.

---

# 🧱 Tools & Technologies

| Category         | Tools                |
| ---------------- | -------------------- |
| Source Control   | GitHub               |
| CI/CD            | Jenkins              |
| Build Tool       | Maven + JDK17        |
| Code Analysis    | SonarQube            |
| Security Scan    | Trivy                |
| Artifact Repo    | Nexus                |
| Containerization | Docker               |
| Orchestration    | Kubernetes (kubeadm) |
| Monitoring       | Prometheus + Grafana |
| Alerts           | Email Notification   |

---

# 🔄 Pipeline Architecture

Developer → GitHub → Jenkins → SonarQube → Trivy → Nexus → DockerHub → Kubernetes → Monitoring → Email Alert

---

# 🏗 Jenkins Pipeline

![pipeline](screenshots/jenkins-stage-view.png)

---

# 🔍 SonarQube Quality Gate

![sonarqube](screenshots/sonarqube-quality-gate-passed.png)

---

# 🔐 Security Scan (Trivy)

![trivy](screenshots/trivyscanimage.png)

---

# 📦 Nexus Artifact Upload

![nexus](screenshots/nexus-artifact-uploaded.png)

---

# 🐳 Docker Image Build & Push

![docker](screenshots/docker-build.png)
![dockerhub](screenshots/dockerhub-image.png)

---

# ☸ Kubernetes Deployment

![pods](screenshots/kubernetes-pods-running.png)
![service](screenshots/kubernetes-service.png)

---

# 📈 Prometheus Monitoring

![prometheus](screenshots/prometheus-targets-up.png)

---

# 📊 Grafana Dashboard

![grafana](screenshots/grafana-node-exporter.png)

---

# 📧 Email Notification

![email](screenshots/jenkins-email-notification.png)

---

# 🧠 What This Project Demonstrates

• CI/CD automation
• DevSecOps practices
• Container orchestration
• Monitoring & observability
• Production-like deployment pipeline

---

# 🏁 Final Output

A developer pushes code → the system automatically delivers a secure production deployment.

---

# 👨‍💻 Author

**Darshan Patgar**
Aspiring DevOps & Cloud Engineer

