# SIT223 Jenkins CI/CD Pipeline — Part 1 Task 1

This repository contains the Jenkins pipeline script for the **SIT223 Credit Task**.

## Pipeline Overview

A 7-stage theoretical CI/CD pipeline that demonstrates the full software delivery lifecycle:

| Stage | Task | Tool |
|-------|------|------|
| 1️⃣ Build | Compile and package the application | Maven |
| 2️⃣ Unit and Integration Tests | Run unit and integration tests | JUnit, Selenium |
| 3️⃣ Code Analysis | Static code analysis | Checkstyle |
| 4️⃣ Security Scan | Identify vulnerabilities | OWASP Dependency-Check |
| 5️⃣ Deploy to Staging | Deploy to staging environment | AWS Elastic Beanstalk |
| 6️⃣ Integration Tests on Staging | End-to-end testing | Selenium WebDriver |
| 7️⃣ Deploy to Production | Deploy to production | AWS CodeDeploy |

## GitHub Integration

This repo is connected to a Jenkins pipeline job that automatically triggers a new build whenever changes are pushed to the `main` branch.

Student: Harshman Kaur | SIT223 — Credit Task 8.1C
test
