# OpenText Support AI Agent

Milestone 1 establishes the Python/FastAPI project scaffold and a health check.
No OpenText services or AI integrations are included yet.

## Run locally

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
uvicorn app.main:app --reload
```

The health endpoint is available at <http://127.0.0.1:8000/health> and returns
`{"status": "healthy"}`.

## Run tests

With the virtual environment activated and dependencies installed:

```bash
pytest
```