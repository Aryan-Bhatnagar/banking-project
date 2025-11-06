# 💼 FinanceMe – Banking & Finance DevOps Automation Project

### 👤 Author: [Aryan Bhatnagar](https://www.linkedin.com/in/aryan-bhatnagar-0146b1170/)
📍 Chandigarh, India | ✉️ aryanmain69@gmail.com | ☁️ [GitHub Repo](https://github.com/Aryan-Bhatnagar/banking-project)

---

## 🚀 Project Overview
**FinanceMe** is a full-scale **DevOps automation project** that demonstrates complete CI/CD implementation, infrastructure provisioning, and monitoring using modern DevOps tools.

It automates everything from infrastructure creation to deployment and monitoring of a cloud-hosted web application — simulating a **real banking/finance system**.

---

## 🏗️ Architecture Summary

| Layer | Tool | Purpose |
|--------|------|----------|
| Infrastructure as Code | **Terraform** | Automates creation of AWS EC2 instances & networking |
| Configuration Management | **Ansible** | Installs & configures Jenkins, Docker, required dependencies |
| CI/CD Pipeline | **Jenkins** | Automates build, test, Docker image creation, and deployment |
| Containerization | **Docker** | Packages app for consistent deployment |
| Monitoring | **Prometheus + Grafana** | Tracks VM and pipeline health metrics |
| Version Control | **Git & GitHub** | Source control and pipeline trigger |

---

## 🧩 Project Phases

### 🟩 Phase 1: Infrastructure Automation
- Created AWS EC2 instances using **Terraform**.  
- Configured servers with **Ansible playbooks** to install Jenkins, Docker, and dependencies.  
- Automated provisioning of Master, Slave, and Production nodes.

### 🟨 Phase 2: Build and Deployment Automation
- Configured **Jenkins Master (VM1)** to trigger pipeline jobs.  
- **Slave Node (VM2)** compiles source code, builds Docker images, and pushes to **Docker Hub**.  
- **Production Node (VM3)** pulls the Docker image and runs the application container.  
- Used **Maven** for build management and **GitHub Webhooks** for CI trigger.

### 🟦 Phase 3: Continuous Monitoring
- Integrated **Prometheus & Grafana** on a monitoring node (**VM4**).  
- Tracked real-time resource usage, job success, and system health.  
- Created custom dashboards for visual insights.

---

## ⚙️ Technologies Used

| Category | Tools |
|-----------|-------|
| Cloud | AWS EC2 |
| IaC | Terraform |
| Configuration | Ansible |
| CI/CD | Jenkins, Maven |
| Containers | Docker |
| Monitoring | Prometheus, Grafana |
| SCM | Git, GitHub |
| OS | Ubuntu, Linux |

---

## 🪜 How to Run Locally

1. **Clone this repository:**
   ```bash
   git clone https://github.com/Aryan-Bhatnagar/banking-project.git
   cd banking-project
