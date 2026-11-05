# Week 1 - Culture DevOps

## Run locally (Windows PowerShell)
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt -r requirements-dev.txt
uvicorn app.main:app --reload
```

## Check
```powershell
curl.exe -s localhost:8000/health
```
Expected: {"status":"ok"}

## Tests
```powershell
pytest
```

## Links
- Repo: https://github.com/medserghini1/capstone-devops-training
- Notion: <Capstone DevOps - Project Home link>
- Exercise 5 review: <Exercise 5 - AI Backlog Review link>
- Lead time card 1: <X h>
