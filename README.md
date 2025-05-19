# solar-challenge-week1
# A project for learning Git and CI/CD.

## Setup
1. Clone: `git clone https://github.com/your-username/solar-challenge-week1.git`
2. Create venv: `python3 -m venv .venv`
3. Activate: `source .venv/bin/activate` (macOS/Linux) or `.venv\Scripts\activate` (Windows)
4. Deactivate: deactivate
5. Initialize: git init
6. Staging: `git add . → git commit -m "chore: init"`
7. Pushing: git push -u origin main
9. Install: `pip install -r requirements.txt`
10. requirements.txt: `pip freeze > requirements.txt`

#CI/Cd
1. Create a Workflow File
Navigate to your repo: `.github/workflows/ci.yml`
GitHub will automatically detect workflows in this directory.
name : Workflow name (e.g., CI)
on	: Triggers (e.g., push, pull_request)
jobs	: Defines tasks (e.g., build, test)
steps	: Individual commands to execute
