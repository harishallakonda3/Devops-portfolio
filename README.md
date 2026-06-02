# Harish Kumar Allakonda — DevOps Portfolio

📍 Hyderabad, India
📧 [harishallakonda3@gmail.com](mailto:harishallakonda3@gmail.com)
📞 +91-7569992623
🔗 [LinkedIn](https://linkedin.com/in/harishkumarofficial)
🐙 [GitHub](https://github.com/harishallakonda3)

---

## Professional Summary

Cloud & DevOps Engineer with **2.5+ years** owning production AWS infrastructure across **24 EKS clusters** serving **200K+ daily users** on enterprise communication platforms at scale. Drove an **87% reduction** in security compliance findings and cut incident MTTR from hours to **under 30 minutes** through automated monitoring and alerting.

---

## Certifications

| Badge | Certification | Year |
|---|---|---|
| [![AWS SAA](https://img.shields.io/badge/AWS-Solutions_Architect_Associate-FF9900?logo=amazonaws&logoColor=white)](https://www.credly.com/badges/87eb74c1-0ac5-4386-abb1-1ce1ea753eb6) | AWS Certified Solutions Architect — Associate | 2026 |
| [![AWS CCP](https://img.shields.io/badge/AWS-Cloud_Practitioner-FF9900?logo=amazonaws&logoColor=white)](https://www.credly.com/badges/1a647154-5ad6-4dea-acfd-64209fdd2a18) | AWS Certified Cloud Practitioner | 2025 |

---

## Technical Skills

| Area | Tools & Technologies |
|---|---|
| **Cloud & Infra** | AWS — EKS, EC2, VPC, S3, IAM, EFS, RDS, ElastiCache, Route53, CloudFormation |
| **Containers** | Kubernetes, Docker, Helm Charts, Karpenter, HPA, Linkerd Service Mesh |
| **IaC & CI/CD** | Ansible, Terraform, CloudFormation, Jenkins, Bash, Python, Git |
| **Monitoring** | Splunk, Grafana, Prometheus, OpenTelemetry (Alloy), CloudWatch |
| **Networking** | TCP/IP, DNS, TLS/mTLS, VPC Endpoints, GSLB, PCI Compliance |
| **Languages** | Java, Spring Boot, Python, SQL |

---

## Experience

### DevOps Engineer — Client: Apple Inc.
**Cognizant Technology Solutions** | Hyderabad, India | *Dec 2023 – Present*

#### Platform Architecture & Infrastructure
- Architected and operated 3 enterprise communication platforms spanning **24 EKS clusters** (6 AWS regions) and **100+ EC2 hosts**, maintaining **99.9% uptime** across all production workloads
- Spearheaded **2 new APAC region buildouts** end-to-end — provisioned VPCs, configured IAM via CloudFormation, stood up EKS clusters, and integrated all services — delivering production-ready infrastructure **within 1 week per region**
- Implemented **Karpenter autoscaler** with custom NodePools and HPA policies, eliminating idle compute spend by removing manual node scaling across 24 clusters

#### Kubernetes & Application Deployment
- Orchestrated **20+ microservices per cluster** via Helm charts with Linkerd service mesh, achieving 99.9% pod availability and **zero unplanned downtime** during 6 major version upgrades
- Engineered zero-downtime rolling upgrade runbooks coordinating Helm value changes, container image promotions, and EFS content sync — executed across all 24 clusters with **zero rollbacks**
- Hardened PCI-compliant container security: enforced approved registry whitelisting, TLS-only middleware, and mTLS on all management interfaces — **passed all quarterly compliance audits**

#### Monitoring, Alerting & Incident Response
- Built **15+ Splunk dashboards** and Grafana panels tracking real-time pod health, session concurrency, and middleware throughput — adopted as primary observability layer by L1/L2 operations team
- Identified silently degraded pods responsible for **23% of platform timeouts** using custom per-pod anomaly detection, resolving a systemic issue that had persisted undetected for weeks
- Authored production incident SOPs adopted by L1/L2 support, standardizing triage workflows for all alert types across 3 platform components

#### Infrastructure Automation, CI/CD & Security
- Automated EC2 provisioning via CloudFormation and Terraform (IAM roles, instance profiles, S3 policies), eliminating **2+ hours of manual setup per host** across 100+ instances
- Drove quarterly OS and application patching via Ansible across 100+ middleware hosts, reducing open security compliance findings from **150 → 20 (87% reduction)**
- Built Jenkins CI/CD pipelines with container image scanning, approval gates, and automated deployment — reducing release cycle from **1 day → 45 minutes**
- Enforced TLS/mTLS across all inter-service communication — RabbitMQ, PostgreSQL, Redis, DNS health checks, and full certificate lifecycle management

#### Application Development & Collaboration
- Developed internal APIs using **Java and Spring Boot** for centralized configuration management, saving **5+ hours/week** of operational overhead
- Led P1 incident bridges across **US, EMEA, and APAC** time zones, coordinating vendor engineering, internal dev teams, and L1/L2 support to drive root cause resolution within SLA

---

## Projects

### EC2 Kernel Patching Automation — Ansible
> **Tools:** Ansible, AWS EC2, Ansible EDA (Event-Driven Ansible), Systemd

Multi-play Ansible orchestrator for zero-downtime kernel patching across 100+ EC2 middleware hosts.
- Webhook-triggered via Ansible EDA with `target_group` label routing (`APP.ENV.REGION.BU`)
- 3-play workflow: pre-patch validation → kernel upgrade → post-patch verification with automated rollback
- EBS volume validation by device mapping, real-time streaming logs, single consolidated `ansible.log`
- Reduced patching cycle from manual multi-hour effort to **fully automated < 30 min per batch**

---

### APAC Region Buildout — EKS + LumenVox STT
> **Tools:** AWS EKS, CloudFormation, Helm, Kubernetes, RabbitMQ, PostgreSQL, GSLB, mTLS

End-to-end production buildout for new APAC speech processing clusters (Singapore + Tokyo).
- Provisioned VPCs, IAM roles, and EKS clusters via CloudFormation from scratch
- Deployed LumenVox STT engine via Helm with Karpenter autoscaling (24+ replicas per service)
- Configured RabbitMQ with mTLS, GSLB health checks (`*.g.apple.com`), and Prometheus metrics
- Integrated Alloy-based observability pipeline to Grafana for real-time concurrency tracking

---

### Unified Observability Platform — Splunk + Grafana
> **Tools:** Splunk, Grafana, Prometheus, OpenTelemetry (Alloy), Kubernetes

Designed and built the primary monitoring layer for 3 enterprise IVR/STT platforms.
- 15+ Splunk dashboards covering SIP/DTMF metrics, ASR failure rates, call volumes by region
- Custom per-pod anomaly detection identifying barge-in ratio degradation (30-min rolling window)
- Grafana panels for real-time EKS pod health, session concurrency, and middleware throughput
- Adopted as the standard observability tool by L1/L2 operations teams

---

### Jenkins CI/CD Pipeline — Container Delivery
> **Tools:** Jenkins, Docker, Kubernetes, Helm, GitHub

End-to-end CI/CD pipeline for containerized application delivery to Kubernetes clusters.
- Container image scanning and vulnerability gating pre-deployment
- Automated Helm value promotion across dev → staging → prod
- Approval gates for production releases with audit logging
- Reduced release cycle from **1 day manual → 45 minutes automated**

---

## Education

| Degree | Institution | Year | Score |
|---|---|---|---|
| B.Tech, Computer Science & Engineering | Jawaharlal Nehru Technological University, Hyderabad | 2020 – 2023 | CGPA: 7.69 |
| Diploma, Mining Engineering | State Board of Technical Education (SBTET), Hyderabad | 2017 – 2020 | 77.83% |

---

## Career Interests

Cloud Infrastructure & Platform Engineering · Kubernetes & Container Platforms · CI/CD & Automation · Site Reliability Engineering (SRE) · Cloud Security & Scalability · Observability Engineering
