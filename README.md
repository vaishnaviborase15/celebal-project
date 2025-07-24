# 🏦 Spring Bank Web Application – CI/CD Deployment

## 🔰 Overview

The **Spring Bank Web Application** is a Java-based **Spring MVC + Maven project** designed to demonstrate a secure and modular online banking system. This application handles customer account management, transaction processing, and service requests while adhering to industry-standard practices.

The project is containerized using **Docker** and deployed to **Azure App Service** using an automated **CI/CD pipeline with GitHub Actions**. It ensures seamless integration, testing, and deployment for enterprise-grade environments.

---

## 🚀 Project Objective

> “To build and deploy a secure, scalable banking web application using **Spring MVC**, **Maven**, and **Tomcat**, leveraging **Azure App Service** and **GitHub Actions** for a fully automated CI/CD pipeline.”

---

## 🧩 Architecture Design

### 🔸 Application Features
- **Customer Account Management** – Create, view, and manage accounts.
- **Transactions** – Fund transfers, deposits, and withdrawals.
- **Admin Dashboard** – Manage customers and transactions securely.
- **Spring MVC Framework** – Implements the Model-View-Controller pattern.
- **MySQL Database Integration** – For persistent data storage.
- **REST Endpoints** – Secure API endpoints for integration with external services.

### 🔸 CI/CD Workflow

| Phase | Description |
|-------|-------------|
| **Build Phase** | Maven compiles and packages the WAR file. |
| **Containerization** | Docker builds the image using Tomcat. |
| **CI Phase** | GitHub Actions runs tests and pushes Docker image to GitHub Container Registry. |
| **CD Phase** | Azure Web App pulls the latest image and deploys automatically. |

---

## ⚙️ Technologies Used

- **Backend**: Java 17, Spring MVC, Maven  
- **Web Server**: Apache Tomcat 9 (Dockerized)  
- **Frontend**: JSP, HTML5, CSS3, Bootstrap  
- **Database**: MySQL (XAMPP / Azure MySQL)  
- **Cloud & CI/CD**: Azure Web App, GitHub Actions, Docker  
- **Version Control**: Git & GitHub  

---

## 📋 Prerequisites

- **Java 17+**  
- **Apache Maven 3.8+**  
- **Docker Desktop**  
- **Azure Subscription**  
- **GitHub Account**  
- **Basic knowledge of Git, Maven build lifecycle, and Azure Web Apps.**

---

## 📐 Implementation Stages

### ✅ Stage 1: Project Setup
- Developed the **Spring Bank** Maven project in Eclipse IDE.
- Configured `pom.xml` for WAR packaging.
- Set up `web.xml` and JSP pages for user interfaces.
- Connected to MySQL database for account transactions.

### ✅ Stage 2: Containerization
- Added a **Dockerfile**:
  - Uses `maven:3.9.6` for building the WAR.
  - Uses `tomcat:9-jdk17` for running the application.
- Built and tested the Docker image locally.

### ✅ Stage 3: GitHub Repository
- Created a GitHub repository.
- Configured `.gitignore` for Maven artifacts (`target/`).
- Pushed source code and Dockerfile to GitHub.

### ✅ Stage 4: CI/CD Pipeline
- Created a **GitHub Actions YAML workflow** to:
  - Build and test the Maven project.
  - Build and push the Docker image to GitHub Container Registry.
  - Deploy the image to Azure App Service.

### ✅ Stage 5: Deployment
- Configured an **Azure Web App (Linux)** instance.
- Pulled the latest Docker image from GitHub Container Registry.
- Verified application availability via `https://<appname>.azurewebsites.net`.

---

## 🛠️ How to Run

### **Local Build**
```bash
mvn clean package
```

## **Local Docker Build**
```bash
docker build -t spring-bank-web .
docker run -p 8080:8080 spring-bank-web
```
Visit: http://localhost:8080


## **Azure Deployment via GitHub Actions**
Push code to the `main` branch.

GitHub Actions automatically builds, tests, and deploys the app.

Access the live app on https://<your-azure-web-app>.azurewebsites.net.

---

## **🧪 Testing and Validation**
- Verified account creation and transaction flows.
- Performed integration tests on database connections.
- CI pipeline runs unit tests on every push.
- Confirmed deployment through Azure Web App logs and monitoring.

---

## **📊 Monitoring & Logs**
- Azure App Service Log Stream for real-time logs.
- Azure Monitor for application insights (performance & errors).
- Docker Logs for debugging container runtime issues.

---

## **✅ Outcome**
- Automated CI/CD with zero manual deployments.
- Scalable architecture ready for enterprise banking solutions.
- Cloud-native deployment using Azure Web App and GitHub Actions.
- Containerized application ensuring consistency across environments.

---

## **📚 References**
- Spring MVC Framework – Official Docs
- GitHub Actions for CI/CD
- Deploy Java Apps to Azure Web App
- Dockerizing Java Web Applications

---

## 🏁 Author

**Vaishnavi Sunil Borase**  
Celebal Summer Internship | DevOps | CT_CSI_DV_4845
Email: vaishnaviborse.clg@gmail.com
GitHub: https://github.com/vaishnaviborase15
