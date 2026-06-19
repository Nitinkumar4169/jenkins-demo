# jenkins-demo
# 🚀 Jenkins CI/CD Demo Project

## 📌 Project Overview

This project demonstrates a basic **CI/CD pipeline using Jenkins**, integrated with **GitHub and Python**, running inside a **Docker-based Jenkins setup on AWS EC2**.

The goal of this project is to understand how modern DevOps pipelines work, starting from source code management to automated execution using Jenkins.

---

## 🎯 Purpose of This Project

This project was created to:

- Learn **Jenkins CI/CD fundamentals**
- Understand **Pipeline as Code using Jenkinsfile**
- Practice **GitHub + Jenkins integration**
- Execute **automated builds and runs using Python**
- Set up Jenkins in a **Docker container on AWS EC2**
- Simulate a real-world DevOps workflow

---

## ⚙️ Technologies Used

- Jenkins (CI/CD tool)
- Docker (containerized Jenkins setup)
- Git & GitHub (source code management)
- Ubuntu (AWS EC2 instance)
- Python 3 (application runtime)

---

## 🏗️ Project Structure
jenkins-demo/
│
├── app.py # Simple Python application
├── Jenkinsfile # CI/CD pipeline definition
└── README.md # Project documentation
---

## 🐍 Application Description

### `app.py`
A simple Python script used to demonstrate pipeline execution.

Webhook Test - June 19, 2026

```python
print("Hello from Jenkins")

This confirms that Jenkins is successfully executing code pulled from GitHub.

🔄 CI/CD Pipeline Flow

The Jenkins pipeline follows this workflow:

GitHub Repository
        ↓
Jenkins (Docker on EC2)
        ↓
Checkout Source Code
        ↓
Install Dependencies (pip)
        ↓
Run Python Application
        ↓
Display Output in Jenkins Console
⚙️ Jenkinsfile Explanation

The pipeline is defined using a Jenkinsfile, which contains the CI/CD stages:

Stages:
Checkout → Pull code from GitHub
Install Dependencies → Install Python packages (if any)
Run App → Execute Python script
🚀 Sample Jenkinsfile
🧠 Key Learnings

Through this project, the following concepts were learned:

Jenkins installation and setup on EC2
Running Jenkins inside Docker container
Creating freestyle and pipeline jobs
Writing Jenkinsfile (Pipeline as Code)
GitHub integration with Jenkins
Understanding CI/CD workflow
Handling Python execution inside Jenkins environment
⚠️ Known Issue (Learning Insight)

While installing Python dependencies inside Jenkins container, a PEP 668 externally managed environment error was encountered.

This is expected in modern Python environments and can be solved using:

Virtual environments (venv)
Docker-based build agents (recommended for production)
📈 Future Improvements

This project can be extended with:

✔ GitHub Webhooks (auto-trigger pipeline)

✔ PyInstaller build (create executable)
✔ Pytest integration (automated testing)
✔ Dockerized application deployment
✔ Kubernetes deployment pipeline
✔ Production-grade CI/CD workflow
👨‍💻 Author

Nitin Kumar

Learning DevOps | CI/CD | Jenkins | AWS | Docker

📌 Summary

This project is a beginner-friendly implementation of a CI/CD pipeline using Jenkins, designed to understand how code moves from GitHub to automated execution using Jenkins pipelines.
