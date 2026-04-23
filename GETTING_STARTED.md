# Getting Started

Follow these steps to get set up in under 1 hour.

## 1. Prerequisites
- Ubuntu or any Linux system
- Git installed
- Python 3 installed

## 2. Clone the repo
```bash
git clone https://github.com/dashing00721/Gitops-workflow.git
cd Gitops-workflow
```

## 3. Set up virtual environment
```bash
python3 -m venv venv
source venv/bin/activate
```

## 4. Install dependencies
```bash
pip install -r requirements.txt
```

## 5. Run the tests
```bash
pytest test_app.py -v
```
You should see 8 tests passing.

## 6. Create your first branch
```bash
git checkout -b feature/TRELLO-00X-your-task
```

## 7. Make changes, commit and push
```bash
git add .
git commit -m "[TRELLO-00X] What you did"
git push origin feature/TRELLO-00X-your-task
```

## 8. Open a Pull Request on GitHub
- Go to your repo on GitHub
- Click Compare & pull request
- Add a title and click Create pull request
- Wait for CI to pass then merge

## Troubleshooting
- If pip not found: use pip3 instead
- If tests fail: make sure venv is activated
- If push fails: check your token has repo and workflow scope
