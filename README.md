# Secure GitFlow Demo

This project demonstrates a secure GitFlow workflow with local checks and CI enforcement.

## Local validation

python -m venv .venv
.venv\Scripts\activate
python -m pip install -r requirements.txt
python -m pytest -q
python scripts/secret_scan.py
python -m bandit -r app.py scripts
python -m pip_audit
