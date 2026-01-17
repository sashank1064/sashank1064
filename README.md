# Hi, I'm Sashank Allugunti 👋

DevOps & Site Reliability Engineer with **3.5+ years of experience** at **Greenhouse Software** and **IBM**, specializing in **cloud-native infrastructure**, **CI/CD automation**, **Docker** and **Kubernetes deployments** across **AWS and Azure**. Focused on reliability, deployment safety, and observability for customer-facing platforms.

---

## 🚀 Featured Project: RoboShop (3-Tier Microservices Deployment & Documentation)

RoboShop is a production-style, microservices-based e-commerce application deployed in a **3-tier architecture** with independent services, multiple databases, and message queues. This project highlights real-world DevOps responsibilities: installation, configuration, service management, runtime wiring, and operational runbooks.

<p align="center">
  <img src="images/roboshop.svg" alt="RoboShop 3-Tier Architecture" width="900"/>
</p>

> Designed and documented a production-grade microservices e-commerce platform,  
> focusing on service isolation, database integration, reverse proxy routing,  
> and systemd-based service management.

### What I Implemented and Documented
- Created structured deployment documentation for **multi-service application setup** including prerequisites, configs, and runbooks
- Deployed and configured databases and messaging components:
  - **MongoDB 7.x** (remote access enabled by binding `0.0.0.0`)
  - **Redis 7.x** (remote access + protected mode adjustments)
  - **MySQL 8.x** (secure installation + schema + app user setup)
  - **RabbitMQ 3.x** (repo config + service setup + app user & permissions)
- Installed and configured application runtimes and services:
  - **Node.js 20+** services (Catalogue, User, Cart)
  - **Java/Maven** service (Shipping)
  - **Python 3** service (Payment)
  - **GoLang** service (Dispatch)
- Managed microservices using **systemd**:
  - Dedicated non-root user (`roboshop`)
  - Environment variables for service-to-service connectivity (MongoDB, Redis, RabbitMQ, MySQL endpoints)
  - daemon reload, enable/start, and restart patterns for stable operations
- Configured **Nginx** as frontend + reverse proxy:
  - Served static UI
  - Routed API paths (`/api/catalogue`, `/api/user`, `/api/cart`, `/api/shipping`, `/api/payment`)
  - Added health endpoint for monitoring (`/health`)

### Services Overview
- **Frontend:** Nginx (static + reverse proxy)
- **Catalogue:** Node.js + MongoDB
- **User:** Node.js + MongoDB + Redis
- **Cart:** Node.js + Redis + Catalogue dependency
- **Shipping:** Java (Maven) + MySQL (schema + master data)
- **Payment:** Python (uWSGI) + RabbitMQ
- **Dispatch:** GoLang + RabbitMQ

### Why This Project Matters
- Multi-runtime services with real dependency wiring
- Process supervision using **systemd**
- Database initialization (schema + master data)
- Reverse proxy/API routing via **Nginx**
- Clear, reusable runbooks for repeatable environments

---

## Tech Stack

### Cloud & Infrastructure
- **AWS:** EC2, EKS, ECR, S3, VPC, IAM, ALB, Route 53, CloudWatch, CloudTrail, SNS  
- **Azure:** VMs, AKS, ACR, VNet, NSG, Load Balancer, Application Gateway, Azure DNS, Azure Monitor

### Containers & Orchestration
- Docker, Kubernetes, OpenShift, Helm

### CI/CD & Infrastructure as Code
- Jenkins, GitHub Actions, GitLab CI
- Terraform, Ansible, AWS CloudFormation

### Monitoring & Logging
- Prometheus, Grafana, ELK Stack (Elasticsearch, Logstash, Kibana), AWS CloudWatch

### Languages & Tools
- Python, Bash, PowerShell, SQL, C, C++, Java, C#
- Git, GitHub, Bitbucket

### Testing & Performance
- Postman, JMeter

### Platforms & OS
- Linux (RHEL/CentOS/Ubuntu), Systemd, Networking (DNS, TCP/IP, firewalls)

### Kubernetes Internals
- Pod lifecycle, Scheduling, Resource management, ConfigMaps, Secrets, Ingress Controllers
- Control plane fundamentals (API server, etcd, scheduler)

### Security & Access
- IAM and RBAC, Secrets management
- TLS/HTTPS fundamentals, Least-privilege access models

### Cloud Networking
- VPC design and subnetting
- Load balancing (ALB, NLB, Azure LB)
- Public/private networking patterns

---

## Key Traits
- Designed and automated **multi-environment CI/CD pipelines**, cutting release cycles **from hours to minutes**
- Containerized **legacy + microservices apps** on Docker and orchestrated them on **Kubernetes / EKS / AKS** to improve stability and availability
- Built **Terraform + Ansible** workflows for repeatable infrastructure provisioning and configuration across AWS/Azure
- Implemented observability stacks (**Prometheus/Grafana/ELK/CloudWatch**) to improve incident detection and reduce MTTR

---

## Education
- **M.S. in Computer Science**, Pace University, New York (2025)  
- **B.E. in Computer Science and Engineering**, BMS Institute of Technology and Management (2022)

---

## Certifications
- Microsoft Certified **Azure Data Scientist Associate**
- Python Programming
- Infrastructure Expert — algoexpert.io

---

## 📫 Contact
- Email: **sashankallugunti@gmail.com**
- Alternate: **sashanksai1064@gmail.com**
- LinkedIn: **https://www.linkedin.com/in/sashanksai1064/**


