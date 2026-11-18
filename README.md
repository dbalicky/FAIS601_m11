# Setup

## Use python 3.10
```bash
pyenv local 3.10
```
**Add .python-version to gitignore**

## Initialize and set repo
```bash
git init

git remote add origin git@github.com:dbalicky/FAIS601_m11.git
```

## Create and activate venv
```bash
python3 -m venv venv

source venv/bin/activate
```

## Install dependencies from requirements.txt
```bash
pip install -r requirements.txt
```

## Update pip
```bash
pip install --upgrade pip
```

## Initial Commit and push to repo
```bash
git add .

git commit -m 'initial commit'

git push -u origin main
```

# Issues

## Assertion Errors

Pytest resulted in 2 failed tests in test_e2e.py with 2 assertion errors. Retried pytest a few times and they passed.

## Trivy Security Errors
**Updated following dependency versions**
```txt
anyio==4.14.2
certifi==2026.10.18
setuptools==78.1.1
urllib3==2.8.0
```

**Reinstalled dependencies with updated versions**
```bash
pip install -r requirements.txt --upgrade
```