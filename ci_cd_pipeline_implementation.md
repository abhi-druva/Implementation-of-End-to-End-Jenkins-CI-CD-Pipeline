# Implementation of End-to-End Jenkins CI/CD Pipeline

This project demonstrates the implementation of a complete CI/CD pipeline to automate the deployment of a blogging application on an Amazon EKS cluster. It uses **Git** for source code management, **Jenkins** for orchestrating the pipeline, **Maven** for building and compiling code, **SonarQube** for code quality analysis, and **Trivy** for vulnerability scanning. **Docker** is used to containerize the application, with **Docker Hub** serving as the image registry. The final deployment is done on **EKS**, with **Prometheus** and **Grafana** integrated for monitoring and visualization.

---

## Project Stages

### Stage 1: Infrastructure Setup

- Provisioned a custom **VPC** and launched **EC2 instances** to host the CI/CD tools (Jenkins, SonarQube, Trivy, etc.).
- Ensured proper **security group configurations** and **IAM roles** for smooth operations.

### Stage 2: Source Code Management

- Created a **Git repository** to manage and version-control the blogging application’s source code.
- Implemented **branch strategies** to streamline feature integration and deployment.

### Stage 3: CI/CD Pipeline

- Used **Jenkins** to configure and automate the pipeline.
- Compiled the code using Maven.
- Integrated **SonarQube** for static code analysis and **Trivy** for container vulnerability scanning.
- Used **Trivy** for vulnerabilities scan.
- **Maven** compiles and builds the Java-based application.
- Artifacts are stored in **Nexus** Repository.
- **Docker** containers are built and pushed to **Docker Hub**.
- Deployed the final application to Amazon EKS cluster.

### Stage 4: Monitoring & Alerting

- Set up **Prometheus** to scrape metrics from the application and infrastructure.
- Configured **Grafana dashboards** for real-time monitoring and visualization.

## Tools & Technologies Used

| Category               | Tools/Services          |
| ---------------------- | ----------------------- |
| Source Control         | Git                     |
| CI/CD                  | Jenkins                 |
| Build Tool             | Maven                   |
| Code Quality           | SonarQube               |
| Vulnerability Scanning | Trivy                   |
| Containerization       | Docker                  |
| Image Registry         | Docker Hub              |
| Orchestration          | Amazon EKS (Kubernetes) |
| Monitoring             | Prometheus, Grafana     |

---

## Author

Abhimanyu KS\
DevOps Engineer
