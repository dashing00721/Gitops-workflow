# Gitops Workflow Project

A lightweight Flask API service with an automated CI/CD pipeline 
using GitHub Actions and GitOps principles.

## Project Overview
This project demonstrates an automated development workflow connecting
Trello for task tracking, GitHub for source control, and GitHub Actions
for automated testing and linting.

## API Endpoints
- GET /health - returns service status
- POST /sum - adds two numbers together
- POST /reverse-string - reverses a string

## CI Pipeline
1. Install dependencies
2. Lint code with flake8
3. Run tests with pytest

## Commit Convention
[TRELLO-###] Short description

## Setup Instructions
1. Clone the repo
2. Create virtual environment: python3 -m venv venv
3. Activate it: source venv/bin/activate
4. Install dependencies: pip install -r requirements.txt
5. Run tests: pytest test_app.py -v
