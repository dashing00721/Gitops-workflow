# Contributing Guide

## Workflow Overview
1. Pick a task from Trello board
2. Create a feature branch
3. Write code and commit
4. Push and open a Pull Request
5. Wait for CI to pass
6. Merge into main

## Branching Rules
- Never push directly to main
- Always create a feature branch first
- Branch naming: feature/TRELLO-###-description

Example:
```bash
git checkout -b feature/TRELLO-001-setup-ci
```

## Commit Format
Every commit must reference a Trello card ID:
