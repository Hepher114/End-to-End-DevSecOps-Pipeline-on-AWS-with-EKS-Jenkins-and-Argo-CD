# End-to-End-DevSecOps-Pipeline-on-AWS-with-EKS-Jenkins-and-Argo-CD
This repository documents a complete **DevSecOps** workflow that provisions infrastructure on AWS, builds and scans code, pushes container images to ECR, and deploys a **three-tier application** (Frontend + Backend + Database) on **Amazon EKS** using **Argo CD GitOps**. The platform also includes **Prometheus + Grafana** for cluster monitoring.

## Tech Stack
**Cloud / Infra**
- AWS (EC2, IAM, S3, DynamoDB, ECR, EKS)
- Terraform (remote state: S3 + DynamoDB)

**CI / Security**
- Jenkins (CI pipelines)
- SonarQube (static analysis + quality gate via webhook)
- OWASP Dependency-Check (dependency vulnerability scan)

**CD / GitOps**
- Argo CD (deploy manifests from Git)

**Observability**
- Prometheus
- Grafana

**App**
- Frontend: React
- Backend: Django REST API (Python)
- Database: PostgreSQL
- Kubernetes Ingress: AWS Load Balancer Controller (ALB)
