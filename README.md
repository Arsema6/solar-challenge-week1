# solar-challenge-week1
# A project for learning Git and CI/CD.

## Setup
1. Clone: `git clone https://github.com/your-username/solar-challenge-week1.git`
2. Create venv: `python3 -m venv .venv`
3. Activate: `source .venv/bin/activate` (macOS/Linux) or `.venv\Scripts\activate` (Windows)
4. Deactivate: deactivate
5. Initialize: git init
6. Staging: git add . → git commit -m "chore: init"
7. Pushing: git push -u origin main
9. Install: `pip install -r requirements.txt`
10. requirements.txt: pip freeze > requirements.txt
# CI
name: CI

on: [push, pull_request]

jobs:

  build:
  
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Set up Python
        uses: actions/setup-python@v4
        with:
             python-version: '3.11'
      - name: Install deps
        run: pip install -r requirements.txt
      - name: Run tests
        run: python --version
