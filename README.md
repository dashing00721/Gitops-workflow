# Gitops Workflow Project

A lightweight Flask API with automated CI/CD using GitHub Actions.

## API Endpoints
- GET /health - returns service status
- POST /sum - adds two numbers
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

## Reflection Questions

### 1. What is GitOps and why is it useful?
GitOps is a way of managing software development where Git is the 
single source of truth for everything. Instead of making changes 
directly to a server, all changes go through Git first. This is 
useful because every change is tracked, you can see who did what 
and when, and you can always go back to a previous version if 
something breaks. It makes teamwork easier because everyone follows 
the same process and nothing gets changed without a record of it.

### 2. Why do we use feature branches instead of pushing to main?
Feature branches keep the main branch clean and stable. If everyone 
pushed directly to main, broken code could affect the whole team. 
With feature branches, each developer works on their own copy of 
the code. When they are done, they open a pull request which lets 
others review the code before it goes into main. This means main 
always has working code and mistakes are caught before they cause 
problems for everyone.

### 3. What happens when CI fails?
When CI fails it means either the linting or the tests found a 
problem with the code. GitHub Actions shows a red X and the pull 
request cannot be merged until the problem is fixed. The developer 
must read the error message in the Actions tab, fix the problem 
locally, and push the fix to the same branch. CI will run again 
automatically and if it passes the pull request can be merged. This 
stops broken code from ever reaching the main branch.

### 4. How does Trello connect to Git in this workflow?
Every Trello card represents a task. When a developer starts working 
on a task they create a branch named after the Trello card ID for 
example feature/TRELLO-001-setup-ci. Every commit message also 
includes the Trello ID like [TRELLO-001] Add CI workflow. This 
connects the code changes directly to the task that required them. 
Anyone on the team can look at a commit and immediately know which 
Trello card it belongs to making it easy to track progress.

### 5. What did you learn from this project?
I learned how a real software team manages their work using tools 
like Trello, GitHub and GitHub Actions together. I learned that 
having a clear process for branching and committing makes teamwork 
much easier and prevents mistakes. I also learned how to set up 
automated testing so that code is always checked before it is merged. 
The most important lesson was that good engineering is not just about 
writing code but about having systems in place that keep the code 
clean, tested and well documented at all times.
