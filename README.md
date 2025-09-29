📖 Overview

This project demonstrates a Continuous Integration / Continuous Deployment (CI/CD) pipeline using GitHub Actions for a sample Python application. The pipeline automatically runs tests, builds the application, and ensures reliable deployments whenever changes are pushed to the repository.

🎯 Objectives

Automate testing with pytest

Build and validate application on every commit

Demonstrate CI/CD fundamentals for DevOps practice

Provide a foundation to extend into Docker, Kubernetes, or Cloud deployments

⚙️ Tech Stack

Language: Python

Version Control: Git & GitHub

CI/CD Tool: GitHub Actions

Testing: Pytest

Environment: Ubuntu (GitHub-hosted runner)

🛠️ Features

✅ Automated testing pipeline triggered on push & pull requests

✅ Dependency installation & build verification

✅ Easy-to-extend workflow for deployments (Docker, AWS, etc.)

✅ Example configuration for Python projects 

📂 Repository Structure

ci-cd-demo/
│── app.py              # Sample Python application
│── test_app.py         # Unit tests with pytest
│── requirements.txt    # Python dependencies
│── .github/workflows/
│    └── ci-cd.yml      # GitHub Actions workflow
└── README.md           # Project documentation

🚀 Getting Started

1. Clone Repository

git clone https://github.com/<NimishaPatel-21>/ci-cd-demo.git
cd ci-cd-demo

3. Install Dependencies

pip install -r requirements.txt

5. Run Tests Locally

pytest

7. GitHub Actions Workflow

The pipeline is defined in .github/workflows/ci-cd.yml. It runs automatically on:

Push to main branch

Pull requests targeting main

🔄 Workflow Diagram
flowchart TD
    A[Push Code to GitHub] --> B[GitHub Actions Trigger]
    B --> C[Checkout Code]
    C --> D[Install Dependencies]
    D --> E[Run Tests with Pytest]
    E --> F{Tests Pass?}
    F -- Yes --> G[Build Successful]
    F -- No --> H[Fail Pipeline]

📌 Future Improvements
Add Docker containerization and push image to DockerHub

Deploy to AWS EC2 / S3 or Azure App Services

Implement Kubernetes deployment in next iteration

👤 Author

Nimisha Patel – Aspiring DevOps Engineer | Open to Internships
